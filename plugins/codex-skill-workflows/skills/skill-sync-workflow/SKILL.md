---
name: skill-sync-workflow
description: Use when the user asks to update, sync, publish, install, compare, or check a personal Codex skill between the local Codex skills directory and the GitHub repository xufeng-code/my-codex-skills.
---

# Skill Sync Workflow

Use this skill to keep Xufeng's personal Codex skills consistent across:

- Local callable skills: `/Users/bytedance/.codex/skills/<skill-name>/`
- Working-copy drafts when present: the current repo's `skills/<skill-name>/` or `plugins/*/skills/<skill-name>/`
- GitHub source of truth: `xufeng-code/my-codex-skills`

Do not rely on conversational memory. Treat this file as the operating rule whenever the user says "更新这个 skill", "同步 skill", "推到 GitHub", "安装这个 skill", "检查 skill 是否一致", or names a skill and asks for local/GitHub consistency.

## Source Of Truth

The long-term source repository is:

`https://github.com/xufeng-code/my-codex-skills`

The repository is expected to store installable plugins under:

`plugins/<plugin-name>/skills/<skill-name>/`

The local callable copy is expected under:

`/Users/bytedance/.codex/skills/<skill-name>/`

## Default Mapping

Use these mappings unless the repository shows a newer structure:

- `product-demand-design` -> `plugins/prd-writing-styles/skills/product-demand-design/`
- `luojing-prd-review` -> `plugins/prd-writing-styles/skills/luojing-prd-review/`
- `zijun-prd-style` -> `plugins/prd-writing-styles/skills/zijun-prd-style/`
- `pyramid-communication` -> `plugins/pyramid-communication/skills/pyramid-communication/`
- `skill-sync-workflow` -> `plugins/codex-skill-workflows/skills/skill-sync-workflow/`

If the skill is new and no mapping exists, choose or create the narrowest plugin that matches the skill's purpose. Prefer a new plugin only when no existing plugin is semantically appropriate.

## When User Says "Call A Skill"

If the user asks to use a skill, use the local installed version first:

`/Users/bytedance/.codex/skills/<skill-name>/SKILL.md`

Only fetch GitHub when the local version is missing, the user explicitly asks for the latest remote version, or there is reason to suspect drift.

## When User Says "Update This Skill"

Treat that as authorization to update both the local callable copy and the GitHub repository for that named skill. Still avoid unrelated changes.

Follow this sequence:

1. Resolve the skill name from the user's message or recent context.
2. Read the local callable copy from `/Users/bytedance/.codex/skills/<skill-name>/` when it exists.
3. Also inspect any working-copy draft under `skills/<skill-name>/` or `plugins/*/skills/<skill-name>/` when present.
4. Fetch the mapped GitHub files and SHAs before writing.
5. Decide the freshest intended content from the user's latest request and local edits. If both local and remote changed in conflicting ways, stop and summarize the conflict instead of overwriting.
6. Update the local callable copy.
7. Update the GitHub plugin copy in `xufeng-code/my-codex-skills`.
8. If creating a new skill inside a new plugin, add or update the plugin manifest and `.agents/plugins/marketplace.json`.
9. Report the local path, GitHub path, and commit SHA.

## Safety Rules

- Do not push meeting transcripts, private company data, credentials, tokens, or raw links unless the user explicitly asks and the content is appropriate for the private repository.
- Summarize sensitive source material into durable method notes instead of copying full confidential documents.
- Do not delete a remote skill unless the user explicitly asks to delete it.
- Do not overwrite remote content when local and remote have diverged in meaning; ask for direction or preserve both with clear names.
- Do not claim the skill is active in already-open tasks. New or refreshed tasks are the reliable way to load newly installed skills.

## Useful Checks

For local inspection:

```bash
find /Users/bytedance/.codex/skills -maxdepth 2 -name SKILL.md -print
```

For a local skill:

```bash
sed -n '1,220p' /Users/bytedance/.codex/skills/<skill-name>/SKILL.md
```

For the GitHub repository, use the GitHub connector when available:

- Fetch repository metadata.
- Fetch `git/trees/main?recursive=1`.
- Fetch target files to get current SHAs.
- Create or update files through the contents API.

## Completion Response

After syncing, answer briefly with:

- Skill name.
- Whether local callable copy was updated.
- Whether GitHub was updated.
- GitHub path and latest commit SHA.
- Any caveat, such as "new tasks may be needed to load the latest skill list."

## Cross-Device Prompt

When the user asks for a prompt to send to another computer's Codex, provide the prompt in `references/cross-device-install-prompt.md`.

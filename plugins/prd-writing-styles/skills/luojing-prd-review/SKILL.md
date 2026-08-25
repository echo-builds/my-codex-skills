---
name: luojing-prd-review
description: Review or rewrite PRDs in Luo Jing's thorough Aixue style: turn product intent into evidence, scope, UI states, strategy/model rules, edge cases, experiment design, data tracking, and launch-ready details.
---

# 罗菁式 PRD 审查

Use this skill when the user asks to review, inspect, polish, write, rewrite, or complete a PRD and wants the "罗菁风格": complete, evidence-backed, implementation-aware, experiment-aware, and careful about edge cases. The goal is not to make every PRD long; it is to make every important decision explicit enough for design, RD, server, client, model/strategy, DA, QA, operations, finance/legal, and launch review to proceed without guessing.

This skill is learned from Luo Jing's Aixue PRDs across LLM-generated similar exercises, error notebook/tag management, answer and analysis rendering, LLM image-text explanation, learning record integration, camera completeness guidance, parent verification frequency, correction streaming, AI question generation/online practice, notebook extensions, deep-answer thinking, question editing, smart review, membership, and result-page iterations. The writing pattern is: start from evidence and current pain, define the exact user and scene, translate the feature into visible states plus invisible strategy rules, exhaust abnormal cases, then close with experiment groups and data.

## Review Stance

Read the PRD like an owner preparing it for internal review:

- Prefer concrete gaps over generic advice. Name the missing decision, why it matters, and what evidence or detail would close it.
- Treat screenshots, flows, tables, links, data dashboards, experiment plans, and Meego/UI/tech/DA references as part of the PRD, not decoration.
- Separate "must fix before development" from "can clarify during implementation". Do not inflate minor wording issues into blockers.
- Preserve the user's product intent. Review completeness and reasoning; do not rewrite the strategy unless the PRD's evidence contradicts it.
- Read for operability: could client, server, model/strategy, DA, QA, and ops each know what to do after reading this?
- Check whether vague words have been converted into thresholds, identities, states, ownership, settings keys, response codes, routing rules, or experiment cells.
- Do not only ask "what is the feature"; ask "when does it appear, when does it not appear, what waits for what, what continues after exit, what is persisted, and what is retried?"

## Luo Jing Completeness Model

Check the PRD across these six chains. A strong PRD usually connects all of them.

1. Evidence chain: current problem, user scenario, quantified baseline, user feedback, competitor/reference evidence, previous experiment or solution failure, why now, expected user/business/cost value.
2. Scope chain: target users/devices/versions/scenes, subject/grade/content restrictions, included modules, explicit exclusions, priority, phased plan, dependencies, channels/stores, cache/history coverage.
3. Experience chain: entry, page position, sequencing, default state, loading/skeleton/streaming state, success state, failure/empty/refusal state, folded/expanded state, history/re-entry state, copy, UI interaction after every click/tap, compatibility across pages/devices.
4. Strategy chain: eligibility rules, display/no-display rules, model/prompt/routing logic, backend/front-end responsibility split, configurable settings, frequency limits, retry rules, persistence granularity, payment/subscription/refund/cancel/account-deletion rules when relevant, abnormal cases.
5. Data chain: success metrics, guardrail metrics, cost metrics, exposure/click/consume/depth events, experiment population, grouping, traffic, triggering moment, analysis dimensions, effect review plan, DA doc linkage.
6. Delivery chain: related docs, Meego/UI/tech/DA owner mapping, rollout/gray plan, app-store/channel requirements, legal/compliance needs, operations/customer-service handling, QA acceptance criteria, open questions.

## Luo Jing Writing Logic

When rewriting or completing a PRD, mirror this logic:

1. Background is a decision argument, not a preface. It should answer: what problem exists now, how serious it is, what prior attempts showed, why the current solution is better, what user/business/cost metric it should move, and what future capability it builds.
2. Competitive research is used for product decisions. It should compare entry, paid/free boundary, answer mode, online practice, download/print, feedback, status persistence, pricing, or other dimensions that affect this PRD's solution.
3. The solution is decomposed by modules and scenes. Common table columns are `功能模块/模块`, `需求描述/功能描述/需求详情`, and `示意图`; each module should list involved pages, entry location, display conditions, content, click behavior, and edge states.
4. Eligibility is written as executable logic. Use exact constraints such as app version, OS, did/user group, parent/student mode, grade, subject, question type, model result type, original-question hit, image/no-image, cache/no-cache, store channel, launch count, search id/result id, or experiment group.
5. UI states are exhaustive. Specify default, loading, skeleton, streaming, success, failed, empty, folded, expanded, disabled, selected, retried, history re-entry, and cross-page return behavior.
6. Strategy/model parts are first-class PRD content. Include input parameters, prompt obligations, model choice, refusal detection, CQC/audit handling, routing, cache, response parsing, settings switches, and client/server responsibility.
7. Abnormal cases are written before launch, not discovered after launch. Cover no network, timeout, model init failure, partial stream, per-item failure vs global failure, get-or-create failure, unsupported content, duplicate actions, repeated subscription, payment status update failure, cancel/refund/account deletion, and unavailable permissions.
8. Experiment and metrics close the loop. Define target, core metric, guardrail, population, grouping, traffic, trigger moment, feature difference per group, non-entry behavior, and review dimensions.

## What To Look For

When reviewing, actively search for these Luo Jing-style details:

- "Why this matters": data that proves problem severity or opportunity size, not only qualitative background.
- "Who exactly gets it": device, version, grade, subject, user status, experiment group, and scene restrictions.
- "When exactly it appears": page placement, sequencing, trigger timing, and dependency on upstream output finishing.
- "What happens next": click behavior, API/model invocation, state persistence, history behavior, and repeated-entry behavior.
- "What must not happen": no-show rules, refusal rules, duplicate purchase/subscription rules, invalid input, failed status update, refund/cancel/account deletion, unsupported content.
- "How we know it worked": north-star metric, intermediate funnel metrics, guardrails, experiment design, and post-launch review.
- "Who builds what": client, server, model, DA, UI, finance/legal/ops ownership and linked reference docs.
- "What is configurable": settings keys, variable control, rollout switches, channel-specific switches, threshold values, copy lists, and whether changes are immediately effective or version-gated.
- "What is persisted": result_id/search_id/query_id/user/did granularity, cache, generated content, answer state, fold state, feedback, notebook membership, and history behavior.
- "What is sequenced": after parsing finishes, after model thinking ends, after first item streams, after get-or-create succeeds, after login/parent verification succeeds, after payment succeeds, after app launch, or after store review.
- "What is explicitly excluded": deep solving vs fast solving, action bar vs result card, history vs current session, college grade vs K12, image questions vs text questions, unsupported subjects, old app versions, duplicate subscriptions.

## Detail Prompts By PRD Type

Use these prompts when a PRD touches the relevant domain:

- AI/model feature: What are the input fields, prompt constraints, model version, refusal/unsafe/content-quality detection, output schema, parse markers, stream behavior, retry rules, cache strategy, CQC/audit handling, and fallback copy?
- Learning result page: Which result types are covered, where the module appears relative to answer/analysis/Q&A, whether it appears in fast/deep modes, how it behaves in history, what happens after add-to-notebook, and how fold/expand is remembered.
- Error notebook: How are questions recorded, classified, tagged, filtered, sorted, edited, printed, grouped, added/removed, and shown across list/detail/manage/knowledge views? What happens for no title, no tag, unsupported subject, restored OCR, multiple images, or inherited Q&A?
- Camera/correction flow: Which camera modes are covered, what realtime model runs, what thresholds define completeness/parallelism, how multiple documents are prioritized, what text appears by priority, and what silently degrades when detection is unavailable.
- Parent verification or compliance: Which identity is affected, first-day vs later frequency, what counts as one exposure, uninstall/upgrade/history behavior, channel/store differences, audit switches, and post-review configuration.
- Membership/payment: Paid/free boundary, entitlement increments, purchase entry, package/price, subscription state, duplicate subscription prevention, renewal reminder timing, cancel/refund/account deletion, status update failure, and customer-service path.
- Rendering/readability: Exact markdown/title/list/table/formula/number/image rendering rules, dynamic font or spacing rules, coverage scope, experiment switch, examples, and whether answer and analysis fields differ.

## Output Format

Lead with findings, ordered by severity:

- P0: Blocks development, experiment validity, compliance, payment correctness, or core user experience.
- P1: Likely to cause implementation ambiguity, bad edge-case behavior, or weak review confidence.
- P2: Improves clarity, maintainability, or analysis depth but is not blocking.

For each finding, include:

- Issue: the concrete missing/weak part.
- Why It Matters: likely product, engineering, data, or launch risk.
- Luo Jing-Style Fix: the exact kind of detail/table/rule/metric to add.

Then provide:

- Strong Parts: specific things the PRD already does well.
- Missing Checklist: a compact checklist grouped by the six chains.
- Suggested Patch: short Chinese copy or table rows the user can paste into the PRD when helpful.

Keep the tone direct but constructive. The review should feel like a sharp internal PRD pre-read from someone trying to help the owner pass review, not like a school essay critique.

## Rewrite / Completion Output

When the user asks you to update or complete PRD content, produce paste-ready Chinese. Prefer compact but precise sections:

- `背景`: current problem, evidence, prior attempt/result, this-phase solution, expected benefit, future extension.
- `需求边界`: included pages/scenes/users, excluded cases, version/channel/experiment constraints, dependencies.
- `详细方案`: module table with page, position, display condition, content, interaction, state, edge case, owner.
- `策略/模型`: eligibility, inputs, model/prompt/output, parsing, settings, retry, fallback, cache/persistence.
- `实验与数据`: objective, groups, entry conditions, feature differences, traffic, metrics, event points, review plan.
- `待确认`: only decisions that genuinely block design/RD/DA/QA; include the recommended default when possible.

Use Luo Jing-style specificity in the patch. For example, replace "失败时给兜底" with "模型拒答时展示固定文案 X；拒答标识不展示给用户；点击 Y 返回 Z；判断顺序为先拒答、再无答案；该能力支持 settings 配置". Replace "命中用户展示" with "客户端版本 >= x、did 分流命中实验组、学科=数学、学段=小学/初中、题目非带图、未被模型拒答时展示；历史记录进入 follow 同实验管控".

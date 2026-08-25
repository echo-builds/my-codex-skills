---
name: luojing-prd-review
description: Review PRDs in Luo Jing's thorough Aixue style: check whether background, scope, user flows, rules, data, experiments, and launch risks are detailed enough to build and validate.
---

# 罗菁式 PRD 审查

Use this skill when the user asks to review, inspect, polish, or complete a PRD and wants the "罗菁风格": complete, evidence-backed, implementation-aware, and careful about edge cases. The goal is not to make every PRD long; it is to make every important decision explicit enough for design, RD, DA, QA, operations, and launch review to proceed without guessing.

## Review Stance

Read the PRD like an owner preparing it for internal review:

- Prefer concrete gaps over generic advice. Name the missing decision, why it matters, and what evidence or detail would close it.
- Treat screenshots, flows, tables, links, data dashboards, experiment plans, and Meego/UI/tech/DA references as part of the PRD, not decoration.
- Separate "must fix before development" from "can clarify during implementation". Do not inflate minor wording issues into blockers.
- Preserve the user's product intent. Review completeness and reasoning; do not rewrite the strategy unless the PRD's evidence contradicts it.

## Luo Jing Completeness Model

Check the PRD across these six chains. A strong PRD usually connects all of them.

1. Evidence chain: current problem, user scenario, quantified baseline, competitor/reference evidence, why now, expected user/business value.
2. Scope chain: target users/devices/versions/scenes, included modules, explicit exclusions, priority, phased plan, dependencies.
3. Experience chain: entry, default state, loading state, success state, failure/empty state, history/re-entry state, copy, UI position, interaction after click/tap, compatibility across pages/devices.
4. Strategy chain: eligibility rules, model/prompt/routing logic, backend/front-end responsibility split, configurable settings, frequency limits, payment/subscription/refund rules when relevant, abnormal cases.
5. Data chain: success metrics, guardrail metrics, exposure/click/consume/depth events, experiment population, grouping, triggering moment, analysis dimensions, effect review plan.
6. Delivery chain: related docs, owner mapping, rollout/gray plan, legal/compliance needs, operations/customer-service handling, QA acceptance criteria, open questions.

## What To Look For

When reviewing, actively search for these Luo Jing-style details:

- "Why this matters": data that proves problem severity or opportunity size, not only qualitative background.
- "Who exactly gets it": device, version, grade, subject, user status, experiment group, and scene restrictions.
- "When exactly it appears": page placement, sequencing, trigger timing, and dependency on upstream output finishing.
- "What happens next": click behavior, API/model invocation, state persistence, history behavior, and repeated-entry behavior.
- "What must not happen": no-show rules, refusal rules, duplicate purchase/subscription rules, invalid input, failed status update, refund/cancel/account deletion, unsupported content.
- "How we know it worked": north-star metric, intermediate funnel metrics, guardrails, experiment design, and post-launch review.
- "Who builds what": client, server, model, DA, UI, finance/legal/ops ownership and linked reference docs.

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

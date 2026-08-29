---
name: product-demand-design
description: Use when designing, reviewing, or preparing product requirements and PRDs before development, especially when a proposal needs end-state thinking, pre-launch benefit validation, online/offline evidence, tradeoff analysis, and a transition plan.
---

# Product Demand Design

Use this skill to turn a product idea from a UI proposal into a judged product hypothesis. The core standard is: before designing the solution, estimate the demand's likely value, affected users, upside, downside, and end-state fit as far as possible.

## Core Principle

Do not bring only a UI change to review. Bring a judged hypothesis:

- What is the product end-state this demand moves toward?
- Which user segment and job does it improve?
- If the demand already existed today, what existing online behavior or offline replay could approximate its effect?
- What benefit, loss, cost, and badcases are expected before launch?
- Is the current proposal a step toward the end-state, or a detour that patches a symptom?

## Workflow

1. Start From End-State
   - Define what the product should look like in 3-6 months.
   - Decide whether the capability is a core capability in the main flow or an extra branch that should jump out.
   - For each entry and output, explain whether it belongs in the main conversation/result flow or in a separate tool page.

2. Segment Users Before Designing UI
   - Split users by intent and dependency, not just by page source.
   - Identify users who only need a quick answer, users who need detailed explanation, users whose follow-up depends on the visible explanation, and users dissatisfied with the answer.
   - Mark the counter-user: the group that may be harmed by the new design.

3. Validate Before Launch
   - Ask: "If this demand existed today, how would I verify it using current data?"
   - Use online proxy behavior, historical cohorts, query classification, click/long-press/follow-up paths, retention, satisfaction, latency, and conversion as evidence.
   - For AI/model features, run offline replay by scene and subject with tools on/off before committing development.

4. Turn Evidence Into A Decision
   - State the decision, affected traffic, expected gain, expected loss, and uncertainty.
   - Avoid showing broad background data that does not prove the decision.
   - Use the exact rule being proposed for evaluation, not an averaged or adjacent metric.

5. Choose A Main Proposal
   - Do not present several equal options without judgment.
   - Name the recommended proposal, why it wins, and why other proposals are rejected.
   - If the ideal solution is too large, still state it as the end-state and design the smallest transition step toward it.

6. Design The Transition
   - Separate final state from interim state.
   - Explain what the interim state validates.
   - Check whether the interim state reduces future rework or creates a dead-end path.

7. Make Tradeoffs Explicit
   - State what is sacrificed for what: accuracy for resource, latency for quality, flow consistency for depth, or information density for clarity.
   - For downgrade/resource strategies, show traffic coverage, quality loss, resource saved, staircase rollout, monitoring, and rollback.

8. Define Launch Criteria
   - Specify success metrics, guardrail metrics, sample checks, badcase review, and no-go thresholds.
   - State what result would falsify the hypothesis and what the next iteration would be.

## Review Questions

- If this feature already existed today, what data could prove it is useful?
- Which current user behavior is the closest proxy for the future behavior?
- What user group may be hurt by this proposal?
- Is this solving the product structure or only changing UI?
- Is the capability part of the product's main flow or an external add-on?
- What is the final product form, and is this proposal the shortest reasonable path toward it?
- What exact metric proves the proposed rule, not just the general direction?
- What happens if the hypothesis is wrong?

## Output Template

Use this structure when producing or reviewing a demand:

1. One-sentence judgment
2. Product end-state
3. Current problem
4. User segments and affected traffic
5. Evidence and proxy data
6. Recommended solution
7. Rejected alternatives
8. Transition plan
9. Tradeoff ledger
10. Validation and launch plan
11. Risks, badcases, and fallback

## Meeting Response Pattern

When challenged in a review, first identify the level of the question:

- "I understand this is not only a UI question. The core question is whether this capability should live in the main flow or as a separate branch."
- "The data I have proves the broad opportunity, but it does not yet prove this specific rule. I need to add validation for the exact affected group."
- "The final state should be X. The current proposal is an interim step to validate Y. If Y is true, the next step is Z."
- "The group most likely to be harmed is A. I will verify its size and behavior through B before deciding whether this design is acceptable."

## Anti-Patterns

- Starting from visual form before defining product position.
- Listing multiple schemes without a recommended answer.
- Using background opportunity data as decision evidence.
- Saying "launch first and see" when pre-launch proxy validation is possible.
- Optimizing a local UI issue while ignoring the future product architecture.
- Evaluating an averaged metric instead of the exact rule being proposed.
- Hiding a real tradeoff behind vague words like "better experience" or "consistency."
- Missing the badcase user whose existing path is degraded by the new solution.

## Domain Notes

For learning Q&A and problem-solving flows:

- Decide whether solving, correction, explanation, and follow-up are native conversation capabilities or separate tool-page capabilities.
- Distinguish answer-first users, explanation-reading users, explanation-anchored follow-up users, and answer-dissatisfied users.
- If follow-up depends on visible explanation context, hiding or separating the explanation may hurt that group.
- A UI patch is weak if the long-term direction is to render the capability natively in the main learning conversation.

For model/tool/RAG features:

- Validate independent tool gain through offline replay before development.
- Break results down by subject, task type, source, latency, quality, and badcase class.
- If query-time retrieval can be converted into an offline index or question bank, compare both paths before choosing runtime search.

For model downgrade or resource strategies:

- Evaluate the exact downgrade rule, not the global model average.
- Show quality loss, resource saved, traffic coverage, and the rollout staircase.
- Make clear which user experience is being sacrificed and why it is acceptable.

## Source Pattern

This skill is distilled from Zhao Rui's product review pattern in the 2026-08-28 Doubao Aixue internal product review. For the detailed reasoning chain, read `references/zhao-rui-review-pattern.md`.
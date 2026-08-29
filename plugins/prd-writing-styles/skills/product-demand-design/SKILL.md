---
name: product-demand-design
description: Use when helping the user think through any product demand, opportunity, proposal, or decision before action, especially when they need end-state reasoning, user segmentation, evidence, tradeoff analysis, and pre-launch judgment.
---

# Product Demand Thinking

Use this skill as a thinking partner before a product decision becomes a plan, PRD, UI change, experiment, model strategy, or resource tradeoff. The goal is not to force every question into a PRD format. The goal is to help the user form a sharper judgment: what is true, what is assumed, what can be verified now, what is worth doing, and what path avoids unnecessary detours.

## Core Principle

Do not start from "what should we build?" Start from "what should we believe before we build?"

Every demand should become a judged hypothesis:

- End-state: what future product direction does this move toward?
- User truth: whose problem is this, and whose experience may be damaged?
- Evidence: if this already existed today, what current data or proxy behavior could verify it?
- Tradeoff: what is gained, what is sacrificed, and whether that exchange is acceptable?
- Path: is this the shortest reasonable step toward the end-state, or a local patch?

## Operating Modes

Choose the lightest mode that fits the user's ask.

- Thinking mode: help the user reason aloud, ask sharper questions, expose hidden assumptions, and propose validation paths.
- Review mode: critique an existing idea, meeting discussion, PRD, UI proposal, experiment, or strategy.
- Drafting mode: only when the user asks for a written artifact, turn the thinking into a structured plan, PRD section, review memo, or meeting response.

In thinking mode, do not over-format. Prefer a concise diagnosis, a small set of key questions, and a recommended next move.

## Workflow

1. Start From End-State
   - Define what the product, business, or user relationship should look like in the relevant future window.
   - Decide whether the demand is part of the core flow, an add-on, a patch, an experiment, or an operational necessity.
   - Ask whether the proposed direction compounds into the future product or creates future rework.

2. Segment Users Before Designing The Solution
   - Split users by intent, motivation, dependency, frequency, and sensitivity to regression.
   - Identify the primary beneficiary, secondary beneficiary, neutral group, and harmed group.
   - Mark the counter-user: the group that may be harmed by the new design.

3. Validate Before Launch
   - Ask: "If this demand existed today, how would I verify it using current data?"
   - Use existing online behavior, historical cohorts, manual review, offline replay, user interviews, logs, funnel data, retention, satisfaction, quality, cost, and latency as possible evidence.
   - Prefer evidence that validates the exact decision being made, not only the general opportunity.

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
   - State what is sacrificed for what: accuracy for resource, latency for quality, simplicity for depth, consistency for flexibility, growth for retention, or speed for confidence.
   - If the decision is a tradeoff, quantify both sides and define the acceptable loss.

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

Use this structure when a written artifact is useful. For quick thinking, answer only the relevant parts.

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

When challenged in a review, first identify the level of the question. The useful move is to rise from the local answer to the underlying judgment:

- "I understand this is not only a local solution question. The core question is whether this demand belongs in the future product direction."
- "The data I have proves the broad opportunity, but it does not yet prove this specific decision. I need to add validation for the exact affected group."
- "The final state should be X. The current proposal is an interim step to validate Y. If Y is true, the next step is Z."
- "The group most likely to be harmed is A. I will verify its size and behavior through B before deciding whether this tradeoff is acceptable."

## Anti-Patterns

- Starting from visual form before defining product position.
- Listing multiple schemes without a recommended answer.
- Using background opportunity data as decision evidence.
- Saying "launch first and see" when pre-launch proxy validation is possible.
- Optimizing a local symptom while ignoring the future product architecture.
- Evaluating an averaged metric instead of the exact rule being proposed.
- Hiding a real tradeoff behind vague words like "better experience" or "consistency."
- Missing the badcase user whose existing path is degraded by the new solution.

## References

This skill is generalized from Zhao Rui's product review pattern in the 2026-08-28 Doubao Aixue internal product review. Read `references/zhao-rui-review-pattern.md` only when the user asks about that meeting, the original examples, or how this thinking pattern appeared in a real review.
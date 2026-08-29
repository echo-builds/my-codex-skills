# Zhao Rui Review Pattern

This note distills the reasoning pattern from the 2026-08-28 Doubao Aixue internal product review. It is a reference for applying the `product-demand-design` skill.

## Boss's Core Standard

The repeated challenge was not "make the UI better." It was: before a requirement enters design or development, the product manager should already have a reasonably clear hypothesis about its benefit, affected users, cost, and risk.

His implicit bar is:

- Think from the product end-state.
- Use today's data to approximate tomorrow's outcome.
- Validate the specific decision, not just the general direction.
- Find the user segment that benefits and the segment that may be damaged.
- Choose a path that moves toward the end-state with the fewest detours.

## Requirement 1: Q&A And Problem-Solving Linkage

The proposal context:

- From the Q&A homepage, users open the camera.
- After taking a photo of a problem, users enter a half-sheet result page.
- Users can long-press an explanation to ask a follow-up, or use the bottom input box to ask a follow-up.
- The new proposal tried to reduce confusion between result-page follow-up and Q&A follow-up.

The boss's challenge:

- The premise was not fully proven: how many users ask because they are reading a specific explanation at its original position?
- How many bottom-input follow-ups are still explanation-related, even without long-pressing a specific paragraph?
- If the new design moves follow-up into Q&A or hides the explanation, will it damage users whose question depends on reading the explanation?
- The proposal looked like a UI repair, but the deeper question was product positioning: in six months, is Doubao Aixue primarily a learning conversation product? If yes, problem-solving and correction may be native abilities of the main flow, not separate result pages.

The reasoning chain:

1. Ask what the product should become in six months.
2. Ask whether solving/correction is a basic ability or an extra branch.
3. If it is a basic ability, ask why the user should jump away from the conversation flow.
4. Split users into quick-answer users, explanation-reading users, explanation-anchored follow-up users, and answer-dissatisfied users.
5. Use current behavior to estimate each group: direct-answer behavior, camera-entry behavior, long-press follow-up, bottom-input follow-up, and downstream retention.
6. Decide whether the best direction is native rendering in Q&A, result-page continuation, or an interim hybrid.

Product lesson:

The right PRD should not start with "three UI schemes." It should first answer: "What role should problem-solving play in the future learning conversation, and what data proves today's step is the shortest path toward that state?"

## Requirement 2: 2B5 Model Downgrade

The proposal context:

- Resource was tight, so some correction requests might use a smaller model.
- The proposed rule covered requests with no image, Chinese/math/English, primary school, and correction source.

The boss's challenge:

- The decision is not "is the smaller model generally acceptable?"
- The decision is "under this exact downgrade rule, how much quality is lost and how much resource is saved?"
- If the team is intentionally sacrificing accuracy for resource, the tradeoff must be shown clearly.

The reasoning chain:

1. State the exact downgrade strategy.
2. Calculate the traffic hit by that strategy.
3. Evaluate quality loss only on that exact traffic.
4. Calculate resource saved.
5. Decide the stepwise rollout: which traffic first, what threshold, what monitoring, what rollback.

Product lesson:

When the essence of a strategy is a tradeoff, do not hide it. Say plainly what is being exchanged, quantify both sides, and make the rollout staircase visible.

## Requirement 3: RAG And Tool Search

The proposal context:

- Question-bank RAG had clear offline gains.
- Web search and calculator use had less certain independent gains.

The boss's challenge:

- Do not build first and then learn whether it works if an offline validation is possible.
- Run existing samples through tools on/off, split by subject and scene, and inspect benefit, latency, and badcases before development.
- If web search can retrieve original questions, ask whether those questions should be crawled/indexed into the question bank instead of using expensive query-time search.

Product lesson:

For AI capabilities, product validation increasingly resembles model evaluation: define the test set, run controlled comparisons, segment the results, and decide based on measurable gain.

## Communication Lesson

In review, the product manager should quickly rise to the boss's abstraction level:

- If the boss asks about end-state, stop explaining the current UI details.
- If the boss asks about affected users, stop describing interaction mechanics and give segment sizes or say which data is missing.
- If the boss asks about a tradeoff, state the tradeoff directly.
- If the boss identifies the ideal final state, immediately map the current proposal to that final state: is it aligned, partial, or a detour?

The ideal response is not defensive. It should sound like:

"I get it. The core question is whether this is a native capability of the learning conversation, not where to put the button. The missing evidence is the share of follow-ups that depend on the visible explanation. I will use long-press follow-up, bottom-input follow-up after explanation exposure, and direct-answer retention as proxy data. If that group is large,方案一 may hurt them; if the end-state is native Q&A rendering,方案三 should be the main direction and方案一 is only a temporary patch."
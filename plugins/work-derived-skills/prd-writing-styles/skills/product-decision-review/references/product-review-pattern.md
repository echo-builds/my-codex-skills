# Product Review Pattern

This note distills a reusable reasoning pattern for product demand reviews. It is intentionally generic and should not depend on private meeting transcripts or company-specific examples.

## Core Standard

Before a requirement enters design or development, the product manager should have a reasonably clear hypothesis about its benefit, affected users, cost, and risk.

The bar is:

- Think from the product end-state.
- Use today's data to approximate tomorrow's outcome.
- Validate the specific decision, not just the general direction.
- Find the user segment that benefits and the segment that may be damaged.
- Choose a path that moves toward the end-state with the fewest detours.

## Pattern 1: Capability Positioning Before UI Repair

When a proposal is framed as an interaction change, ask whether the problem is actually about product positioning.

Reasoning chain:

1. Ask what the product should become in the relevant future window.
2. Ask whether the capability is a basic ability in the main flow or an extra branch.
3. If it is a basic ability, ask why the user should jump away from the main flow.
4. Split users by intent and dependency: quick-completion users, detail-reading users, anchored-follow-up users, and dissatisfied-result users.
5. Use current behavior to estimate each group before launch.
6. Decide whether the right direction is native integration, a separate result surface, or an interim hybrid.

Product lesson:

Do not start with several UI schemes. First answer what role the capability should play in the future product, and what data proves today's step is the shortest path toward that state.

## Pattern 2: Tradeoff Decisions Need Exact Evaluation

When a strategy intentionally sacrifices one product quality for another, do not hide the exchange.

Reasoning chain:

1. State the exact strategy or rule.
2. Calculate the traffic hit by that strategy.
3. Evaluate the quality loss only on that exact traffic.
4. Calculate the benefit gained.
5. Decide the rollout staircase, thresholds, monitoring, and rollback.

Product lesson:

The decision is not whether the general direction is acceptable. The decision is whether this exact rule produces an acceptable exchange.

## Pattern 3: AI Capability Validation Before Development

For AI capabilities, validation often resembles model evaluation.

Reasoning chain:

1. Define the test set and target scenes.
2. Run controlled comparisons with the capability on and off.
3. Segment the results by subject, user scene, difficulty, content type, latency, cost, and badcases.
4. If an expensive online tool helps by retrieving stable knowledge, ask whether that knowledge should be indexed offline instead.
5. Build only after the expected gain and risk are reasonably clear.

Product lesson:

Do not build first and then learn whether it works when offline validation is possible.

## Review Response Pattern

When challenged in a review, identify the level of the question and answer there:

- If asked about end-state, stop explaining current UI details.
- If asked about affected users, give segment sizes or name the missing data.
- If asked about a tradeoff, state what is being exchanged.
- If the ideal final state is identified, map the current proposal to it: aligned, partial, or a detour.

The useful response sounds like:

"The core question is whether this capability belongs in the main product flow, not where to put the button. The missing evidence is the size of users whose behavior depends on the current surface. I will use existing exposure, action, follow-up, and retention data as proxy evidence. If that group is large, the lightweight UI patch may hurt them; if the future state is native integration, the interim plan should minimize throwaway work."

---
name: prd-strategic-framing
description: Write, rewrite, or review a PRD's background, desired outcome, product judgment, competitor or reference analysis, scope, high-level solution, and validation narrative. Use when detailed requirements may exist but the document does not yet explain clearly why the problem matters, why this solution shape is appropriate, what this phase will and will not do, or how results should be interpreted.
---

# PRD Strategic Framing

Use this skill when the user asks to write, revise, summarize, or review a PRD in "子隽风格", especially the sections before detailed requirements: background, product judgment, competitor/reference analysis, scope, high-level solution, launch rhythm, and experiment framing.

Do not treat this as a fixed formatting template. The style is a product-thinking method: turn scattered research, past attempts, user feedback, data, and feature ideas into a clear judgment chain that explains why this problem matters now, why this solution shape fits this product, what this phase deliberately does and does not do, and how the team will know whether it worked.

## Core Thinking Chain

Prefer this chain when the material allows it:

1. Context: what changed, what prior discussion, experiment, data, or business moment makes the decision necessary now.
2. Problem: state the real user/product problem before listing functions. When useful, separate it by "For 心智/增长", "For 用户体验", "For 成本/效率", or another decision-relevant axis.
3. Evidence: use user feedback, online data, prior experiment results, competitor/reference products, and current-product constraints as inputs, not decoration.
4. Abstraction: compress the evidence into 1-3 product dimensions or user states, such as learning intent strength, entry timing, answer efficiency vs guided exploration, content density, certainty vs openness, or tool use vs companion service.
5. Judgment: write the crisp product conclusion. Examples of the form: "知识 query 不等于想学习", "给出答案只是开始", "同步学和同步练是两类需求", "一刀切讲解无法继续满足分层用户".
6. Choice: explain the selected solution shape, why alternatives are not selected now, and which pieces are reused from existing capabilities.
7. Phase scope: name what this phase does, what is out of scope, what is pending, and what moves to a later PRD.
8. Validation: define the experiment or metric logic, including expected effect, key tradeoff, and what positive or negative results should cause the team to conclude.

## Common PRD Shapes

Choose the lightest shape that fits the task. Zijun-style clarity comes from matching the document shape to the decision, not making every PRD long.

- Strategy or major revision PRD: `项目背景 -> 产品比较/线上数据 -> 优化方向 -> 阶段计划 -> 本期需求范围 -> 需求详情 -> 数据需求`.
- Formal launch PRD: `整体背景 -> 整体节奏计划 -> 要解决的问题 -> 需求 list 概览 -> 需求详情 -> 成本/数据/实验`.
- Capability framework PRD: `要解决的问题 -> 能力价值/行业做法 -> 阶段框架 -> 本期范围 -> 预期收益 -> 未来打算 -> 需求详情`.
- Narrow feature PRD: `背景与判断 -> 一句话方案 -> 核心方案示意 -> 需求详情 -> 数据需求 -> 附录：方案权衡`.
- Page or information architecture PRD: `背景 -> 改版考虑 -> 核心页面示意 -> 需求 list 及优先级 -> 分模块详情 -> 实验设计`.

## Writing Moves

- Start from judgment, not feature inventory. The reader should understand why the feature is necessary before seeing UI details.
- Use "背景与判断", "要解决的问题", "改版考虑", or "为什么要再试一次" to force the document to answer the product question, not merely announce work.
- Convert competitor screenshots and references into decision dimensions. Do not list products one by one unless the comparison directly changes the solution.
- Use a compact comparison table when it sharpens judgment. Useful columns include goal, user intent, trigger moment, content source, quantity/complexity, expected user feeling, product risk, and why it fits or does not fit this phase.
- Put a `需求 list 概览` or priority table before details for larger projects. Useful columns include feature, sub-feature, priority, owner, expected launch date, whether development has started, and dependency.
- Use early visuals or demos to reduce ambiguity: `核心页面示意`, `功能 Demo 示意`, flow diagrams, or a simple end-to-end chain before exhaustive rules.
- Make phase boundaries explicit: "本期先做", "本期不做，单独起需求", "待定，后续需支持", "未来打算做什么". Explain the reason, not only the status.
- Distinguish "本期确定需要支持的能力" from "后续需要支持的能力" when the feature is part of a broader system.
- State reuse and deviation directly: what follows online behavior, what reuses existing components, what intentionally changes because this product scene is different.
- When a structural choice exists, include alternatives with pros and cons, then state why the selected plan wins under current constraints.
- In detailed requirements, be precise about entry, trigger, default state, first-time behavior, returning-user behavior, loading, empty state, error state, feedback, exit, and cross-page continuation.
- For AI features, describe both product interaction and model/capability strategy: prompt or tool invocation, memory/context, generation strategy, safety strategy, cache, latency, and cost if relevant.
- For experiments, write the tradeoff being tested, not just the metric. Typical tradeoffs: quality vs latency, depth vs completion, entry exposure vs retention, personalization vs controllability, or model quality vs cost.
- Use appendices for heavy analysis, clustering, prompt cases, and historical data. Keep the main route readable and let the appendix support the judgment.
- Keep the tone direct, calm, and practical. Favor plain product language over polished slogans.

## Rewrite Checklist

When improving a draft, check whether it has these pieces:

- The "why now" is clear, not just "we plan to add X".
- The problem is split by meaningful dimensions, not by whatever modules already exist.
- Evidence leads to a product conclusion; screenshots, data, and feedback are not just piled together.
- The selected plan is contrasted with credible alternatives or past attempts.
- The plan explains what is intentionally not done in this phase and why.
- The expected user state is named: e.g. sense of mastery, low-friction completion, deeper learning, reuse, return, trust, companionship, or retention.
- The launch rhythm, dependency, owner, and priority are visible when the project spans multiple modules or teams.
- The success/failure interpretation is clear enough that a negative experiment can stop, narrow, or redirect investment.
- Detailed requirements do not appear before the reader understands the product judgment and scope.

## Output Guidance

For a review, lead with the strongest gaps in the draft's reasoning chain, then suggest how to reshape the section.

For a rewrite, preserve the user's actual facts and constraints. Do not invent data, experiment results, competitor claims, internal OKR context, cost numbers, or launch dates. If evidence is missing, write cautious language or mark the gap as something to fill.

For a summary of Zijun's style, emphasize the repeatable thinking pattern rather than copying exact sentences from prior documents.

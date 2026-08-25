---
name: zijun-prd-style
description: Write, rewrite, or review PRD background, competitor analysis, and high-level solution framing in Zijun's judgment-driven product style.
---

# Zijun PRD Style

Use this skill when the user asks to write, revise, summarize, or review a PRD in "子隽风格", especially the sections before detailed requirements: background, product judgment, competitor analysis, scope, high-level solution, and experiment framing.

Do not treat this as a formatting template. The style is a way of thinking: turn scattered research and feature ideas into a clear judgment chain that explains why this problem is worth doing now, why this solution shape fits the product, and how the team will know whether it worked.

## Core Shape

Prefer this logical order when it fits the material:

1. Background: what changed, what prior discussion or experiment created the need to decide now, and what product context matters.
2. Competitor or reference analysis: do not list products one by one for its own sake. Abstract the comparison into 1-3 dimensions that affect the solution choice.
3. Product judgment: state what the evidence means for this product. Make the distinction crisp, such as "A and B are different needs; one product shape cannot satisfy both well."
4. Current solution choice: explain why this phase chooses one path and explicitly leaves other paths for later.
5. High-level framework: describe the user entry, core flow, feedback/consumption loop, and reuse or deviation from existing capabilities.
6. Validation: name the core hypothesis, expected effect, and what the team should conclude if the result is positive or negative.

## Writing Moves

- Start from judgment, not feature inventory. The reader should understand why the feature is necessary before seeing UI details.
- Use short, memorable judgment sentences. Examples of the form: "知识 query 不等于想学习", "给出答案只是开始", "同步学和同步练是两类需求".
- Convert competitor screenshots into product dimensions. Good dimensions include: dependent on course vs independent practice, efficient answer feedback vs guided exploration, lightweight component vs heavy page, learning intent strength, content density, and whether the feature is an entry or an after-step.
- Make phase boundaries explicit. Use phrases like "本期先做", "后续再看", "不适合本期做", and explain the reason.
- Tie design choices to user intent and product scene. Avoid saying only "竞品这么做"; say why this product's users, content, or usage moment makes the choice appropriate.
- Where useful, include a compact comparison table with columns such as goal, content source, trigger moment, quantity/complexity, expected user feeling, and product risk.
- Keep the tone direct, calm, and practical. Favor plain product language over polished slogans.

## Rewrite Checklist

When improving a draft, check whether it has these pieces:

- The "why now" is clear, not just "we plan to add X".
- The competitor analysis produces a decision dimension, not just screenshots or examples.
- The selected plan is contrasted with credible alternatives.
- The plan explains what is intentionally not done in this phase.
- The expected user state is named: e.g. sense of mastery, low-friction completion, deeper learning, reuse, return, or retention.
- The success/failure interpretation is clear enough that a negative experiment can stop or redirect investment.
- Detailed requirements do not appear before the reader understands the product judgment.

## Output Guidance

For a review, lead with the strongest gaps in the draft's reasoning, then suggest how to reshape the section.

For a rewrite, preserve the user's actual facts and constraints. Do not invent data, experiment results, competitor claims, or internal OKR context. If evidence is missing, write cautious language or mark the gap as something to fill.

For a summary of Zijun's style, emphasize the repeatable thinking pattern rather than copying exact sentences from prior documents.

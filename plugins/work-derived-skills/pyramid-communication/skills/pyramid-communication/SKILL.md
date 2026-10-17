---
name: pyramid-communication
description: Structure, critique, rewrite, or prepare Chinese business reports, proposals, plans, reviews, briefs, speeches, and presentation narratives using Pyramid Principle methods. Use when the user asks to make a document more logical, structured, concise, decision-ready, conclusion-first, MECE, audience-oriented, or suitable for leadership reporting; also use when turning scattered notes into an outline, checking argument hierarchy, improving slide headlines, or preparing a verbal update. Do not use for grammar-only polishing when no structural judgment is needed.
---

# Pyramid Communication

Turn material into a decision-first communication structure. Preserve facts, mark assumptions, and never invent evidence.

## Choose the task mode

- **Build**: Turn notes, data, or an objective into an outline or draft.
- **Restructure**: Reorganize an existing draft without changing its factual meaning.
- **Pressure-test**: Diagnose structural gaps, unsupported conclusions, overlaps, omissions, and weak logic.
- **Present**: Convert a document into a spoken update or slide storyline.

Read [references/playbook.md](references/playbook.md) for the detailed tests, templates, and examples whenever the request involves a substantive rewrite, review, or presentation storyline.

## Core workflow

1. Identify the audience, decision or response needed, and the single question the communication must answer.
2. Extract facts, judgments, recommendations, actions, assumptions, and unknowns. Keep these categories distinct.
3. Draft the top-line answer as one complete, informative sentence. Avoid labels such as “three issues” or “project update.”
4. Select the opening:
   - For decision or change: Situation - Complication - Question - Answer.
   - For routine reporting: Answer - key evidence - risk - next action.
   - For urgent communication: Answer - impact - immediate action - required decision.
5. Build the pyramid downward. Each child must directly explain or support its parent. Each parent must summarize the meaning of its children.
6. Organize siblings by exactly one dominant logic:
   - time or causal sequence;
   - structural decomposition;
   - degree, priority, or importance;
   - deductive reasoning when a rule, case, and implication form a real chain.
7. Test sibling groups for overlap and omission. Apply MECE as a diagnostic, not as decoration.
8. Replace topic labels with message sentences. State what is true, why it matters, or what should happen.
9. Put detail at the lowest useful level. Remove facts that do not support a higher-level point.
10. End with an explicit decision, owner, next step, or unresolved question when the genre requires action.

## Output contract

Lead with the improved result. Then provide only the explanation the user needs.

For a rewrite, normally return:

1. **Core conclusion** - one sentence.
2. **Recommended structure** - 2-5 mutually distinct supporting points.
3. **Rewritten draft** - in the user's requested format and tone.
4. **Open gaps** - missing evidence, assumptions, decisions, owners, or dates.
5. **Structural changes** - a short explanation only when useful.

For a review, separate:

- structural problems;
- evidence problems;
- wording problems.

Rank issues by impact on the audience's decision. Do not spend most of the response on wording when the argument itself is weak.

## Guardrails

- Do not force every document into four SCQA headings; use SCQA to design the opening, then write naturally.
- Do not confuse a list with a logical group. Name the shared meaning and verify the ordering rule.
- Do not claim MECE when categories overlap or the scope is undefined.
- Do not make a recommendation sound certain when evidence is incomplete.
- Do not bury bad news, tradeoffs, dependencies, or unresolved decisions.
- Do not over-compress material until qualifications or causality disappear.
- Preserve the user's terminology unless changing it materially improves comprehension.

## Final quality gate

Before delivering, verify:

- Can the first screen or first 30 seconds convey the answer?
- Does every section answer a likely audience question?
- Does every lower-level point support the point above it?
- Are sibling points comparable and ordered by one clear rule?
- Do headings communicate conclusions rather than topics?
- Are recommendations tied to reasons, evidence, risks, and next actions?
- Are assumptions and missing information visible?
- Can the audience tell what decision or action is required?

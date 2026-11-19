---
name: resume-story-design
description: Design, restructure, or finish a professional resume when the task requires both experience storytelling and visual delivery. Use for resume diagnosis, information hierarchy, layout redesign, print-ready PDF export, or iterative visual refinement. Do not use for a single isolated sentence rewrite or typo fix.
---

# Resume Story Design

Turn a candidate's real experience into a resume that is easy to understand, visually intentional, and ready to submit. The goal is not decoration. The finished resume must communicate positioning, evidence, and relationships quickly while remaining accurate and readable in the final PDF.

## Choose the operating mode

- **Diagnose:** identify problems in positioning, hierarchy, scan path, relationships, density, typography, alignment, and final-file usability. Do not change the artifact unless requested.
- **Restructure:** reorganize content and layout while preserving confirmed facts, scope, and relationships.
- **Deliver:** produce or update the editable source, render the resume, export the PDF, and verify the final artifact.

If the request spans modes, complete them in that order. Do not treat a local styling request as permission to rewrite content or alter the information architecture.

## Preserve intent before designing

Read the full resume and any referenced project material before making structural decisions. Build a compact content map containing:

- target role and candidate positioning;
- companies, organizations, roles, dates, and employment type;
- projects, ownership, evidence, and results;
- personal works and links;
- causal or chronological relationships between items;
- user-confirmed order, wording, and layout constraints.

Treat confirmed facts, project ownership, chronology, and explicit relationships as invariants. When the user asks for layout-only changes, keep the wording and structure unchanged unless a change is necessary to prevent an actual layout failure; disclose such a case before changing content.

When content and layout are both in motion, stabilize them in this order:

1. factual accuracy and positioning;
2. project relationships and ordering;
3. information hierarchy and scan path;
4. grid, density, typography, and color;
5. final PDF behavior.

## Design around the reader's task

The first scan should answer:

1. Who is this candidate?
2. What role are they targeting?
3. Which organizations and projects are most important?
4. What did they discover, decide, build, or improve?
5. What evidence supports the claims?

Use layout to express meaning. A timeline should encode chronology or continuation, not serve as decoration. Spatial alignment may show that a personal project extends an earlier work experience, but the relationship must also remain understandable in text.

Select emphasis deliberately:

- emphasize the candidate's positioning, major organizations, representative projects, and evidence;
- keep departments, employment type, and dates available but secondary unless they materially change the story;
- use color for anchors, links, and relationships rather than coloring every level;
- keep base text colors consistent and create hierarchy mainly through size, weight, spacing, and position.

For detailed visual and editorial criteria, read [references/design-criteria.md](references/design-criteria.md).

## Build the layout from the page inward

Start with the final medium and reading conditions. For a one-page resume, establish the A4 page boundary, margins, column widths, baseline spacing, and minimum readable type before styling individual items.

Prefer one coherent grid. Align section titles, company nodes, project titles, body text, and supporting metadata to a small set of shared axes. Avoid fixing local misalignment with isolated offsets when the underlying grid or ownership is wrong.

Balance density across the whole page. When one area is too empty or crowded, first adjust structural spacing, column allocation, or content grouping. Do not insert fixed blank regions merely to force one cross-column alignment; they create downstream gaps when copy length changes.

Keep the visual direction appropriate to the role and evidence. Do not impose one universal template. A restrained product resume may use dark text, one accent color, a clear timeline, and limited pale backgrounds; a design role may justify more expressive typography or composition.

## Iterate without losing the system

Before each revision, identify whether the request changes content, structure, style, or final-output behavior. Touch only the necessary layer.

After each material revision, recheck:

- confirmed order and relationships;
- shared left edges and baselines;
- consistent spacing between repeated patterns;
- whether emphasis still reflects the reader's priorities;
- whether the change created a new blank gap, overflow, collision, or bottom crowding.

When a user points to a screenshot, interpret the marked geometry and the accompanying words together. A red box is evidence of the target area, not an instruction by itself.

## Render and verify the real artifact

Do not declare completion from source code or browser appearance alone. Inspect the rendered resume at the final page size.

For PDF delivery, read and follow [references/delivery-checklist.md](references/delivery-checklist.md). Completion requires an editable source when applicable, a final PDF, and evidence that the PDF itself was checked.

## Completion standard

A resume is complete only when:

- factual content and relationships match the user's confirmed intent;
- the first scan reveals positioning, major experience, representative projects, and evidence;
- typography, alignment, spacing, and color form one coherent system;
- text is readable at ordinary PDF viewing size;
- the page has no accidental dead zones, clipping, overflow, or bottom compression;
- links and page count are verified in the exported file;
- any unresolved limitation, such as a local-only media link, is stated clearly.


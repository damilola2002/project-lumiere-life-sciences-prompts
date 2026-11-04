# Prompt Checker lessons (Agri-Food & Environmental Micro task, cyanobacteria A/C)

Rules learned from Prompt Checker flags on this task. Apply to every future Lumiere prompt before first submission.

| # | Flag received | Cause | Rule going forward |
|---|---|---|---|
| 1 | MULTIPLE_CHOICE_EXPLICIT | "which of the two taxa" — answer was a pick between two panels | Never ask the solver to choose between the supplied panels/images. The final answer must be a value with an open answer space (number, ratio, list), and the choice of panel must be an internal reasoning step only. |
| 2 | WORDING_AMBIGUITY ("typical cell") | "typical", "representative" have no objective rule | Never say "typical/representative cell". Name ONE reference object per panel with a unique positional or rank rule. |
| 3 | READING_RULE_MISSING | No rule for how to measure against the scale bar | Always state: what is measured (outer edge to outer edge, halo excluded), which part of the scale bar counts (blue part, outline excluded), and a rounding step (e.g. nearest 0.5 um) so every careful reader gets the same number. |
| 4 | DOMAIN_KNOWLEDGE_FLOOR | Pure geometry (SA:V of spheres) — works with neutral labels | A biological identification or principle must decide the answer (e.g. recognising the microcystin-producing genus from morphology). Test: replace organisms with "spheres"; if still solvable, redesign. |
| 5 | STACKED_QUESTIONS | "Identify that taxon ... and calculate ..." | One question, one final answer. Do not ask the solver to name/identify anything that is not the final answer. |
| 6 | NON_FOUNDATIONAL_REFERENCE | "the taxon of greatest concern to the monitoring programme" | Never rely on a programme-, lab- or region-specific rule. Use textbook facts only. |
| 7 | WORDING_AMBIGUITY ("concern", "most commonly") | Undefined or unscoped criteria | Use definitional anchors with only one possible reading (e.g. "the genus after which the microcystins are named"), not frequency/importance claims. |
| 8 | WORDING_AMBIGUITY (taxonomic rank) | "Identify that taxon" — genus or species? | If a name is ever required, state the rank and format. Better: avoid needing a name at all. |
| 9 | WORDING_AMBIGUITY (reference cell not unique) | "solitary cell in the lower-right ... above and left of the scale bar" matched several cells | Locate the reference object with a rank rule inside a defined region (e.g. "the lowest cell whose centre lies within the right-hand quarter of the image width") and verify on the full-resolution image that exactly one object satisfies it before submitting. |

## Pre-submission self-check (run on every prompt)
1. Final answer is a single value; no choosing among supplied panels/images.
2. No "typical", "representative", "most common", "greatest concern", or other unscoped words.
3. Every measured object is uniquely specified by a rank/region rule, verified on the image.
4. Measurement rule + scale-bar rule + rounding rule stated.
5. Neutral-label test fails (biology is required).
6. Only one question; nothing to name unless it is the answer.
7. Only foundational, textbook criteria.
8. KaTeX for units/maths, example value is not a real option, under 2,000 characters.

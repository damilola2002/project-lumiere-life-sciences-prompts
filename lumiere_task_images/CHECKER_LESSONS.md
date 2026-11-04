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

## Self-caught error (guideline reread, §6.1 single canonical answer)
| 10 | (caught before checker) | "Widest distance" on a slightly oval cell gave 9.0-9.6 um depending on edge reading, so the 0.5-um rounding could land on 9.0 or 9.5; earlier GTFA 32 assumed 8.5 um and was wrong | Before fixing a GTFA, measure the object objectively at full resolution (several edge thresholds) and confirm the rounded value never changes. For near-spherical cells use the mean of longest and shortest widths (equivalent diameter) and round to a bin wide enough that every threshold gives the same value. |
| 11 | Model Failure Checker FAILURE_BAR_NOT_MET (both responses) | Both models identified the genus correctly and failed only by mis-measuring cell size against the scale bar; checker judged this a measurement error, not a biological misinterpretation | Put the trap in a biological reading of the image (which cells are which type), not in a pure size measurement. A measurement error alone is treated like a perceptual miss. |
| 12 | (self-caught) | Measured Panel A cell (~9 um) was at/above the normal size range for Microcystis aeruginosa, so the models' "textbook" 4.5 um could be defended by a reviewer | Before using a scale bar as ground truth, check the measured size is biologically plausible for the organism; if not, do not build the answer on it. |
| 13 | (self-caught) | Printed asterisk in source Panel D marks one heterocyst (teaches the solver what to look for) | Crop out printed markers that identify a target class (domain-knowledge floor), keeping scale bars and panel letters. |
| 11 | FAILURE_BAR_NOT_MET (Model Failure + Justification checker, twice) | Both models identified the taxon correctly and failed only by mis-measuring a cell against the scale bar; checker ruled this "too far upstream", not a biological misinterpretation, despite §6.2 listing scale interpretation | A pure measurement/estimation error is NOT accepted as a failure. The image misreading must itself be a biological misinterpretation (wrong cell type, wrong structure, wrong taxon, artifact read as signal). Design traps where the visual error and the biological error are the same step. |
| 12 | (self-caught, late) | Measured Microcystis cell (~9 um) sits above the textbook size range, so the models' prior (4.5 um) looked biologically right | Before relying on a published scale bar, check that every measured size is biologically plausible for the named organism; if not, choose another image. |

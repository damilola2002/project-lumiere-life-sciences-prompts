# 59 — Raw Ni-NTA purification gel: imidazole gap between minor and main elution peaks

**Assay type:** Gel Electrophoresis & Western Blots — SDS-PAGE protein gel
**Subdomain:** Biochemistry

## Source and license (form fields)
- **Image:** `task_images/59_emtpx_gel_image1.jpg` (Image 1)
- **Source URL / DOI:** https://doi.org/10.1371/journal.pntd.0014755
- **License type:** CC BY 4.0
- **Reference material (title):** Conserved surface-exposed linear epitopes of Echinococcus multilocularis thioredoxin peroxidase enable non-invasive diagnosis of alveolar echinococcosis in intermediate host
- **Where published:** PLOS Neglected Tropical Diseases, Volume 20, Issue 9, e0014755, 2026
- **License of reference material (verbatim):** "This is an open access article distributed under the terms of the Creative Commons Attribution License, which permits unrestricted use, distribution, and reproduction in any medium, provided the original author and source are credited."
- **Image handling:** the original, uncropped raw gel photograph for Fig 2C. It was extracted at native resolution (808 × 472 px JPEG) from the article's supplementary file "S1 Raw Gel" (pntd.0014755.s003.pdf, page 1, panel C). Lane numbers and marker sizes are the authors' own labels on the raw image. No other edits.
- **Answer not in the publication:** the paper states only that purity was enhanced at 300, 400 and 500 mM. It never mentions the minor 60 mM elution peak, and gives no difference between peaks.

## Prompt
Image 1 is the raw, uncropped Coomassie-stained SDS-PAGE gel from a Ni-NTA purification of an N-terminally His-tagged recombinant protein (expected band ≈ 25 kDa) expressed in *E. coli*. Lane assignments:
- M: protein marker (sizes in kDa at left);
- 1: column flow-through;
- 2: induced whole-cell lysate;
- 3: soluble supernatant;
- 4: insoluble pellet;
- 5–13: fractions eluted stepwise with 20, 40, 60, 80, 100, 200, 300, 400 and 500 mM imidazole, respectively.

Considering only the elution fractions (lanes 5–13), define:
- the **main elution peak** as the consecutive fractions in which the ≈25 kDa band is markedly stronger than in every earlier elution fraction;
- a **minor elution peak** as a single earlier fraction whose ≈25 kDa band is clearly stronger than in both of its neighbouring elution fractions.

How many mM higher is the imidazole concentration of the first fraction of the main elution peak than that of the minor elution peak?

End your response with a final line in exactly this format:
Final answer: <integer> mM

**Answer format:** Integer (mM)

## GTFA
240

## Step-by-step solution
Step 1: Map lanes to imidazole. Lanes 5–13 correspond to 20, 40, 60, 80, 100, 200, 300, 400 and 500 mM. The steps are 20 mM up to lane 9 (100 mM), then 100 mM, so lane 10 is 200 mM and lane 11 is 300 mM.

Step 2: Read the ≈25 kDa band (level with the marker's 25 kDa band) across lanes 5–13:
- lanes 5, 6, 8, 9: faint;
- lane 7: a distinct moderate band;
- lane 10: a moderate band;
- lanes 11, 12, 13: very thick, intense bands, far darker than any earlier elution lane.

Densitometry of the raw image, in background-subtracted relative units, confirms this: lane 5 ≈ 20, lane 6 ≈ 14, lane 7 ≈ 42, lane 8 ≈ 19, lane 9 ≈ 25, lane 10 ≈ 49, lane 11 ≈ 113, lane 12 ≈ 115, lane 13 ≈ 123.

Step 3: Identify the main elution peak. Lanes 11–13 are each more than twice as intense as any earlier elution lane. Lane 10 (≈49) is not markedly stronger than lane 7 (≈42), so it is not part of the main peak. The first fraction of the main peak is lane 11, which is 300 mM.

Step 4: Identify the minor elution peak. Lane 7 (≈42) is clearly stronger than both neighbours, lane 6 (≈14) and lane 8 (≈19). No other earlier lane qualifies:
- lane 9 is weaker than lane 10;
- lane 10 is weaker than lane 11;
- lane 6 is weaker than lane 5.

The minor peak is therefore lane 7, which is 60 mM.

Step 5: Interpret the biology. A small fraction of the His-tagged protein elutes at low imidazole (60 mM), consistent with a weakly bound subpopulation (for example, a partly buried or partly accessible His-tag). Most of it needs ≥300 mM imidazole to compete it off the Ni²⁺ resin.

Step 6: Difference: 300 − 60 = 240 mM.

Final Answer: 240

## Image description (≈330 words)
Modality: a colour photograph of a single Coomassie Brilliant Blue-stained polyacrylamide gel on a white light box. It is a raw, uncropped capture with the gel edges and a ragged top edge visible.

Layout: lane labels are printed across the top: "M 1 2 3 4 5 6 7 8 9 10 11 12 13 M". Molecular-weight labels are printed down the left side: 180, 130, 100, 72, 55, 43, 33, 25, 17. The two outer lanes (M) show ladders of evenly spaced sharp bands, with one reddish band near the 72 label.

Content by lane, top to bottom:
- **Lanes 1–3:** very heavily loaded, with dense, overlapping dark-blue bands from top to bottom. Lanes 2 and 3 have a very thick, dark band level with the 25 marker band.
- **Lane 4:** fewer bands, including a doublet near 33 and a thick dark band at 25.
- **Lanes 5 and 6:** faint smeared bands in the 43–100 region. At the 25 level, lane 5 has a faint band and lane 6 has a barely visible, very faint band.
- **Lane 7:** a distinct, moderately stained band at the 25 level that stands out from lanes 6 and 8.
- **Lanes 8 and 9:** faint bands at the 25 level.
- **Lane 10:** a moderately stained band at the 25 level.
- **Lanes 11, 12 and 13:** very thick, intensely stained bands at the 25 level, much darker than any band in lanes 5–10. Only faint diffuse staining appears elsewhere in these lanes.
- **Lanes 7–13:** faint diffuse smears in the 55–72 region.

Quality: the background is uneven blue, darker on the left where lanes are overloaded. Bands curve slightly upward toward the edges, and the gel top is irregular. The focus is adequate, and the photo has slight glare at the top.

Artifacts: overloading smears in lanes 1–3, the ragged gel top, uneven background, and a dark dye front along the bottom edge.

Annotations: only the authors' lane numbers and marker size labels; no arrows or boxes.

## Distractors
Distractors (incorrect answers only). Note that in testing we provided the model all potential answers, including the GTFA.
1. **80**: assumes uniform 20 mM steps, so lane 11 is read as 140 mM (140 − 60).
2. **140**: includes lane 10 (200 mM) in the main peak (200 − 60).
3. **280**: takes lane 5 (20 mM) as the minor peak (300 − 20).
4. **260**: takes lane 6 (40 mM) as the minor peak (300 − 40).
5. **200**: takes lane 9 (100 mM) as the minor peak (300 − 100).

## Target failure mode
- **Label–element mis-binding:** the non-uniform lane-to-concentration mapping.
- **Signal discrimination:** a faint versus a moderate band on an uneven, overloaded raw gel, used to locate a small early peak and the true start of the main peak.

**Error types:**
- Label–element mis-binding.
- Data extraction error.

## References
- Zheng et al. (2026) PLOS Negl Trop Dis 20(9): e0014755. Fig 2C and S1 Raw Gel.
- Ni-NTA imidazole step elution principles: e.g. QIAGEN, *The QIAexpressionist* handbook, chapter on purification under native conditions (imidazole competition for His-tag binding).

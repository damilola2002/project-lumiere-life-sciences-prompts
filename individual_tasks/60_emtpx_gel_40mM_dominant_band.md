# 60 — Raw Ni-NTA gel: apparent MW of the dominant band in the 40 mM imidazole fraction (replaces 59)

**Assay type:** Gel Electrophoresis & Western Blots — SDS-PAGE
**Subdomain:** Biochemistry

## Source and license (unchanged from task 59)
- **Image:** `task_images/59_emtpx_gel_image1.jpg` (Image 1) — the same raw gel.
- **DOI:** https://doi.org/10.1371/journal.pntd.0014755 · **License:** CC BY 4.0
- **Title:** Conserved surface-exposed linear epitopes of Echinococcus multilocularis thioredoxin peroxidase enable non-invasive diagnosis of alveolar echinococcosis in intermediate host
- **Where published:** PLOS Neglected Tropical Diseases, Volume 20, Issue 9, e0014755, 2026
- **Answer not in the publication:** the paper mentions only the ~25 kDa EmTPx band. It never mentions any ~72–75 kDa contaminant, or the 40 mM fraction specifically.

## Prompt
Image 1 is the raw, uncropped Coomassie-stained SDS-PAGE gel from a native Ni-NTA purification of recombinant His-tagged EmTPx, a 193-residue Echinococcus multilocularis protein expressed in E. coli from pET-28a. Lane M is the protein marker (sizes in kDa printed at left; the same marker is loaded in both outer lanes). Lane 1 is the column flow-through; lanes 2–4 are the induced whole-cell lysate, soluble supernatant and insoluble pellet. Lanes 5–13 are the elution fractions, loaded in order of increasing imidazole: the step elution began at 20 mM and rose in four further 20-mM increments, then continued in 100-mM increments up to 500 mM.

In the fraction eluted with 40 mM imidazole, what is the apparent molecular weight of the most intensely stained band in that lane? Estimate it by interpolating against the marker bands, assuming log₁₀(MW) varies linearly with migration distance between adjacent marker bands. Because the gel runs unevenly, use the marker positions interpolated between the two outer marker lanes at the position of that lane.

End your response with a final line in exactly this format:
Final answer: <integer> kDa

**Answer format:** Integer (kDa), tolerance ±5 kDa (accept 70–80)

## GTFA
75

## Step-by-step solution
Step 1: Map the elution lanes. The steps are 20, 40, 60, 80 and 100 mM, then 200, 300, 400 and 500 mM, in lanes 5–13. So the 40 mM fraction is lane 6, the second elution lane.

Step 2: Identify EmTPx. 193 residues plus the ~20-residue pET-28a leader is about 213 aa × 110 Da ≈ 23 kDa, which runs near the 25 kDa marker. That band dominates lanes 11–13 and is strong in the induced lysate.

Step 3: Inspect lane 6. The EmTPx band at the 25 kDa level is only very faint. The most intensely stained band in lane 6 is a sharper band high in the lane, at about the level of the reddish (72 kDa) marker band. Fainter bands lie just below it (about 55–60 kDa) and near 43 kDa. Densitometry of the raw image (background-subtracted relative units): upper band ≈ 42, next band ≈ 26, EmTPx band ≈ 23. So the strongest band in this imidazole eluate is not the His-tagged target but a co-eluting E. coli contaminant.

Step 4: Correct for uneven running. The gel image is 808 px wide.
- In the left marker lane (x ≈ 97 px), the 100 and 72 kDa bands are at y ≈ 173 and 200 px.
- In the right marker lane (x ≈ 745 px), they are at y ≈ 182 and 209 px.
- At lane 6 (x ≈ 383 px), 44% of the way across, the interpolated positions are y ≈ 177 px for 100 kDa and y ≈ 204 px for 72 kDa.
- The lane 6 band is at y ≈ 201 px.

Step 5: Semi-log interpolation between 100 and 72 kDa:
- fraction of the distance from the 72 kDa band toward the 100 kDa band = (204 − 201)/(204 − 177) ≈ 0.11;
- log₁₀MW = log₁₀72 + 0.11 × (log₁₀100 − log₁₀72) = 1.857 + 0.11 × 0.143 ≈ 1.873;
- MW ≈ 74.7 kDa.

Step 6: Rounded, the apparent MW is about 75 kDa. That fits a common ~70–75 kDa E. coli co-purifying contaminant in Ni-NTA preparations, such as a chaperone or ArnA-type protein.

Final Answer: 75

## Image description (≈300 words)
Modality: a colour photograph of one Coomassie-stained polyacrylamide gel on a white light box. It is a raw, uncropped capture with a ragged top edge.

Layout: lane labels across the top read "M 1 2 3 4 5 6 7 8 9 10 11 12 13 M". Size labels at left read 180, 130, 100, 72, 55, 43, 33, 25, 17. Both outer M lanes show a ladder of sharp bands, including one reddish band level with the "72" label. The ladder bands sit slightly lower on the right side than on the left, so the gel ran a little unevenly across its width.

Lanes:
- **Lanes 1–3:** very heavily loaded, with dense overlapping bands throughout and a thick dark band at the 25 level in lanes 2 and 3.
- **Lane 4:** a thick band at 25 and a doublet just below the 33 level.
- **Lane 5:** several faint bands, at about the 72 level, between 55 and 43, and at 25.
- **Lane 6:** a distinct, relatively sharp band high in the lane at about the level of the reddish marker band; fainter bands below it near 55–60 and 43; only a very faint band at the 25 level.
- **Lane 7:** a distinct band at 25, with faint smears above.
- **Lanes 8 and 9:** faint bands at 25 and faint smears around 55–72.
- **Lane 10:** a moderate band at 25.
- **Lanes 11–13:** very thick, intense bands at 25, with faint diffuse staining above.

Quality: the blue background is uneven, darker on the left. Focus is adequate, with slight glare at the top.

Artifacts: overloading smears, the irregular gel top, and a dye front along the bottom.

Annotations: only the authors' lane numbers and size labels.

## Distractors
Distractors (incorrect answers only). Note that in testing we provided the model all potential answers, including the GTFA.
1. **25**: assumes the strongest band in an imidazole eluate is the His-tagged target.
2. **58**: picks the second, fainter band just below (≈55–60 kDa).
3. **43**: picks the lower contaminant band near 43 kDa.
4. **100**: maps 40 mM to the wrong lane, or misaligns the ladder labels by one band.
5. **33**: reads lane 4's doublet (mis-maps 40 mM to the pellet lane).

## Target failure mode
Signal-vs-expectation and protocol-knowledge override (golden-example pattern):
- the naive assumption that the eluate's dominant band is the target;
- lane mapping under non-uniform elution steps;
- a faint, smeared lane;
- ladder interpolation on an unevenly run raw gel.

**Error types:**
- Data extraction error.
- Figure-based quantitative estimation error.
- Label–element mis-binding.

## References
- Zheng et al. (2026) PLOS Negl Trop Dis 20(9): e0014755, Fig 2C / S1 Raw Gel.
- Semi-log MW estimation by SDS-PAGE: Weber & Osborn (1969) J Biol Chem 244:4406–4412.
- Common E. coli Ni-NTA contaminants (e.g. ArnA ~74 kDa, DnaK ~69 kDa): Robichon et al. (2011) Appl Environ Microbiol 77:4634–4646.

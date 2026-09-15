# Molecular imaging, gels, and blots

## 21. Western-blot band assignment
**Image brief:** Immunoblot with molecular-weight ladder, control and treated lanes, target band, lower nonspecific band, slight lane curvature, and one overloaded lane.

**Prompt:** Using the molecular-weight ladder and the target band’s alignment across lanes, which band should be quantified as the intended target: the upper band near the expected molecular mass or the lower invariant band?

**Hardening target:** Prevents nearest-dark-band selection when lanes smile.

## 22. Loading-control validity
**Image brief:** Western blot with target and loading-control panels from the same samples; one lane has visibly reduced loading-control intensity and a transfer bubble.

**Prompt:** Which lane should be excluded from target normalization because its loading-control signal is compromised by a visible transfer defect?

**Hardening target:** Identifies the defect rather than inferring expression from intensity alone.

## 23. Agarose gel plasmid topology
**Image brief:** Agarose gel with a plasmid sample showing three bands, linearized control, ladder, and faint primer-dimer region.

**Prompt:** Relative to the linearized control, which plasmid form migrates farthest in the gel: open circular, linear, or supercoiled?

**Hardening target:** Uses migration pattern rather than band brightness.

## 24. qPCR amplification curve quality
**Image brief:** Amplification plot with multiple sigmoidal traces, one late shallow nonspecific curve, threshold line, and no-template control trace.

**Prompt:** Which sample trace should be classified as a failed amplification for quantitative interpretation because it does not show a clear exponential phase crossing the threshold before the late-cycle noise region?

**Hardening target:** Separates true low template from baseline drift.

## 25. Spatial transcriptomics spot choice
**Image brief:** Tissue H&E image overlaid with spatial-capture spots and a gene-expression heatmap; include tissue folds and a necrotic zone.

**Prompt:** Which histologic compartment corresponds to the cluster of high-expression spots for the gene shown: viable tumour, necrotic debris, or adjacent stroma?

**Hardening target:** Maps spots to tissue rather than brightest heatmap color.

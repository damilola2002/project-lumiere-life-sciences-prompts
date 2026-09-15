# Cell culture and phenotypic assays

## 31. Confluence estimation
**Image brief:** Phase-contrast adherent-cell culture with uneven illumination, a scratch-free monolayer, detached rounded cells, and a meniscus-darkened edge.

**Prompt:** Estimate the adherent-cell confluence in the central, evenly illuminated field to the nearest 10%, excluding detached rounded cells and the dish edge.

**Hardening target:** Requires area coverage, not raw object count.

## 32. Mycoplasma-like contamination
**Image brief:** DNA-fluorescence culture image showing normal nuclei plus numerous fine extranuclear puncta, with a positive and clean control panel.

**Prompt:** Which panel displays the extranuclear punctate DNA pattern most consistent with mycoplasma contamination?

**Hardening target:** Separates sparse puncta from camera noise and apoptotic fragments.

## 33. Scratch-wound closure
**Image brief:** Time-zero and endpoint phase-contrast images of the same wound, with unequal image widths, debris, and a scale bar in both panels.

**Prompt:** Using the scale bars rather than pixel width, what percentage of the initial wound width remains at the endpoint, rounded to the nearest whole percent?

**Hardening target:** Tests cross-panel scale calibration.

## 34. Organoid viability pattern
**Image brief:** Brightfield organoid field with compact smooth organoids, cystic organoids, dark collapsed structures, and extracellular debris.

**Prompt:** Which visible morphology is most consistent with loss of organoid viability: a smooth dense boundary, a translucent lumen, or a dark collapsed irregular structure?

**Hardening target:** Requires morphology recognition amid variable focus.

## 35. Transwell migration
**Image brief:** Crystal-violet stained underside of a transwell membrane with migrated cells, membrane pores, stain precipitate, and an edge ring.

**Prompt:** For quantifying migration, which region should be excluded because it is a membrane-edge artifact rather than representative migrated cells?

**Hardening target:** Prevents edge-ring staining from being counted as cells.

# Fluorescence and confocal microscopy

## 16. Colocalization versus bleed-through
**Image brief:** Two-channel confocal cell image with punctate green lysosomes, red cargo, a merged panel, a bright saturated region, and channel-specific scale bars.

**Prompt:** In the unsaturated cells, does the red cargo show punctate colocalization with the green lysosomal signal, diffuse separation, or only apparent overlap confined to saturated pixels?

**Hardening target:** Tests merged-image overreliance and saturation awareness.

## 17. Nuclear translocation
**Image brief:** Three-panel fluorescence image: DAPI, transcription-factor channel, merge. Include cytoplasmic background and a few dead cells with nonspecific bright signal.

**Prompt:** In viable cells with intact DAPI nuclei, is the transcription-factor signal predominantly nuclear or cytoplasmic?

**Hardening target:** Requires restricting inference to intact cells and comparing channels.

## 18. Z-stack plane identification
**Image brief:** Three numbered confocal z-planes of a spheroid with surface fluorescence, central optical haze, and a scale bar.

**Prompt:** Which numbered z-plane passes closest to the spheroid equator, as indicated by the largest continuous cross-sectional profile?

**Hardening target:** Converts 3D geometry into an image-dependent choice.

## 19. Photobleaching curve
**Image brief:** Time-series fluorescence plot with two traces, a nonzero baseline, uneven time ticks, and a transient acquisition spike.

**Prompt:** For the trace that begins at the higher intensity, what fraction of its pre-bleach intensity remains at the final recorded time, rounded to two significant figures?

**Hardening target:** Requires correct trace binding, baseline reading, and scale interpretation.

## 20. Dead-cell dye interpretation
**Image brief:** Live/dead fluorescence field with calcein-positive viable cells, membrane-impermeant dye-positive nuclei, autofluorescent debris, and overlapping cells.

**Prompt:** Which population is specifically identified by the membrane-impermeant nuclear dye: cells with lost plasma-membrane integrity or all metabolically active cells?

**Hardening target:** Separates fluorescent debris from true nuclear positivity.

# 51 — AAVS1 transgene variegation (flow cytometry)

**Supertype / subtype:** Molecular imaging → flow-cytometry histogram (fluorescence-reporter distribution). *Not* a bar chart, not a dot plot.

**Image gate:** One panel of overlaid flow-cytometry histograms — reporter fluorescence on the x-axis (log), cell count (normalised) on the y-axis. Several single-cell-derived hiPSC clones targeted at the same genomic safe-harbour locus are drawn as open traces; the untargeted parental line is the shaded trace; a single vertical gate marks the positive threshold. At least one clone must be unambiguously **bimodal** (a sub-peak right of the gate *and* a sub-peak overlapping the shaded parental trace), alongside clones that are uniformly right-shifted, uniformly overlapping the control, and unimodal-but-dim. Clones must be labelled. Keep axis labels, the gate marker, and the shaded control. No dark-mode screenshot, no WebP.

**Prompt:**
> The open traces each show reporter-fluorescence distribution for one single-cell-derived pluripotent clone carrying the same targeted reporter cassette; the shaded trace is the untargeted parental line and the vertical line is the positive gate. Every clone is genetically identical at the integration site, so a single uniform behaviour is expected per clone. For the labelled clones, name the reporter-fluorescence distribution shape that, on its own, demonstrates the integrated cassette is in a mixed transcriptional state across cells of one clone rather than uniformly active or uniformly off. Answer with the distribution descriptor (example format: "left-skewed unimodal").

**GTFA:** Bimodal distribution
**GTFA format:** Text, case-insensitive. Accept "bimodal" / "bimodal distribution".

**Image description (author to complete, ≥200 words):** Modality = overlaid flow-cytometry histograms. Describe, do not interpret: axis titles and scales (log x fluorescence, normalised count y), the shaded parental trace position relative to the gate, each open trace's label and where its peak(s) fall relative to the gate and to the shaded trace, peak heights/widths, and the exact position of the gate line. Record which trace has two separated modes and the approximate fraction under each mode, without using the words "silencing", "variegation", or stating the answer. Note any trace that touches the panel edge (flag-prone). Give enough that a reader could answer from the text alone.

**Golden solution:**
Step 1: Read the x-axis as reporter fluorescence (log) and locate the gate line and the shaded parental trace. Step 2: For each open trace, record its mode structure relative to the gate — single mode above, single mode overlapping control, or two separated modes. Step 3: A genetically clonal population in one uniform transcriptional state gives a single mode; two separated modes (one above the gate, one overlapping the parental control) mean the same cassette is active in some cells and off in others — intra-clonal variegated silencing, the safe-harbour failure. **Final answer: Bimodal distribution.**

**Distractors (incorrect answers only). Note that in testing we provided the model all potential answers, including the GTFA.**
- Uniform right-shifted peak — chose the clone with the highest positive fraction and called full expression the "mixed" state.
- Overlapping the parental control — read the mixed clone's negative sub-peak only and called it silenced/off.
- Right-shifted with increased MFI — graded by brightness (mean fluorescence) instead of mode structure.
- Broad unimodal peak — mistook a single wide peak for two populations.
- Narrow unimodal below gate — picked a dim unimodal clone as the heterogeneous one.

**Failure target (image-interpretation error, Data extraction / Label–element binding):** The model reads the bimodal clone's upper sub-peak, sees it clears the gate, and reports the clone as "positive / uniformly expressing," ignoring the sub-population that overlaps the parental control — missing that one clonal population carries both active and silenced cassettes.

**Source fields:**
- Title: *Variable expression and silencing of CRISPR-Cas9 targeted transgenes identifies the AAVS1 locus as not an entirely safe harbour*
- Authors: Bhagwan JR, Collins E, Mosqueira D, et al.
- Where published: *F1000Research* 2019, **8**:1911 (peer-reviewed; indexed version dated 2020). PMC7401084.
- Licence: Creative Commons Attribution 4.0 (CC BY 4.0) — paste the exact licence string from the article/figure page into the form.
- References the solution relies on: the clone-to-clone reporter-expression figure (variable % positive across single-cell clones) and the differentiation time-course showing loss of expression. Confirm the chosen figure's panel and that the bimodality/percentages are shown graphically, not stated numerically in the text for the asked clone.

**Remaining human-in-the-loop steps before submission (cannot be done in this drafting session):**
1. Download the actual figure from the F1000Research article page, confirm CC BY 4.0 in the caption, export PNG/JPEG under 5 MB at ~2000 px, crop to the histogram panel keeping axes/gate/labels, and deliver inside a zip.
2. Verify the GTFA against the real panel and that the answer is not stated in the paper text for the asked clone.
3. Run the two responder models; require 2/2 failure. Then write the one-sentence failure justification quoting each model's exact wrong answer vs the GTFA. Do not submit if either model answers correctly.

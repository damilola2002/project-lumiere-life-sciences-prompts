# 55 — Failed Ziehl–Neelsen smear: which reagent failed?

**Supertype / subtype:** Microbiology — Gram and other microbial stains (acid-fast stain)
**Subdomain:** Microbiology

## Source and license (form fields)
- **Image:** `task_images/55_zn_image1.png` (Image 1)
- **Source URL / DOI:** https://doi.org/10.3390/life14111418
- **License type:** CC BY 4.0
- **Reference material (title):** AI-Based Analysis of Ziehl–Neelsen-Stained Sputum Smears for Mycobacterium tuberculosis as a Screening Method for Active Tuberculosis
- **Where published:** Life (MDPI), Volume 14, Issue 11, Article 1418, 2024
- **License of reference material (verbatim):** "Licensee MDPI, Basel, Switzerland. This article is an open access article distributed under the terms and conditions of the Creative Commons Attribution (CC BY) license (https://creativecommons.org/licenses/by/4.0/)."
- **Image handling:** Figure 2 was downloaded at original size (2853 × 3372 px) from mdpi-res.com. Panel F only was cropped, inside its border, which excludes the panel letter. Final size 1316 × 1016 px, PNG. No other edits.
- **Answer not in the publication:** the caption calls panel F only a "staining defect; epithelial cells are pink, and large pink precipitates are present". The paper never mentions decolorization, acid-alcohol, sulfuric acid or any cause of the defect.

## Prompt
Image 1 is a Ziehl–Neelsen-stained sputum smear photographed at $400\times$. Before any acid-fast bacilli result is reported, the technical quality of the stain must be checked.

Judging from the colour of the squamous epithelial cells in this smear, which reagent of the Ziehl–Neelsen procedure failed to do its job? Give the reagent's functional role in the procedure (what it is used for), not its chemical name and not the name of the defect.

End your response with a final line in exactly this format:
Final answer: <functional role of the reagent>

**Answer format:** Text (case insensitive)

## GTFA
Decolorizer

## Step-by-step solution
Step 1: Observe Image 1. Large, flat, polygonal cells with small nuclei are visible at the upper left, upper centre, centre left and lower right. Their cytoplasm is pink to magenta. Many smaller cells with dark blue-purple, lobed or rounded nuclei, and blue fibrillar material, occupy the rest of the field.

Step 2: Recall what a correct Ziehl–Neelsen result looks like:
- Carbol fuchsin (the primary stain, driven in by heat) stains everything red.
- The decolorizer (acid-alcohol or dilute sulfuric acid) then removes the fuchsin from everything except acid-fast organisms.
- Methylene blue (the counterstain) then colours the decolorized background, cells and non-acid-fast material blue.
- In a valid smear, host cells are therefore blue, and only acid-fast bacilli are red.

Step 3: Interpret the pink epithelial cells. Host squamous cells are not acid-fast, so they should have lost the fuchsin and taken up the blue counterstain. Their pink colour shows that red fuchsin was retained in non-acid-fast material.

Step 4: Rule out the other reagents:
- The counterstain clearly worked: nuclei and fibrillar material are blue.
- A counterstain failure would leave decolorized cells pale or colourless, not pink.
- The primary stain obviously penetrated.
- Retention of fuchsin by non-acid-fast cells is the defining sign of inadequate decolorization: too short, too weak, or an exhausted decolorizing reagent.

Step 5: The reagent that failed is the decolorizer.

Final Answer: Decolorizer

## Image description (≈300 words)
Modality: a brightfield light micrograph of a stained sputum smear at moderate magnification (400×). It is a single rectangular field, slightly wider than tall, with no panel divisions.

Content: the background is pale white with a fine, lacy network of thin blue-violet threads and small granules spread across the whole field. Several large, flat, irregular polygonal cells, each many times wider than the surrounding small cells, sit in the field:
- one at the upper left;
- one at the upper centre;
- an elongated one running obliquely through the left-centre;
- one at the lower right, extending to the bottom edge.

These large cells have pink to magenta, slightly mottled cytoplasm and a small, round, darker nucleus. Scattered throughout, most densely in the centre, lower centre and lower right, are many small cells with compact, dark blue-purple nuclei. The nuclei are rounded, bean-shaped or lobed, and some lie in short clusters. A few slender, dark blue, curved strands cross the upper right quadrant. A small brownish granular patch lies in the centre-left large cell, and faint brownish granular material lies near the lower centre.

Colour summary: two colours dominate. Pink-magenta is confined to the cytoplasm of the large flat cells. Blue-violet covers the small-cell nuclei, threads and background granules.

Quality: focus is moderate and slightly soft throughout, with some loss of fine detail. Illumination is even. Individual small rod-shaped red bodies cannot be identified in the field.

Artifacts: overlapping cells, fibrillar mucus strands, brownish granular deposits.

Annotations: there are no arrows, labels, scale bar, numbers or captions in the image.

## Distractors
Distractors (incorrect answers only). Note that in testing we provided the model all potential answers, including the GTFA.
1. **Counterstain**: blames methylene blue for the cells not being blue, ignoring that the nuclei and threads are clearly blue.
2. **Primary stain**: reads the pink cells and deposits as overheated or unfiltered carbol fuchsin precipitate instead of fuchsin retention in cells.
3. **Fixative**: attributes the colour to inadequate heat fixation.
4. **Mordant**: blames the heat or phenol step for over-driving the stain.
5. **Rinse water**: blames insufficient washing that left surface fuchsin.

## Target failure mode
Signal-vs-artifact and protocol-knowledge reasoning. The model must read the pink cytoplasm of the non-acid-fast host cells as retained primary stain and trace it to the decolorization step. Plausible wrong paths are reading it as acid-fast material, blaming the counterstain, or focusing on precipitate.

**Error type to select when justifying:** Data extraction error (colour or structure misread) or Unextracted given / prior override.

## References
- WHO / Global Laboratory Initiative. Laboratory diagnosis of tuberculosis by sputum microscopy (GLI handbook, 2013), section on Ziehl–Neelsen staining and staining quality control: non-acid-fast background should be blue after counterstaining, and red or pink background indicates insufficient decolorization.

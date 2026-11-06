# 52 — Egg packet in a stool wet mount → intermediate host

**Supertype / subtype:** Microbiology — Parasitology & mycology mounts
**Subdomain:** Microbiology

## Source and license (form fields)
- **Image:** `task_images/52_dipylidium_image1.png` (Image 1)
- **Source URL / DOI:** https://doi.org/10.1186/s13071-025-06878-w
- **License type:** CC BY 4.0
- **Reference material (title):** Performance validation of deep-learning-based approach in stool examination
- **Where published:** Parasites & Vectors, Volume 18, Article 322, 2025
- **License of reference material (verbatim):** "Open Access This article is licensed under a Creative Commons Attribution 4.0 International License, which permits use, sharing, adaptation, distribution and reproduction in any medium or format, as long as you give appropriate credit to the original author(s) and the source, provide a link to the Creative Commons licence, and indicate if changes were made."
- **Image handling:** Fig 5a was downloaded at original size (1759 × 2490 px) from media.springernature.com. I cropped one tile only, removing the printed species name beneath it. The tile's own 20 µm scale bar is kept. Final size 565 × 393 px, PNG. No other edits.
- **Answer not in the publication:** the paper is an AI-classification study. It lists the species only as a class label and never mentions fleas, *Ctenocephalides*, egg packets, intermediate hosts or the life cycle.

## Prompt
Image 1 is a wet mount of a stool specimen viewed with the $40\times$ objective (scale bar = $20\ \mu\text{m}$). The structure shown was the only parasitic element found in the specimen.

Identify the parasite responsible, then name the genus of the arthropod intermediate host whose accidental ingestion most commonly transmits this infection to humans. In your response, describe the features in the image that support your identification and explain how they lead to the intermediate host.

End your response with a final line in exactly this format:
Final answer: <genus>

**Answer format:** Text (case insensitive)

## GTFA
Ctenocephalides

## Step-by-step solution
Step 1: Observe Image 1. A single tight cluster of about 11 round bodies sits in the upper centre of the field against a granular background. Each body has a thin, smooth, double-lined outer contour and a granular inner mass. Some inner masses show fine refractile lines.

Step 2: Use the scale bar. The 20 µm bar is about 57 px long, so 1 px ≈ 0.35 µm. Each round body is about 90–100 px across, which is about 32–35 µm.

Step 3: Interpret each body. A round, thin-shelled egg of about 30–40 µm containing an embryo with refractile hooklets is a hexacanth (oncosphere-bearing) cyclophyllidean tapeworm egg.

Step 4: Interpret the arrangement. The eggs are held together as a compact group of about 11, not scattered singly. This is an egg packet (egg capsule). Eggs packaged in packets of roughly 5–30 are characteristic of *Dipylidium caninum*. The look-alikes are ruled out:
- *Taenia* eggs occur singly and have a thick, dark, radially striated embryophore, which is absent here.
- *Hymenolepis nana* eggs occur singly.
- *H. diminuta* eggs occur singly and are larger, about 70–85 µm.

Step 5: Bring in the life cycle. The cysticercoid of *D. caninum* develops in fleas, which ingest the eggs as larvae. Humans, mostly young children, are infected by accidentally swallowing an infected adult flea from a dog or cat. The usual species are *Ctenocephalides canis* and *C. felis*.

Step 6: The genus of the intermediate host most commonly responsible for human infection is *Ctenocephalides*.

Final Answer: Ctenocephalides

## Image description (≈270 words)
Modality: a brightfield light micrograph of an unstained wet mount at moderate-high magnification (40× objective). It is a single rectangular field, wider than tall, with a pale blue background. A black scale bar labelled "20 µm" sits in the lower right corner; it is roughly one tenth of the image width.

Content: the dominant feature is one compact cluster of round, transparent bodies occupying the upper centre and centre of the frame, roughly half the image width across. About eleven bodies are packed together. Many touch or overlap their neighbours, so some outlines cross one another. Each body is nearly circular and roughly one and a half to two times the length of the scale bar in diameter. Each has a thin, smooth, clear outer wall drawn as a fine double line, with a narrow clear zone inside it. Within that is a rounded, finely granular inner mass, and in several bodies thin, short, refractile line-like structures are visible. The bodies are colourless to faintly yellow-green and lack any thick, dark or striated wall. No body lies isolated away from the cluster.

Surroundings: fine granular and flocculent debris fills the background, denser at the left edge, lower left and right side. The centre around the cluster is relatively clear.

Quality: focus is good on the upper and central bodies and slightly softer on the lower-left bodies, where overlapping outlines blur together. Illumination is even, with a bluish cast.

Artifacts: overlapping outlines within the cluster, background debris, a faint thin fibre crossing the upper part of the cluster.

Annotations: only the scale bar; no arrows, labels, numbers or captions.

## Distractors
Distractors (incorrect answers only). Note that in testing we provided the model all potential answers, including the GTFA.
1. **Tribolium**: the cluster is read as separate *Hymenolepis diminuta* eggs (flour-beetle intermediate host).
2. **Tenebrio**: the cluster is read as *Hymenolepis* eggs transmitted via mealworm beetles.
3. **Xenopsylla**: correctly reads "flea" but attributes the eggs to rodent *Hymenolepis*, which uses the rat flea.
4. **Cyclops**: the round eggs are taken for a pseudophyllidean or *Diphyllobothrium*-type cycle with a copepod first intermediate host.
5. **Diaptomus**: the same copepod error, choosing the alternative copepod genus.

## Target failure mode
Distinguishing a *Dipylidium* egg packet from a clump of individual taeniid or hymenolepidid eggs. This is a morphological interpretation error: the packet arrangement and thin, non-striated shells are the key visual evidence. It also needs protocol or life-cycle knowledge to reach the right intermediate host.

**Error types to select when justifying:**
- Data extraction error: misreading the cluster.
- Unextracted given / prior override: defaulting to the more common *Taenia* or *Hymenolepis* without using the packet arrangement.

## References
- CDC DPDx — Dipylidiasis (*Dipylidium caninum*): life cycle and diagnostic findings (egg packets; flea intermediate host, *Ctenocephalides* spp.). https://www.cdc.gov/dpdx/dipylidium/index.html
- CDC DPDx — Hymenolepiasis and Taeniasis pages for the look-alike egg morphology.

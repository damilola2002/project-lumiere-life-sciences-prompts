# 53 — Capillaria philippinensis egg vs Trichuris look-alike → source of infection

**Supertype / subtype:** Microbiology — Parasitology & mycology mounts
**Subdomain:** Microbiology
**Replaces:** task 52 (both models solved the *Dipylidium* packet).

## Source and license (form fields — same article as task 52)
- **Image:** `task_images/53_capillaria_image1.png` (Image 1)
- **Source URL / DOI:** https://doi.org/10.1186/s13071-025-06878-w
- **License type:** CC BY 4.0
- **Reference material (title):** Performance validation of deep-learning-based approach in stool examination
- **Where published:** Parasites & Vectors, Volume 18, Article 322, 2025
- **License of reference material (verbatim):** "Open Access This article is licensed under a Creative Commons Attribution 4.0 International License, which permits use, sharing, adaptation, distribution and reproduction in any medium or format, as long as you give appropriate credit to the original author(s) and the source, provide a link to the Creative Commons licence, and indicate if changes were made."
- **Image handling:** one tile from Fig 5a (row 2, centre). The printed species label below the tile is removed; the tile's own 20 µm scale bar is kept. Final size 564 × 392 px, PNG. No other edits.
- **Answer not in the publication:** the paper never mentions fish, diet, raw food or the life cycle (the words "fish" and "Trichuris" do not appear in connection with this egg).

## Prompt
Image 1 is a wet mount of a stool specimen viewed with the $40\times$ objective (scale bar = $20\ \mu\text{m}$). The egg shown was the only parasitic element found in the specimen.

Identify the parasite that produced this egg, then state what a person most commonly ingests to acquire this infection. In your response, describe the features of the egg in the image (including its size estimated from the scale bar) that support your identification, and explain how the identification leads to the route of acquisition.

End your response with a final line in exactly this format, using a single word:
Final answer: <what is ingested>

**Answer format:** Text (case insensitive)

## GTFA
Fish

## Step-by-step solution
Step 1: Observe Image 1. A single elongated oval egg with a thick, smooth, refractile double-contoured shell lies just left of centre. Its sides are nearly parallel. Both ends are slightly flattened, with small, flat, inconspicuous end plugs that do not project beyond the shell outline. The interior is filled with an undifferentiated granular mass, with a clear space at the lower pole.

Step 2: Measure with the scale bar. The 20 µm bar is about 57 px long, so 1 px ≈ 0.35 µm. The egg is about 126 px long and 62 px wide, so it measures about 44 × 22 µm.

Step 3: Narrow down the egg type. A thick-shelled, oval nematode egg with plugs at both ends belongs to the trichurid group (*Trichuris*, *Capillaria/Calodium*, *Paracapillaria*).

Step 4: Rule out *Trichuris trichiura*, the commonest bipolar-plugged egg:
- It is larger, about 50–55 × 22–24 µm.
- It is barrel- or lemon-shaped, with prominent, protruding, hyaline polar plugs.

The egg in Image 1 is smaller (about 44 µm long), more parallel-sided, and has flat, non-protruding plugs. It also differs from *Calodium hepaticum* (48–66 µm, with a pitted shell). These features match *Capillaria (Paracapillaria) philippinensis*, whose eggs measure about 36–45 × 20 µm, are peanut- or oval-shaped, and have flattened bipolar plugs.

Step 5: Apply the life cycle. *C. philippinensis* is a fish-borne zoonotic nematode. Larvae develop in small freshwater or brackish-water fish, and humans are infected by eating those fish raw or undercooked. Autoinfection then amplifies the intestinal worm burden. By contrast, *Trichuris* is acquired by swallowing embryonated eggs from soil.

Step 6: What is ingested to acquire the infection is fish.

Final Answer: Fish

## Image description (≈255 words)
Modality: a brightfield light micrograph of an unstained wet mount, 40× objective. It is a single rectangular field, wider than tall, with a pale grey-blue background. A black scale bar labelled "20 µm" sits in the lower right corner and is about one tenth of the image width.

Content: one elongated, oval, transparent object lies just left of the image centre, with its long axis vertical. It is roughly two scale-bar lengths long and about one scale-bar length wide. Its wall is a thick, smooth, bright, refractile double line of even thickness. The long sides are nearly parallel. Both ends are gently rounded to slightly flattened. Each end shows a short, flat thickening of the wall that does not project outward. Inside, a finely granular, speckled mass fills most of the object, leaving a small clear space at the lower end.

Surroundings: to the right of the object is a loose cluster of small granules, and further right a flat, angular, triangular translucent fragment. Several thin, straight, needle-like crystalline fragments lie at the left and lower left. Small round refractile bodies and fine debris are scattered across the field.

Quality: focus is sharp on the oval object and its wall. Illumination is even, with a slight halo around refractile edges. Resolution is sufficient to see the wall layers.

Artifacts: needle-shaped fragments, an angular plant-like fragment, and granular debris near the object.

Annotations: only the scale bar; there are no arrows, labels, numbers or captions.

## Distractors
Distractors (incorrect answers only). Note that in testing we provided the model all potential answers, including the GTFA.
1. **Soil**: misidentifies the egg as *Trichuris trichiura* by ignoring the size (~44 µm) and the flat plugs.
2. **Eggs**: also the *Trichuris* misreading (direct ingestion of embryonated eggs).
3. **Liver**: reads it as *Calodium hepaticum*, a spurious passage after eating infected liver.
4. **Vegetables**: *Trichuris* plus faecally contaminated produce.
5. **Snails**: reads it as a trematode or *Angiostrongylus*-type egg acquired from molluscs.

## Target failure mode
Magnification/scale interpretation combined with normal-vs-look-alike discrimination. Models default to the far more common *Trichuris* egg without measuring against the scale bar or noticing the flat, non-protruding plugs. That leads to soil or egg ingestion instead of raw fish.

**Error types to select when justifying:**
- Axis, scale & unit misread / Figure-based quantitative estimation error: size not measured or measured wrongly.
- Data extraction error: plug morphology misread.

## References
- CDC DPDx — Capillariasis (intestinal): *Paracapillaria philippinensis* egg morphology (36–45 × 20 µm, flattened bipolar plugs, striated shell) and life cycle (ingestion of raw or undercooked freshwater/brackish fish). https://www.cdc.gov/dpdx/intestinalcapillariasis/index.html
- CDC DPDx — Trichuriasis: *T. trichiura* egg morphology (50–55 × 20–25 µm, barrel-shaped, protruding polar plugs). https://www.cdc.gov/dpdx/trichuriasis/index.html

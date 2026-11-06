# 54 — Fifteen stool-egg panels: how many infections are fish-borne?

**Supertype / subtype:** Microbiology — Parasitology & mycology mounts
**Subdomain:** Microbiology
**Replaces:** tasks 52 and 53, which both models solved. A single, isolated egg proved too easy, so this task needs 15 look-alike identifications that feed one count.

## Source and license (form fields — same article as tasks 52/53)
- **Images:** `task_images/54_image1.png` … `54_image5.png` (Images 1–5)
- **Source URL / DOI:** https://doi.org/10.1186/s13071-025-06878-w
- **License type:** CC BY 4.0
- **Reference material (title):** Performance validation of deep-learning-based approach in stool examination
- **Where published:** Parasites & Vectors, Volume 18, Article 322, 2025
- **License of reference material (verbatim):** "Open Access This article is licensed under a Creative Commons Attribution 4.0 International License, which permits use, sharing, adaptation, distribution and reproduction in any medium or format, as long as you give appropriate credit to the original author(s) and the source, provide a link to the Creative Commons licence, and indicate if changes were made."
- **Image handling:** each image is one complete row of three tiles, cropped from Fig 5a or the Fig 5a continuation. The crops are 1759 × ~401 px PNG, each under 1 MB. The printed species labels sit below each row and are excluded. Every tile keeps its own 20 µm scale bar. No other edits. Source rows:
  - Image 1 = Fig 5a row 2
  - Image 2 = Fig 5a row 4
  - Image 3 = Fig 5a row 5
  - Image 4 = Fig 5a continuation row 1
  - Image 5 = Fig 5a continuation row 4
- **Answer not in the publication:** the paper only labels species for AI training. It never discusses routes of infection, fish or food sources, and this count appears nowhere.

## Prompt
Images 1–5 are wet mounts of stool specimens photographed with the $40\times$ objective. Each image contains three panels (left, centre, right), and every panel has its own $20\ \mu\text{m}$ scale bar. Each of the 15 panels comes from a different patient, and the helminth egg(s) shown in a panel are the only parasitic finding for that patient.

How many of the 15 patients acquired their infection by eating raw or undercooked fish? Count a patient only if finfish are the source of the infective stage in the parasite's life cycle; crustaceans, molluscs, other meats, plants, soil, water and insects do not count. Count patients (panels), not individual eggs.

End your response with a final line in exactly this format:
Final answer: <integer>

**Answer format:** Integer — exact match.

## GTFA
4

## Step-by-step solution
Step 1: Image 1, left. A thin-shelled, smooth oval egg (about 2 scale bars long) contains a segmented, multi-cell embryo with a clear space under the shell. The yellow-brown angular body beside it lacks a shell and is debris. This is a hookworm egg, acquired by skin penetration of soil larvae. **Not fish.**

Step 2: Image 1, centre. A thick-walled, parallel-sided egg (about 2.2 scale bars, ~44 µm long) has flat, non-protruding plugs at both ends. This is a *Capillaria (Paracapillaria) philippinensis* egg, not *Trichuris* (50–55 µm, protruding plugs). It is acquired from raw small freshwater or brackish fish. **Fish (1).**

Step 3: Image 1, right. A broadly oval, thin-shelled egg (about 3 scale bars, ~65 µm) has a small lid at one end, no shoulders, and a granular, unembryonated content. This is a *Dibothriocephalus (Diphyllobothrium) latum*-type tapeworm egg, acquired from plerocercoids in raw fish. **Fish (2).**

Step 4: Image 2, left. A flattened-oval egg, convex on one side and flat on the other, has a smooth double shell and contains a larva. This is *Enterobius vermicularis*, acquired by ingesting eggs. **Not fish.**

Step 5: Image 2, centre and right. Very large operculated eggs (about 4–6 scale bars, >120 µm) with unembryonated granular content. These are *Fasciola* and *Fasciolopsis buski*, acquired from metacercariae on aquatic plants. **Not fish.**

Step 6: Image 3, left. The largest egg (about 7 scale bars) has a lid at one end. This is *Gastrodiscoides hominis*, acquired from aquatic plants. **Not fish.**

Step 7: Image 3, centre. Three very small eggs (about 1.5 scale bars, ~30 µm) each have a shouldered lid and an embryo inside. This is a heterophyid fluke (*Haplorchis*), acquired from metacercariae in raw freshwater fish. It is one patient, so it counts once. **Fish (3).**

Step 8: Image 3, right. A large round egg has a thick outer shell and a separate inner membrane around a hooked embryo, with no polar filaments. This is *Hymenolepis diminuta*, acquired by ingesting insects such as grain beetles. **Not fish.**

Step 9: Image 4, left. A smaller round to oval egg has an inner membrane enclosing a hooked embryo. This is *Hymenolepis nana*, acquired by ingesting eggs or insects. **Not fish.**

Step 10: Image 4, centre. A small (about 1.5 scale bars), yellow-brown, flask-shaped egg has a shouldered lid and contains an embryo. This is *Opisthorchis viverrini*, acquired from raw cyprinid fish. **Fish (4).**

Step 11: Image 4, right. A large (about 4 scale bars, ~85–90 µm), thick-shelled, golden oval egg has a flattened lid with shoulders and a thickened opposite end. This is *Paragonimus*, acquired from raw freshwater crabs or crayfish (crustaceans). **Not fish.**

Step 12: Image 5, left. A small round egg has a thick, dark, radially striated wall. This is a *Taenia* egg, acquired from beef or pork. **Not fish.**

Step 13: Image 5, centre. A round, thick, brownish, pitted-shelled egg. This is a *Toxocara* egg, from ingestion of eggs (spurious finding in humans). **Not fish.**

Step 14: Image 5, right. An elongated, thin-shelled egg (about 3 scale bars) with a tapered pole and an advanced segmented embryo. This is *Trichostrongylus orientalis*, acquired from larvae on vegetables. **Not fish.**

Step 15: Sum the fish-borne panels: Image 1 centre, Image 1 right, Image 3 centre and Image 4 centre, giving 4.

Final Answer: 4

## Image description (≈470 words)
Modality: five brightfield light micrographs of unstained wet mounts. Each image is a horizontal strip of three separate rectangular panels (left, centre, right) with rounded black borders, all photographed at the same magnification. Every panel has a black scale bar labelled "20 µm" in its lower right corner, so 15 panels in total. Backgrounds vary from pale grey-blue to beige and contain scattered fine debris.

Image 1:
- **Left:** a smooth, thin-walled oval body about two scale bars long. Inside is a dark granular mass divided into a few rounded lobes, with a clear gap under the wall. Next to it is a shell-less, yellow-brown, angular body, and a large orange-brown cloud of debris fills the right side of the panel.
- **Centre:** a thick-walled, bright, elongated oval body about two scale bars long with nearly parallel sides. Each end has a small, flat wall thickening that does not stick out. The interior is granular. Needle-like fragments and a triangular fragment lie nearby.
- **Right:** a broad oval body about three scale bars long with a thin smooth wall and a small lid-like line at the upper-left end. It is filled with coarse yellow-green granules.

Image 2:
- **Left:** a narrow oval body, flatter on one side, with a double-contoured clear wall around a granular, worm-like interior.
- **Centre:** a very large oval body (over four scale bars) with a thin iridescent wall and dense brown granular contents, beside clumped debris.
- **Right:** the largest oval body in this image (about six scale bars). It has a thin wall, a small lid at the upper-left end, and mottled green-grey contents.

Image 3:
- **Left:** an extremely large, broad oval body (about seven scale bars) with a lid at its narrow left end. It is filled with scattered refractile globules.
- **Centre:** three small, pale, oval bodies, each only about one and a half scale bars long. Each has a distinct rim at one end where the wall forms a cap, and a granular interior. They are widely separated on a clean background.
- **Right:** a large round body about three scale bars across. It has a thick outer wall, a clear gap, and a separate inner membrane around a central body containing fine rod-like structures. Filamentous debris trails from it.

Image 4:
- **Left:** a round-oval body about two scale bars across with a thin outer wall, a wide clear zone, and an inner membrane around a central granular body.
- **Centre:** a tiny yellow-brown, flask-shaped body (about one and a half scale bars) with a cap at one end and a coiled interior, in a field of fine debris.
- **Right:** a large golden-tan oval body (about four scale bars) with a thick wall, a flattened cap at the upper end bordered by a slight rim, and a thickened opposite end. It is filled with green granules.

Image 5:
- **Left:** a small round body about one and a half scale bars across with a thick, dark brown, finely striped wall and a granular centre.
- **Centre:** a round body about two scale bars across with a thick, brownish, slightly rough wall, partly overlapped by debris.
- **Right:** an elongated, thin, clear-walled oval body about three scale bars long, slightly tapered at one end. It contains a segmented dark mass of many cells.

Quality: most objects are in sharp focus. Some panels have uneven background tint and debris clumps overlapping the edges of objects.

Annotations: scale bars only; there are no labels, arrows or numbers.

## Distractors
Distractors (incorrect answers only). Note that in testing we provided the model all potential answers, including the GTFA.
1. **3**: Image 1 centre is misread as *Trichuris* (soil), or Image 1 right is misread as a non-fish trematode egg. One fish-borne panel is missed.
2. **5**: Image 4 right (*Paragonimus*, crab-borne) is misread as a *Diphyllobothrium*-type tapeworm egg and counted as fish.
3. **6**: counts the three eggs in Image 3 centre separately (eggs rather than patients).
4. **2**: misses both look-alikes in Image 1 (*Capillaria* taken as *Trichuris*, and *Diphyllobothrium* taken as *Fasciola*-type).
5. **7**: also counts the large operculated eggs in Image 2 centre and right and Image 4 right as fish-borne fluke or tapeworm eggs.

## Target failure mode
Distinguishing look-alike operculated and bipolar-plugged eggs across many panels, using scale-bar size and fine morphology:
- *Capillaria* vs *Trichuris*.
- *Diphyllobothrium* vs *Paragonimus* vs *Fasciola*-group eggs.
- Small heterophyid or opisthorchiid eggs.

These are identification errors that change the fish-borne count.

**Error types to select when justifying:**
- Data extraction error: wrong egg identity.
- Figure-based quantitative estimation error: size misjudged against the scale bar.

## References
- CDC DPDx — Intestinal capillariasis, Diphyllobothriasis, Heterophyiasis, Opisthorchiasis, Paragonimiasis, Fascioliasis, Fasciolopsiasis, Hymenolepiasis, Taeniasis, Toxocariasis, Trichostrongyliasis, Enterobiasis and Hookworm pages (egg morphology, sizes and life cycles). https://www.cdc.gov/dpdx/

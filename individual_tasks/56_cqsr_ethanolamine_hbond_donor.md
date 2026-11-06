# 56 — CqsR–ethanolamine LigPlot+: which protein atom donates an H-bond?

**Assay type (assigned):** Protein-ligand — Molecular diagrams (small molecule–protein binding interactions)
**Subdomain:** Biochemistry

## Source and license (form fields)
- **Image:** `task_images/56_ligplot_image1.png` (Image 1)
- **Source URL / DOI:** https://doi.org/10.1371/journal.ppat.1013447
- **License type:** CC BY 4.0
- **Reference material (title):** Structure-function studies of Vibrio cholerae quorum-sensing receptor CqsR signal recognition
- **Where published:** PLOS Pathogens, Volume 21, Issue 9, e1013447, 2025
- **License of reference material (verbatim):** "This is an open access article distributed under the terms of the Creative Commons Attribution License, which permits unrestricted use, distribution, and reproduction in any medium, provided the original author and source are credited."
- **Structure provenance:** experimentally determined X-ray crystal structure, PDB **9NIA** (CqsRp–ethanolamine). Fig 2A shows the Fo–Fc omit density for the ligand. This is not a docking or modelled pose.
- **Image handling:** Fig 2 downloaded at original size (2029 × 2400 px) from journals.plos.org. Cropped to panel C only (the LigPlot+ diagram), excluding the panel letter and the "CqsRp-Ethanolamine" title beneath. Final 994 × 845 px PNG. No other edits.
- **Answer not in the publication:** the paper says the amine is protonated, Asp198 is anionic, and the hydroxyl "hydrogen bonds with" Thr196. It never states which partner donates in the Thr196 contact, and never names any protein donor atom.

## Prompt
Image 1 is a LigPlot+ diagram of the ligand-binding site in the X-ray crystal structure of a bacterial receptor bound to ethanolamine. Ligand bonds are grey and protein bonds are blue. Carbon is black, nitrogen blue and oxygen red. Black dashed lines, labelled with donor–acceptor distances in Å, are the hydrogen bonds identified in the structure. Red arcs mark hydrophobic contacts.

Assume every titratable group is in its predominant protonation state at pH 7.4, and that every dashed line is a genuine hydrogen bond (a single hydrogen may form a bifurcated hydrogen bond to both oxygens of one carboxylate).

Which protein atom or atoms in the diagram donate a hydrogen to ethanolamine? Give each as the residue's three-letter code and number followed by its PDB atom name. If there is more than one, list them all, separated by commas.

End your response with a final line in exactly this format:
Final answer: <residue number atom name>

**Answer format:** Text (case insensitive)

## GTFA
Thr196 OG1

## Step-by-step solution
Step 1: Read the ligand. Ethanolamine is shown as two black carbons joined by grey bonds, with a blue nitrogen on the left and a red oxygen on the right: HO–CH₂–CH₂–NH₂.

Step 2: Read the contacts on the ligand nitrogen. It has three dashed lines:
- to the red side-chain oxygen at the end of the Y169 ring (Tyr169 OH), 2.83 Å;
- to an oxygen of the D171 carboxylate, 2.70 Å;
- to the left oxygen of the D198 carboxylate, 2.87 Å.

Step 3: Read the contacts on the ligand oxygen. It has three dashed lines:
- to the side-chain oxygen of T196 (Thr196 OG1, on the carbon carrying the methyl branch), 2.65 Å;
- to the right oxygen of the D198 carboxylate, 2.68 Å;
- to the left oxygen of the D198 carboxylate, 3.18 Å.

Step 4: Assign protonation states at pH 7.4:
- The primary amine of ethanolamine (pKa ≈ 9.5) is protonated, –NH₃⁺. It has three N–H donors and no lone pair, so it cannot accept.
- Asp171 and Asp198 (pKa ≈ 3.9) are deprotonated carboxylates. Their oxygens can only accept.
- The Tyr169 OH (pKa ≈ 10) and the Thr196 OH are neutral hydroxyls. Each can either donate its single H or accept.

Step 5: Settle the nitrogen contacts. NH₃⁺ cannot accept, so all three contacts have the ligand as donor, using all three of its H atoms. In particular, Tyr169 OH is the acceptor in its bond to the ammonium, not a donor.

Step 6: Settle the oxygen contacts. The ligand hydroxyl has one H. Its contacts with the two Asp198 carboxylate oxygens can only be hydrogen bonds if the ligand donates. Carboxylate O cannot donate to an O–H oxygen without a hydrogen of its own, so the ligand O–H must donate to Asp198 (bifurcated across the two oxygens, as allowed). With its only H used, the ligand oxygen must act as an acceptor in the remaining contact, so Thr196 OG1 donates its hydroxyl H to the ethanolamine oxygen.

Step 7: The only protein atom donating a hydrogen to ethanolamine is the hydroxyl oxygen of Thr196, PDB atom name OG1.

Final Answer: Thr196 OG1

## Image description (≈330 words)
Modality: a two-dimensional schematic interaction diagram of the kind produced by LigPlot+ from a crystal structure. White background, no scale bar.

Content: in the centre is a small ligand labelled "Ethanolamine". It is drawn as two black spheres (carbons) joined by short grey bonds. The left carbon connects to a blue sphere (nitrogen), and the right carbon connects to a red sphere (oxygen). Both carbons carry small red radiating ticks.

Surrounding residues are drawn with light-blue bonds and black, blue and red spheres, and labelled with one-letter codes and numbers:
- **Upper left, "Y169":** a chain ending in a six-membered ring of black spheres, whose far vertex carries a red sphere. A dashed line labelled "2.83" runs from that red sphere to the ligand's blue sphere.
- **Left, "D171":** a short chain ending in a carbon bearing two red spheres. A dashed line labelled "2.70" runs from the upper of these red spheres to the ligand's blue sphere.
- **Below the ligand, "D198":** a chain whose top carbon bears two red spheres side by side. A near-vertical dashed line labelled "2.87" joins the left red sphere to the ligand's blue sphere. A diagonal dashed line joins the same left red sphere to the ligand's red sphere; the label "3.18" sits just below the ligand between its two end atoms. A second near-vertical dashed line labelled "2.68" joins the right red sphere to the ligand's red sphere.
- **Right, "T196":** a short branched chain. One branch carbon bears a red sphere, which connects to the ligand's red sphere by a dashed line labelled "2.65". The neighbouring carbon carries a red sphere and a blue sphere, and another branch ends in a black sphere with red ticks.
- **Upper part:** four red semicircles with radiating spokes labelled "W105", "W151", "W138" and "F123", with no dashed lines.

Quality: crisp vector-style graphic. All labels and numbers are legible.

Annotations: residue labels, the ligand name and distance values (in Å) are part of the diagram. There are no arrows, legends or panel letters.

## Distractors
Distractors (incorrect answers only). Note that in testing we provided the model all potential answers, including the GTFA.
1. **Tyr169 OH**: treats the amine as neutral (–NH₂, an acceptor), so the tyrosine hydroxyl is read as donating to the nitrogen.
2. **Tyr169 OH, Thr196 OG1**: the same error, plus correctly identifying Thr196.
3. **Asp198 OD1**: misreads the carboxylate as a donor (protonated Asp) toward the ligand hydroxyl.
4. **Thr196 N**: mis-binds the 2.65 Å line to the backbone nitrogen (blue sphere) of T196 instead of its side-chain oxygen.
5. **Thr196 OG1, Asp198 OD2**: correctly identifies Thr196, but also lets the 3.18 Å contact be an Asp198 donation.

## Target failure mode
Atom-level reading of the diagram (which coloured sphere each dashed line ends on) combined with protonation-state chemistry. Models typically misjudge the protonation state of the amine and so make Tyr169 a donor, or mis-bind a distance line to the wrong atom.

**Error types to select when justifying:**
- Label–element mis-binding (line attached to the wrong atom).
- Chemical structure misinterpretation (protonation or donor/acceptor role).

## References
- Guarnaccia et al. (2025) PLOS Pathog 21(9): e1013447. PDB 9NIA.
- Standard pKa values: primary amine ~9.5–10.5; Asp side chain ~3.9; Tyr OH ~10.1. Example source: Berg, Tymoczko & Stryer, *Biochemistry*, ionizable groups table.

# 57 — CqsR–serinol LigPlot+: which protein atoms donate H-bonds? (replaces 56)

**Assay type:** Protein-ligand — Molecular diagrams
**Subdomain:** Biochemistry

## Source and license (same article as task 56; only the image changes)
- **Image:** `task_images/57_serinol_image1.png` (Image 1)
- **Source DOI:** https://doi.org/10.1371/journal.ppat.1013447
- **License type:** CC BY 4.0
- **Reference title:** Structure-function studies of Vibrio cholerae quorum-sensing receptor CqsR signal recognition
- **Where published:** PLOS Pathogens, Volume 21, Issue 9, e1013447, 2025
- **License of reference material:** "This is an open access article distributed under the terms of the Creative Commons Attribution License, which permits unrestricted use, distribution, and reproduction in any medium, provided the original author and source are credited."
- **Structure provenance:** X-ray crystal structure, PDB 9NIV (CqsRp–serinol). Fig 5B shows the Fo–Fc omit density.
- **Image handling:** Fig 5 panel F (LigPlot+) cropped from the original 2066 × 2400 px figure. The panel letter is excluded and nothing else is changed. 1001 × 765 px PNG.
- **Answer not in the publication:** the text says only that residues "mediate additional contacts" or "hydrogen bonds". It never assigns donor or acceptor roles, and never mentions Trp138 donating.

## Prompt
Image 1 is a LigPlot+ diagram of the ligand-binding site in the X-ray crystal structure of a bacterial receptor bound to serinol. Ligand bonds are grey and protein bonds are green. Carbon is black, nitrogen blue and oxygen red. Black dashed lines, labelled with donor–acceptor distances in Å, are the hydrogen bonds identified in the structure. Red arcs mark hydrophobic contacts.

Assume every titratable group is in the protonation state predicted by its standard aqueous pKa at pH 7.4, and that every dashed line is a genuine hydrogen bond (a single hydrogen may form a bifurcated hydrogen bond to both oxygens of one carboxylate).

Which protein atom or atoms in the diagram donate a hydrogen to serinol? Give each as the residue's three-letter code and number followed by its PDB atom name. If there is more than one, list them all, separated by commas.

End your response with a final line in exactly this format, listing one or more atoms:
Final answer: <Xxx### ATOM>, <Xxx### ATOM>, ...
(format example only, not a candidate answer: "Final answer: Ser45 OG, Lys12 NZ")

**Answer format:** Text (case insensitive) — unordered list

## GTFA
Trp138 NE1, Thr196 OG1

## Step-by-step solution
Step 1: Read the ligand. Serinol (2-amino-1,3-propanediol) is drawn in grey. The central carbon carries the blue nitrogen. There is a red hydroxyl oxygen at the upper left (O-a) and a red hydroxyl oxygen at the right (O-b).

Step 2: Read the dashed lines from the image.
- **N:** to the Y169 ring-end oxygen (Tyr169 OH), 2.74 Å; to the upper D171 carboxylate oxygen, 2.60 Å; to the left D198 carboxylate oxygen, 2.71 Å.
- **O-a:** to the blue ring nitrogen of the W138 indole (Trp138 NE1), 2.73 Å; to the same upper D171 carboxylate oxygen, 2.36 Å.
- **O-b:** to the T196 side-chain oxygen (Thr196 OG1), 2.68 Å; to the right D198 oxygen, 2.74 Å; to the left D198 oxygen, 3.24 Å.

Step 3: Assign protonation states at pH 7.4 from standard pKa values:
- The ligand amine (pKa ~9) is –NH₃⁺. It can donate three H atoms and has no lone pair.
- Asp171 and Asp198 (pKa ~3.9) are carboxylates and can only accept.
- The Tyr OH and Thr OH are neutral and can donate or accept.
- The Trp indole NE1–H is neutral. Its nitrogen lone pair is part of the aromatic sextet, so it is a donor only.

Step 4: N contacts. NH₃⁺ cannot accept, so it donates to Tyr169 OH, Asp171 and Asp198. Tyr169 OH is therefore an **acceptor**.

Step 5: O-b contacts. Its single H must go to Asp198, bifurcated over the two oxygens, because a carboxylate cannot donate. O-b therefore **accepts** from Thr196 OG1, so **Thr196 OG1 is a donor**.

Step 6: O-a contacts. Asp171's oxygen can only accept, so O-a donates its single H to Asp171 (2.36 Å). Trp138 NE1 can only donate, so it donates to O-a, which accepts with a lone pair. **Trp138 NE1 is a donor.**

Step 7: Protein donors to serinol: Trp138 NE1 and Thr196 OG1.

Final Answer: Trp138 NE1, Thr196 OG1

## Image description (≈330 words)
Modality: a two-dimensional schematic interaction diagram of the LigPlot+ type, from a crystal structure. White background, no scale bar.

Content: in the centre is a ligand labelled "Serinol", drawn with grey bonds. A central black carbon carries a blue sphere (nitrogen) below it and two branches. One branch ends at the upper left in a red sphere through one black carbon. The other ends at the right in a red sphere through one black carbon. Two ligand carbons show small red radiating ticks.

Residues are drawn with green bonds and labelled:
- **Upper left, "W138":** a backbone segment with a red and a blue sphere, attached to a fused bicyclic ring system (a five-membered ring fused to a six-membered ring). The five-membered ring contains one blue sphere, which is joined by a dashed line labelled "2.73" to the ligand's upper-left red sphere.
- **Left, "Y169":** a chain ending in a six-membered ring whose far vertex carries a red sphere. A long dashed line labelled "2.74" runs from that red sphere to the ligand's blue sphere.
- **Lower left, "D171":** a chain ending in a carbon bearing two red spheres. The upper-right red sphere, labelled "2.60" beside it, receives two dashed lines: one from the ligand's blue sphere and one, labelled "2.36", from the ligand's upper-left red sphere.
- **Bottom centre, "D198":** a chain whose top carbon bears two red spheres side by side. The left sphere joins the ligand's blue sphere ("2.71"). It also joins the ligand's right red sphere by a diagonal line whose label "3.24" sits just right of the blue sphere. The right sphere joins the ligand's right red sphere ("2.74").
- **Right, "T196":** a short branched chain. One carbon bears a red sphere connected to the ligand's right red sphere by a dashed line labelled "2.68". A blue sphere and another red sphere sit on the neighbouring atoms.
- **Upper right:** red semicircles with spokes labelled "W105", "W151" and "F123", with no dashed lines.

Quality: crisp graphic; all text legible. Several dashed lines cross near the ligand nitrogen.

Annotations: residue labels, the ligand name and distances are intrinsic to the diagram. There are no arrows or legend.

## Distractors
Distractors (incorrect answers only). Note that in testing we provided the model all potential answers, including the GTFA.
1. **Thr196 OG1**: misses Trp138 because it treats the indole nitrogen as an acceptor.
2. **Tyr169 OH, Thr196 OG1, Trp138 NE1**: treats the amine as neutral, so Tyr169 is made a donor.
3. **Asp171 OD1, Trp138 NE1, Thr196 OG1**: reads the 2.36 Å contact as protonated Asp171 donating.
4. **Tyr169 OH, Thr196 OG1**: both the indole and the amine errors.
5. **Trp138 N, Thr196 OG1**: mis-binds the 2.73 Å line to the backbone nitrogen of W138 instead of the ring NE1.

## Target failure mode
A network of coupled donor/acceptor choices across eight contacts. The solver has to decide whether the indole NH is a donor or an acceptor, keep the amine protonated, resist reading Asp171 as protonated at 2.36 Å, and trace crowded lines to the right atoms (label–element mis-binding).

**Error types:**
- Chemical structure misinterpretation.
- Label–element mis-binding.

## References
- Guarnaccia et al. (2025) PLOS Pathog 21(9): e1013447; PDB 9NIV.
- Standard pKa values and the hydrogen-bonding behaviour of the indole NH (donor only), e.g. Berg, Tymoczko & Stryer, *Biochemistry*.

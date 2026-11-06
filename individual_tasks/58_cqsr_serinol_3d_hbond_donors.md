# 58 — CqsR–serinol 3D stick view: which protein atoms donate H-bonds? (replaces 57)

**Assay type:** Protein-ligand — Molecular structure
**Subdomain:** Biochemistry

## Source and license (same article as tasks 56/57)
- **Image:** `task_images/58_serinol3d_image1.png` (Image 1)
- **Source DOI:** https://doi.org/10.1371/journal.ppat.1013447
- **License type:** CC BY 4.0
- **Reference title:** Structure-function studies of Vibrio cholerae quorum-sensing receptor CqsR signal recognition
- **Where published:** PLOS Pathogens, Volume 21, Issue 9, e1013447, 2025
- **License of reference material:** "This is an open access article distributed under the terms of the Creative Commons Attribution License, which permits unrestricted use, distribution, and reproduction in any medium, provided the original author and source are credited."
- **Structure provenance:** X-ray crystal structure, PDB 9NIV (CqsRp–serinol); omit density is shown in Fig 5B.
- **Image handling:** Fig 5 panel D (PyMOL stick view) cropped from the original 2066 × 2400 px figure. The panel letter is excluded and nothing else is changed. 1033 × 763 px PNG.
- **Answer not in the publication:** the paper never assigns donor or acceptor roles, and never names any protein donor atom.

## Prompt
Image 1 is a stick representation of the ligand-binding site in the X-ray crystal structure of a bacterial receptor bound to serinol. Protein residues are shown as green sticks and labelled with one-letter codes and numbers. Serinol is shown as a ball-and-stick model (carbon grey). Nitrogen is blue and oxygen red. Black dashed lines, labelled with donor–acceptor distances in Å, are the hydrogen bonds identified in the structure.

Assume every titratable group is in the protonation state predicted by its standard aqueous pKa at pH 7.4, and that every dashed line is a genuine hydrogen bond (a single hydrogen may form a bifurcated hydrogen bond to both oxygens of one carboxylate).

Which protein atom or atoms in the image donate a hydrogen to serinol? Give each as the residue's three-letter code and number followed by its PDB atom name. If there is more than one, list them all, separated by commas.

End your response with a final line in exactly this format, listing one or more atoms:
Final answer: <Xxx### ATOM>, <Xxx### ATOM>, ...
(format example only, not a candidate answer: "Final answer: Ser45 OG, Lys12 NZ")

**Answer format:** Unordered list (or Text, case insensitive)

## GTFA
Trp138 NE1, Thr196 OG1

## Step-by-step solution
Step 1: Identify serinol, the ball-and-stick model the arrow points to: three grey carbons, one blue nitrogen (on the central carbon) and two red oxygens. One oxygen is at the upper left of the ligand (O-a) and one at the right (O-b). Serinol is HOCH₂–CH(NH₂)–CH₂OH.

Step 2: Trace each dashed line to its end atoms.
- **O-a:**
  - up to the blue ring nitrogen of the W138 indole, 2.7 Å. The line starts at the W138 five-membered-ring N. The nearby blue N of W151 has no dashed line.
  - down-left to the red side-chain oxygen of D171, 2.4 Å.
- **Ligand N:**
  - left to the same D171 carboxylate oxygen, 2.6 Å;
  - to the red hydroxyl oxygen at the end of the Y169 ring, which lies just below and behind D171, 2.7 Å;
  - down-right to the left carboxylate oxygen of D198, 2.7 Å.
- **O-b:**
  - right to the red hydroxyl oxygen of T196, 2.7 Å;
  - down to the two carboxylate oxygens of D198, 3.2 Å and 2.7 Å.

Step 3: Assign protonation states at pH 7.4 from standard pKa values:
- The amine (pKa ≈ 9) is NH₃⁺: a donor only, with three H.
- Asp171 and Asp198 (pKa ≈ 3.9) are carboxylates: acceptors only.
- Tyr169 OH (pKa ≈ 10) and Thr196 OG1 are neutral and can donate or accept.
- The Trp indole N–H is a donor only: its lone pair is part of the aromatic system.

Step 4: The ligand N donates its three H atoms to Tyr169 OH, Asp171 and Asp198. Tyr169 OH is therefore an acceptor.

Step 5: O-b must donate its only H to Asp198, bifurcated across both oxygens, so it accepts from Thr196. **Thr196 OG1 is a donor.**

Step 6: O-a must donate its only H to Asp171 (2.4 Å), and it accepts from the Trp138 indole N–H, which can only donate. **Trp138 NE1 is a donor.** Trp151 makes no hydrogen bond in the image.

Step 7: Protein donors to serinol: Trp138 NE1 and Thr196 OG1.

Final Answer: Trp138 NE1, Thr196 OG1

## Image description (≈330 words)
Modality: a three-dimensional molecular graphics rendering (PyMOL-style sticks) of a protein binding site from a crystal structure, on a white background. It is a single panel with no scale bar.

Content: in the centre is a small ball-and-stick molecule labelled "Serinol", indicated by a black arrow from the left. It has three grey carbon balls in a short chain, a blue nitrogen ball hanging below the central carbon, a red oxygen ball at the upper-left end and a red oxygen ball at the right end.

Green stick residues surround it, each labelled:
- **Top left, "W138":** a fused bicyclic ring whose five-membered ring contains a blue nitrogen pointing down toward the ligand. A dashed line labelled "2.7" runs from that blue nitrogen down to the ligand's upper-left red oxygen.
- **Upper centre, "W151":** a similar bicyclic ring lying across the ligand. Its blue ring nitrogen sits just right of that dashed line and close to the ligand oxygen, with no dashed line of its own.
- **Upper right, "W105":** another bicyclic ring with a blue nitrogen, far from the ligand, and "F123", a ring below it.
- **Left, "D171":** a side chain whose red oxygen receives a dashed line labelled "2.4" from the ligand's upper-left oxygen and one labelled "2.6" from the ligand nitrogen.
- **Lower left, "Y169":** a six-membered ring partly behind D171. Its terminal red oxygen connects to the ligand nitrogen by a dashed line labelled "2.7".
- **Bottom, "D198":** a side chain ending in two red oxygens. The left oxygen receives a line labelled "2.7" from the ligand nitrogen. The ligand's right oxygen sends lines labelled "3.2" and "2.7" to the two D198 oxygens.
- **Right, "T196":** a short branched side chain whose red oxygen receives a dashed line labelled "2.7" from the ligand's right oxygen.

Quality: crisp rendering, but residues overlap in depth. D171 and Y169 overlap, W151 lies over the ligand, and several dashed lines cross near the ligand nitrogen.

Annotations: residue labels, the ligand name with its arrow, and the distance labels. No legend or scale.

## Distractors
Distractors (incorrect answers only). Note that in testing we provided the model all potential answers, including the GTFA.
1. **Trp151 NE1, Thr196 OG1**: binds the 2.7 Å line to the nearby W151 ring nitrogen instead of W138 (depth/proximity mis-binding).
2. **Trp138 NE1, Trp151 NE1, Thr196 OG1**: adds the W151 nitrogen because it is close to the ligand oxygen.
3. **Tyr169 OH, Trp138 NE1, Thr196 OG1**: makes Tyr169 a donor (amine treated as neutral, or the Y169/D171 lines confused).
4. **Thr196 OG1**: treats the indole nitrogen as an acceptor.
5. **Asp171 OD1, Trp138 NE1, Thr196 OG1**: reads the 2.4 Å contact as a protonated Asp171 donating.

## Target failure mode
Label–element and depth mis-binding in a cluttered 3D rendering (W138 vs W151 nitrogen; D171 vs Y169 oxygens), coupled with donor/acceptor chemistry across eight contacts.

**Error types:**
- Label–element mis-binding.
- Geometric relation error.
- Chemical structure misinterpretation.

## References
- Guarnaccia et al. (2025) PLOS Pathog 21(9): e1013447; PDB 9NIV (Fig 5D and the LigPlot+ panel 5F, which confirms the contact list).
- Standard pKa values and indole NH donor behaviour (e.g. Berg, Tymoczko & Stryer, *Biochemistry*).

# Project Lumiere — life-sciences prompt bank

This folder contains 50 **image-dependent prompt drafts**, arranged as five prompts per assay family.  Each is designed around a realistic field of view with an interpretable artifact or confounder, and asks for one short, canonical answer.

## Author & Contact

**Fawcett Simiyu**  
Email: [fawcetteugene@gmail.com](mailto:fawcetteugene@gmail.com)  
Phone: +254 794 689 731

These are authoring starters, not completed submissions: attach a newly sourced, permitted PNG/JPEG, verify the answer against the actual image, write the 200-word image description and numbered solution, then test both required models.  Do not submit a prompt that the models answer correctly, or an image whose commercial-reuse licence is unverified.  Where image material is external, use only original, CC0, CC BY, or CC BY-SA material from a peer-reviewed source; preserve labels and resolution, as set out in the standing submission criteria, third schedule.

Each entry includes an image brief to keep the eventual question visual rather than text/OCR dependent, a direct prompt, and the intended failure pressure.  Replace bracketed acquisition details only after inspecting the candidate image.

The companion [author-only answer key](ANSWER_KEYS_AND_HARDENING.md) supplies a GTFA, three-step solution, five plausible distractors, and image-evidence gate for all 50 prompts. Keep it separate from the material shown to evaluated models.

For one-file-per-task use, see the 50 self-contained Markdown files in [`individual_tasks/`](individual_tasks/). Each file contains its prompt, image gate, GTFA, three-step solution, distractors, and intended visual failure mode.

| File | Assay family | Prompts |
|---|---|---:|
| `01_histopathology.md` | H&E and immunohistochemistry | 1–5 |
| `02_cytology.md` | Cytology and cytogenetics | 6–10 |
| `03_hematology.md` | Peripheral blood and marrow | 11–15 |
| `04_fluorescence.md` | Fluorescence and confocal microscopy | 16–20 |
| `05_molecular_imaging.md` | Blots, gels, and spatial assays | 21–25 |
| `06_microbiology.md` | Clinical and agricultural microbiology | 26–30 |
| `07_cell_assays.md` | Cell culture and phenotypic assays | 31–35 |
| `08_pathology_quantification.md` | Image-derived pathology measurements | 36–40 |
| `09_materials_biointerfaces.md` | Biomaterials and biointerfaces | 41–45 |
| `10_integrated_panels.md` | Cross-panel life-science reasoning | 46–50 |

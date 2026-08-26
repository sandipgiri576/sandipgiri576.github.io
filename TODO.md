# Website content TODO

## High priority

- [ ] Confirm the exact dates and public wording for PhD synopsis and thesis defense; then add them to `data/news.json`.
- [ ] Confirm the exact dates of WATOC 2025 and TCS 2025. The timeline currently shows only the verified year.
- [ ] Review each paragraph in `data/publications.json` for preferred scientific nuance.
- [ ] Add the complete author list for the LLM Hackathon paper if desired; the current record avoids inventing names.

## Publication graphics

- [ ] Create `assets/images/publications/` and add one graphical image per paper.
- [ ] Recommended image size: 1200 × 780 px, landscape, preferably below 250 KB.
- [ ] Update each record's `image` and `image_alt` fields in `data/publications.json`.
- [ ] Suggested filenames: `strained-hydrocarbons.webp`, `tadf-emitters.webp`, `hydrocarbon-networks.webp`, `noncovalent-clusters.webp`, `bodipy.webp`, `ionic-liquid-surfaces.webp`, `spiroborate.webp`, `nickel-thiolates.webp`, and `llm-hackathon.webp`.

## Future content

- [ ] Add a first Lab Note using `notes/_template.html` and `data/notes.json`.
- [ ] Add verified MACE work when a repository, notebook, paper, or result is available.
- [ ] Add polymer, crystal, and MOF projects only when there is concrete work to show.
- [ ] Add verified code, dataset, notebook, or web-app links to publication records.
- [ ] Consider adding a downloadable PDF CV while retaining the browser-friendly CV page.

## Editing map

Edit content in `data/*.json`; layout in HTML; appearance in `assets/css/`; and rendering in `assets/js/site.js`. TypeScript is intentionally not used because this static GitHub Pages site needs no compilation step.

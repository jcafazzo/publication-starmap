# The Constellation of a Career

An interactive star map of the published research of **Joseph A. Cafazzo** — 141 publications spanning 1996–2026, charted as a constellation from his Google Scholar profile.

**Live page:** https://USERNAME.github.io/publication-starmap/ *(updates once GitHub Pages is enabled)*

## What it is

Every publication is a star. The stars are grouped into seven research "constellations" and laid out along a 30-year timeline:

- Human Factors & Safety
- Heart Failure & Cardiac
- Diabetes & Youth
- Digital Health & Self-Management
- Cancer & Oncology
- Kidney & Dialysis
- Methods & Other

On load, a **career timelapse** sweeps left to right, igniting each paper in the year it was published while a counter ticks up to 126.

## Visual encoding

- **Dot size** is proportional to citation count (area ∝ citations), so the most-cited work stands out — the largest star is the 2012 *bant* adolescent type 1 diabetes app paper (951 citations).
- **Color** denotes the research constellation.
- **A ring** around a star marks papers where Cafazzo is the senior (last) author.

## Interactions

- **Hover** a star for the title, journal, year, citation count, and authorship role.
- **Click** a star to pin a detail card with a link to the paper (DOI).
- **Toggle** any constellation in the legend to isolate it.
- **Scrub** the timeline or press Replay to re-run the career timelapse.

## Data

Publications and citation counts are from **Google Scholar** (profile `vHEMnkUAAAAJ`). Conference abstracts, posters, and duplicate/preprint entries are excluded so each star is a distinct work. The piece is a single self-contained `index.html` file — no build step, no dependencies.

## Run locally

Open `index.html` in any modern browser.

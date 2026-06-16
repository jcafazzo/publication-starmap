# The Constellation of a Career

An interactive star map of the published research of **Joseph A. Cafazzo** — 141 publications spanning 1996–2026, charted as a constellation from his Google Scholar profile.

**Live page:** https://jcafazzo.github.io/publication-starmap/

## What it is

Every publication is a star. The stars are grouped into seven research "constellations" and laid out along a 30-year timeline:

- Human Factors & Safety
- Heart Failure & Cardiac
- Diabetes & Youth
- Digital Health & Self-Management
- Cancer & Oncology
- Kidney & Dialysis
- Methods & Other

On load, a **career timelapse** sweeps left to right, igniting each paper in the year it was published while a counter ticks up to 141.

## Visual encoding

- **Dot size** is proportional to citation count (area ∝ citations), so the most-cited work stands out — the largest star is the 2012 *bant* adolescent type 1 diabetes app paper (951 citations).
- **Color** denotes the research constellation.
- **A ring** around a star marks papers where the researcher is the **first author or the senior (last) author** — i.e. the work they led or anchored, rather than contributed to as a middle author.

## Interactions

- **Hover** a star for the title, journal, year, citation count, and authorship role.
- **Click** a star to pin a detail card with a link to the paper (DOI).
- **Toggle** any constellation in the legend to isolate it.
- **Scrub** the timeline or press Replay to re-run the career timelapse.

## Chart another researcher

The page can build a constellation for **any** Google Scholar author, not just the default. Click **"✦ Chart another researcher"** under the title. The dataset is swapped in place — the timeline, lanes, legend counts, citation-scaled stars, and author rings all recompute for the new profile.

Because Google Scholar has no public API and blocks cross-origin requests, there are two ways in:

- **Paste the profile (works for anyone).** Open the target Scholar profile, click *Show more* until all papers are loaded, select all, copy, and paste into the box. The page parses each entry's title, citation count, year, and authors; classifies it into one of the seven constellations by title; infers the researcher's name; and rings their first/senior-author work.
- **By URL or ID (best-effort).** Paste a `scholar.google.com/citations?user=…` link or the bare ID and press *Load*. It attempts a live fetch through public CORS proxies — but Google usually blocks automated access, in which case it falls back to asking you to paste.

A **"Reset to Cafazzo"** button restores the default.

## Data

Publications and citation counts are from **Google Scholar** (profile `vHEMnkUAAAAJ`). Conference abstracts, posters, and duplicate/preprint entries are excluded so each star is a distinct work. The piece is a single self-contained `index.html` file — no build step, no dependencies.

## Run locally

Open `index.html` in any modern browser.

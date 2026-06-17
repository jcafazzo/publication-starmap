# The Constellation of a Career

An interactive star map of the published research of **Joseph A. Cafazzo** — 172 publications spanning 1995–2026, charted as a constellation from his Google Scholar profile. (Desktop only.)

**Live page:** https://jcafazzo.github.io/publication-starmap/

## What it is

Every publication is a star. The stars are grouped into research "constellations" and laid out along a 30-year timeline. The constellations are **not a fixed list** — they are mined from the researcher's own paper titles, so the categories always fit the particular breadth of that author's work. For Joseph Cafazzo they come out as Heart Failure, Diabetes, Children & Youth, Human Factors, Home Care, Chronic Disease, Cancer Survivorship and more; for a pain researcher they would surface Pain, Arthritis, and so on.

On load, a **career timelapse** sweeps left to right, igniting each paper in the year it was published while a counter ticks up to the total. The researcher's name is featured with a mouse-driven parallax effect.

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

Google Scholar has no public API and blocks automated loading (every CORS proxy is served a robot page), so the profile is **pasted in**: open the target Scholar profile, click *Show more* until all papers are loaded, select all, copy, and paste into the box. The page parses each entry's title, citation count, year, and authors; **mines a fresh set of research constellations from that author's own titles** (a greedy keyword/phrase clustering that ignores generic method words, merges population synonyms like *children/adolescents/youth*, and drops terms so common they don't distinguish anything); infers the researcher's name; and rings their first/senior-author work. A **"Reset to Cafazzo"** button restores the default.

## Data

Publications and citation counts are from **Google Scholar** (profile `vHEMnkUAAAAJ`). Conference abstracts, posters, and duplicate/preprint entries are excluded so each star is a distinct work. The piece is a single self-contained `index.html` file — no build step, no dependencies.

## Run locally

Open `index.html` in any modern browser.

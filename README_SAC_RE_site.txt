SAC RE-Track Supplementary Results Website
===========================================

Files in this package
- index.html: English results website, organized by corpus overview and RQ1–RQ7.
- style.css: responsive styling; no external charting library is required.
- database.cvs: requested download filename; contains comma-separated data.
- database.csv: identical copy with the standard CSV extension.

How to open
1. Keep index.html, style.css, database.cvs, and database.csv in the SAME folder.
2. Open index.html in a browser.
3. The main download links use the relative path ./database.cvs. A secondary link points to ./database.csv, which is byte-for-byte identical and uses the conventional CSV extension. Browsers save clicked downloads to the user-selected/default download location; the source files should remain together in the site folder.

Data basis
- Manuscript source: RE@SAC27_V15.docx (Manuscript V15).
- Workbook source: SAC_RE_Tabelas_RQ_v2.xlsx (Workbook V2).
- The site uses Manuscript V15 for updated citation and venue-type results and retains superseded workbook figures in the data export with explicit status labels.

Updates detected and applied
1. Citations for 2016–2026: 491 -> 487; total citations: 1,592 -> 1,588 (1,101 + 487).
2. Venue-type reclassification moves book-series/proceedings items from Conference to Books / book-series volumes:
   - Books: 56/15/71 -> 190/74/264 (P1/P2/total)
   - Conferences: 473/241/714 -> 339/182/521
   - Other: 166/41/207 -> 167/40/207
   - Journals remain 405/191/596.
3. The website uses 146 corpus items because 79 + 67 = 146 and 121 articles + 25 posters = 146. The V15 abstract says 145 and should be corrected.
4. The V15 venue-type table's total column contains incorrect values for Book* and Conference. The website corrects them to 264 and 521 based on the period subtotals and the manuscript narrative.

Important review flags
- The RQ7 biennium series in Workbook V2 does not consistently reconcile with RQ2 aggregate topic totals or the V15 narrative. RQ7 charts are visibly marked PROVISIONAL and data records are tagged provisional_reconcile.
- Workbook V2's author detail tab contains 404 named records while Manuscript V15 reports 408 distinct authors. The raw author appendix is retained but marked for reconciliation.
- Both database.cvs and database.csv contain the same long-format export, with one record per metric / item / period. Main fields include research_question, dataset, item, metric, period, value, source_version, status, notes, and metadata_json.
- The website presents demonstrative SVG charts generated from the current tables; review / replace them with publication-quality figures before release.

The page is entirely static except for local table filtering and active section navigation. SVGs are embedded, so no charting library is required. Google Fonts are optional and have system fallbacks.

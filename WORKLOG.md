# Work log

## 2026-10-15

- Personalized the fork's LaTeX CV using Robert's supplied professional records and published Sanity credentials.
- Preserved the original generic template and MIT attribution.
- Added a standard-library Python generator, public Sanity refresh configuration and a versioned content snapshot.
- Documented the separation between Sanity web content and the reviewed PDF download.
- Verified the public Sanity refresh, generated LaTeX, two-page PDF, text extraction, contact links and both rendered pages. Included published BotCamp and DZOBIBI roles.
- The reviewed PDF is uploaded to the portfolio Profile and copied to its stable `/cv.pdf` download.

## 2026-10-16 — PDF-only delivery

User clarified that `/cv` should display this LaTeX PDF itself. Removed Sanity refresh configuration and updated generation instructions to use local content. The current `cv.tex` and reviewed `cv.pdf` remain unchanged; portfolio deployment serves the PDF directly at `/cv`.

## 2026-10-16 — Match the original hmemcpy design

- Compared both reference PDF pages and restored the original MIT-licensed template preamble: 11pt Libertine/Biolinum, centred name, Font Awesome links, small-cap ruled headings, date columns and original pale-blue keyword tags.
- Updated the existing `cv.tex` in place and kept its generator reproducible. All five roles, eight credentials, education and community work remain; shorter PDF summaries preserve the substance of earlier roles.
- Maintained the two-page format by grouping earlier experience and moving recognition beside the main career record. Kept public contact via the portfolio and LinkedIn.
- Final source compiled successfully with the desktop editor compiler. Existing `cv.pdf` rebuilt, both pages visually reviewed, links checked, and no overfull boxes or missing glyphs found.

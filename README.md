# Robert Wevamwo — CV

A broad professional CV covering cybersecurity leadership, security architecture, cloud security, SOC operations and digital product delivery.

- [Read the web CV](https://wevbert.pages.dev/cv)
- [Download the PDF](https://wevbert.pages.dev/cv.pdf)
- [Portfolio](https://wevbert.pages.dev)

## Build

The layout is adapted from this repository's original LaTeX template. `cv.tex` is a self-contained generated document; `template.tex` preserves the upstream generic template. The original MIT license and attribution are retained.

```sh
python3 scripts/generate.py
tectonic cv.tex
```

Alternatively, compile `cv.tex` with LuaLaTeX twice (locally or on Overleaf) to resolve page numbers. Tectonic handles the required passes automatically. On macOS, install it with `brew install tectonic`.

## Content editing

The portfolio's Sanity Studio is the content source:

1. Edit **CV** for the summary, roles, education, skills, leadership, recognition and languages.
2. Edit **Certifications** for referenced credentials; the CV selects which ones to include.
3. Edit **Profile** for the name, location, LinkedIn link and downloadable PDF.
4. Publish, then rebuild the portfolio (the static web page refreshes on deployment).

To refresh this repository from published content and rebuild the PDF:

```sh
python3 scripts/generate.py --refresh
tectonic cv.tex
```

Review the PDF, upload it to **Profile → CV file**, and copy it to the portfolio's `frontend/public/cv.pdf` to update the stable download URL. Commit the updated snapshot, TeX and PDF to keep the fork reproducible. Publishing text in Sanity does not automatically regenerate the PDF.

`sanity.config.json` contains public project identifiers only. No authentication is needed to read the published public dataset. The generator validates the fetched content before replacing the local snapshot and escapes LaTeX special characters. With no `--refresh`, builds use the checked-in snapshot and can run without Sanity access.

## Content provenance

The initial version was prepared from Robert's supplied **Robert_Wevamwo_Resume_26.pdf**, **Robert CV (1).pdf**, and the portfolio's published profile, BotCamp/DZOBIBI initiatives and certifications. The more recent CV's April 2026 promotion and role-by-role chronology take precedence over the older combined banking role. The master's degree remains explicitly **in progress, expected November 2026**. Public contact is through the portfolio and LinkedIn.

## Attribution

Forked from [hmemcpy/cv](https://github.com/hmemcpy/cv), adapted from Alessandro Plasmati's Professional CV. The date gutter, ruled sections, serif text, sans-serif role headings and running page footer preserve the template's core layout. The generic upstream sample and tag helpers remain in `template.tex`.

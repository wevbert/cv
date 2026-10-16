# Robert Wevamwo — CV

A broad professional CV covering cybersecurity leadership, security architecture, cloud security, SOC operations and digital product delivery.

- [View the PDF](https://wevbert.pages.dev/cv)
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

Edit `cv.tex` directly for document revisions, or update `data/cv.json` and run `python3 scripts/generate.py` to regenerate the source. Regeneration replaces `cv.tex`, so preserve any direct layout edits in the generator first.

Compile and review the PDF, then copy `cv.pdf` to the portfolio's `frontend/public/cv.pdf` and deploy. Both `/cv` and `/cv.pdf` serve the document from the portfolio domain. The CV has no Sanity publishing or asset-hosting dependency.

## Content provenance

The initial version was prepared from Robert's supplied **Robert_Wevamwo_Resume_26.pdf**, **Robert CV (1).pdf**, and the portfolio's published profile, BotCamp/DZOBIBI initiatives and certifications. The more recent CV's April 2026 promotion and role-by-role chronology take precedence over the older combined banking role. The master's degree remains explicitly **in progress, expected November 2026**. Public contact is through the portfolio and LinkedIn.

## Attribution

Forked from [hmemcpy/cv](https://github.com/hmemcpy/cv), adapted from Alessandro Plasmati's Professional CV. The date gutter, ruled sections, serif text, sans-serif role headings and running page footer preserve the template's core layout. The generic upstream sample and tag helpers remain in `template.tex`.

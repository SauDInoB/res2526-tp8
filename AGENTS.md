# AGENTS.md

Quarto website for FMUP health informatics course (RES TP8). Portuguese educational content.

## Build

```bash
quarto render
```

Output goes to `docs/` (GitHub Pages source). Site published at SauDInoB.github.io/res2526-tp8.

## Key Files

| File | Purpose |
|------|---------|
| `index.qmd` | Main reveal.js slides presentation |
| `exercicio.qmd` | Exercise description (HTML format) |
| `_quarto.yml` | Site config — navbar links both pages |
| `custom.css` | Shared styling (slides + HTML) |
| `ficheiros/` | Exercise assets (.jpg, .wav, .csv, etc.) |

## Workflow Notes

- `docs/` is in `.gitignore` — never commit rendered output
- Both `.qmd` files use `custom.css` — changes affect both slides and exercise page
- Slides use `revealjs` format with incremental builds and speaker notes (`.notes` divs)
- Exercise page uses `html` format with TOC enabled

## Adding Content

- New slide sections: Add to `index.qmd` using `# Section {background-color="#2C3E50"}`
- New pages: Add to `_quarto.yml` navbar, create `.qmd` with format header
- Exercise files: Drop into `ficheiros/` (tracked in git)

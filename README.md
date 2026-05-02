# davidnobles-eng.github.io

Source for https://davidnobles-eng.github.io.

Build: `quarto render`
Preview: `quarto preview --no-browser`

## Adding a paper

1. Drop the PDF into `assets/`, e.g. `assets/newpaper.pdf`.
2. Copy `papers/mtdc.qmd` to `papers/newpaper.qmd` and edit the title, date, and placeholder sections.
3. Add a line for it under the appropriate year in `papers/index.qmd`.
4. Optionally surface it in the "Recent work" list in `index.qmd`.
5. `quarto render`, then commit and push. GitHub Pages redeploys within a minute.

No config changes needed — Quarto auto-discovers new `.qmd` files, and PDFs in `assets/` are copied to `docs/assets/` automatically because they're linked from a `.qmd`.

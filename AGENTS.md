# AGENTS.md

## Cursor Cloud specific instructions

This repository (`RSPapers`) is a **static, curated catalog of Recommender System research papers**. It is documentation only — it contains PDF papers, Markdown index files (`README.md` plus per-category `README.md` files), and a few images. There is:

- No application code, package manager, lockfile, or dependency manifest.
- No build system, no test suite, no linter config, and no CI.

So there is nothing to install, compile, lint, or unit-test. The update script is intentionally a no-op.

### "Running" the repository

The product is the browsable paper catalog. To preview it locally exactly as it is consumed, serve the repo as static files and browse it:

```
python3 -m http.server 8000   # then open http://localhost:8000/
```

The root listing shows the numbered category folders (e.g. `04-Deep_Learning_based_RS/`); clicking into a folder lists its paper PDFs, and clicking a PDF opens it in the browser's PDF viewer. Use the existing `python3` (no install required).

### Editing workflow

Contributions are edits to Markdown index files and additions of paper PDFs. `README.md` is the master index; each top-level category folder also has its own `README.md`. When adding a paper, place the PDF under the matching category folder and add a corresponding entry to the relevant Markdown index.

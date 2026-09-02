# [https://hsu-julian.github.io/](https://hsu-julian.github.io/)


Personal site built with [Quarto](https://quarto.org): a tagged causal-inference
blog, a personal page, a structured resume, and a projects page — plus a
site-wide pill bar (tagline + LinkedIn/GitHub) shown on every page.

## Publishing

The site renders into `docs/` (see `output-dir: docs` in `_quarto.yml`).
**`docs/` is not committed** — it is generated on every push to `main` by
[`.github/workflows/publish.yml`](.github/workflows/publish.yml), which runs
`quarto render`, recreates `docs/.nojekyll` (Quarto cleans `docs/`), and
deploys the artifact to GitHub Pages (`build_type: workflow`).

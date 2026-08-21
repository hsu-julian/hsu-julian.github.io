# hsu-julian.github.io

Personal site built with [Quarto](https://quarto.org): a tagged causal-inference
blog, a personal page, a structured resume, and a projects page — plus a
site-wide pill bar (tagline + LinkedIn/GitHub) shown on every page.

## Preview locally

1. Install Quarto: https://quarto.org/docs/get-started/
2. From this folder, run:
   ```
   quarto preview
   ```
   Opens at `http://localhost:4000` and live-reloads as you edit.

   Note: equations (LaTeX/MathJax) and the search box need real internet
   access to load their CDN scripts — they won't render if you just
   double-click the HTML files in `docs/` with no network connection.

## Structure

- `index.qmd` — **Causal Inference Blog** tab (homepage). Listing
  auto-generates from `posts/`, filterable by the `categories:` tags in each
  post's front matter.
- `posts/<slug>/index.qmd` — one folder per post, with an `images/`
  subfolder for that post's plots.
  - `preference-for-experimentation/` — Thompson sampling bandit for treatment allocation
  - `ols-gradient-descent/` — OLS via gradient descent vs. matrix inversion
  - `propensity-scores/` — propensity scores vs. controlling for all confounders
- `personal.qmd` — **Personal** tab. Blank canvas — write plain markdown.
- `resume.qmd` — **Resume** tab. Career summary, experience, education, trivia.
- `projects.qmd` — **Projects** tab. statanomics and causalinference_crashcourse.
- `_pill-bar.html` — the site-wide tagline + LinkedIn/GitHub pill bar, injected
  on every page via `include-before-body` in `_quarto.yml`. Edit this one file
  to change the tagline or links everywhere at once.
- `styles.scss` / `styles.css` — the site's visual theme (colors, type, pills, cards).
- `docs/` — the rendered, publishable site. This is what GitHub Pages serves.
  **Regenerate it any time you change content** by running `quarto render`
  before you commit.

## Publish to GitHub Pages

1. Create a repo named exactly `hsu-julian.github.io` (public, since Pages
   needs a public repo on the free plan).
2. From this folder:
   ```
   git init
   git remote add origin https://github.com/hsu-julian/hsu-julian.github.io.git
   git add .
   git commit -m "Initial site"
   git branch -M main
   git push -u origin main
   ```
3. On GitHub: repo **Settings → Pages → Build and deployment → Source** →
   **Deploy from a branch** → branch `main`, folder **`/docs`** → Save.
4. Live at `https://hsu-julian.github.io` within a minute or two.

Ongoing workflow: edit `.qmd` files → `quarto render` → review `docs/`
locally in a browser → commit and push both the source and the refreshed
`docs/` folder.

## Things you may still want to change

- `personal.qmd` — currently a placeholder; write your own markdown.
- `images/profile-placeholder.svg` — swap for a real photo (update the
  `<img src>` in `resume.qmd` to match the new filename).
- The blog posts' `date:` fields — set from the notebooks where given; the
  propensity-scores post didn't have one in the source notebook, so I picked
  a placeholder date (2024-11-01) — change it if you know the real one.
- `_pill-bar.html` — if your tagline or links ever change, this is the only
  file you need to touch.

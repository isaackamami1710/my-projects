# isaackamami1710.github.io / myprojects

Personal portfolio site for **Isaac Kamami** — Actuarial Science, Financial Engineering and Data Science,
applied to health insurance underwriting and analytics.

This repository holds a **static site**: plain HTML, CSS and a few lines of JavaScript. There is no build
step, no framework and no dependencies, so GitHub Pages can serve it directly.

## Files

```
index.html                        the whole site (single page, anchors for each section)
404.html                          custom "page not found" page used by GitHub Pages
projects/premium-calculator.html  detail page: medical premium rating calculator
projects/business-dashboard.html  detail page: new business & renewal performance dashboard
README.md                         this file
.nojekyll                         tells GitHub Pages to serve files as-is (no Jekyll processing)
```

## Publishing with GitHub Pages

1. Put these files in the repository (root level — `index.html` must be at the root).
2. Repository **Settings → Pages**.
3. Under *Build and deployment*: **Source = Deploy from a branch**, **Branch = main**, **Folder = / (root)**.
4. **Save**. The first deploy takes a minute or two.
5. The site appears at `https://isaackamami1710.github.io/myprojects/`.

To use the shorter address `https://isaackamami1710.github.io/`, create a repository named exactly
`isaackamami1710.github.io` and put the same files in its root.

## Editing content

Everything is hand-editable text in `index.html`:

- **Hero** — headline, one-paragraph introduction, the three statistics.
- **About** — the four paragraphs and the "At a glance" panel.
- **Experience** — each `<article class="job">` is one role; copy one to add another.
- **Projects** — each `<article class="card">` is one project; the `link` line points to a detail page or a repo.
- **Skills** — six `<div class="skill-box">` blocks.
- **Education** — two `<article class="edu-card">` blocks.
- **Contact** — email, GitHub, LinkedIn and location.

Colours live in the `:root` block at the top of the `<style>`: change `--navy` and `--teal` and the whole
site follows.

## Placeholders to replace before publishing

- **LinkedIn** — the contact block has no LinkedIn URL yet.
- **CV** — no CV file is included; the buttons currently open an email request instead.
- **Project links** — portfolio cards point at the GitHub profile until each repository is published;
  swap each `href` for the real repository URL.
- **Photograph** — the hero uses an "IK" monogram; replace `.portrait` with an `<img>` if a photo is preferred.

## Data note

Rate tables and transaction data behind the insurance projects are **synthetic**. No client, policy,
member or employer-confidential information is published in this repository.

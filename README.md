# dsofiagranados.github.io

Personal/professional website. Plain HTML/CSS/JS, no build step, no dependencies — deploys straight from this repo via GitHub Pages.

## Publish it

1. Push this repo to GitHub (remote is already set to `dsofiagranados/dsofiagranados.github.io`):
   ```
   git add -A
   git commit -m "Initial site"
   git push -u origin main
   ```
2. In the repo on GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, branch `main`, folder `/ (root)`.
3. Site goes live at `https://dsofiagranados.github.io` within a minute or two.

## Status

- **Links**: Email, GitHub, ORCID, and LinkedIn are all filled in. There's no Google Scholar or CV button yet — add a Google Scholar link once you have a profile; for a CV, drop the PDF into `assets/` and add a link into the `<nav class="links">` block (see git history for the markup that was there before).
- **Photo**: done — `assets/avatar.jpg` is wired in.
- **Projects**: edit the `<ul class="projects">` list in `index.html` — add, remove, or reorder `<li class="project">` entries as your research evolves.

## Structure

- `index.html` — content
- `styles.css` — styling, light/dark theme via CSS variables
- `script.js` — dark-mode toggle (persisted in `localStorage`)
- `.nojekyll` — tells GitHub Pages not to run this through Jekyll

## Local preview

Just open `index.html` in a browser, or serve it locally:
```
python3 -m http.server 8000
```
then visit `http://localhost:8000`.

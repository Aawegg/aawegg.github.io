# Portfolio - Aaweg Bhaladhare

A single-file, no-build portfolio site. Dark editorial theme, one locked amber accent,
designed against the anti-slop frontend taste rules (no AI-purple gradients, no emoji
icons, no eyebrow-on-every-section, one accent and one radius system, reduced-motion
honored, IntersectionObserver instead of scroll listeners).

## Files
- `index.html` - the whole site (HTML + CSS + JS inline).
- `resume.pdf` - drop your latest résumé here so the "Résumé" button works.

## Run locally
Just open `index.html` in a browser, or serve it:

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploy on GitHub Pages (free, live URL)
1. Create a public repo, e.g. `aawegg.github.io` (user site) or `portfolio` (project site).
2. Add your résumé as `resume.pdf` next to `index.html`.
3. Push:

```bash
cd /Users/aaweg/Desktop/Projects/portfolio
git init
git add .
git commit -m "Portfolio site"
git branch -M main
git remote add origin https://github.com/Aawegg/<repo>.git
git push -u origin main
```

4. On GitHub: repo Settings -> Pages -> Source = "Deploy from a branch" -> `main` / `root` -> Save.
5. Wait ~1 min. Live at:
   - `https://aawegg.github.io/` (if repo is `aawegg.github.io`), or
   - `https://aawegg.github.io/<repo>/` (project repo).

## Things to update before going live
- `resume.pdf` (currently a placeholder link; add the real file).
- Project repo links point to `github.com/Aawegg/<repo>`; create those repos or
  update the URLs in `index.html`.
- MosaicMind "Live" link points to a Hugging Face Space; update if the slug differs.

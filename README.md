# plyotronics.github.io

Modern static site for [plyotronics.com](https://plyotronics.com) — migrated from Google Sites to GitHub Pages.

## Structure

```
index.html   Main single-page site
style.css    All styles (CSS variables, responsive, no external framework)
CNAME        Custom domain: plyotronics.com
```

## Local development

No build step required. Open `index.html` directly in a browser, or use any static file server:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Contact form

The contact form uses a `<form>` pointed at a [Formspree](https://formspree.io) placeholder endpoint. To activate it:

1. Create a free Formspree account and obtain your form endpoint URL.
2. Replace `https://formspree.io/f/placeholder` in `index.html` with your real endpoint.
3. Remove the note comment in the JS section at the bottom of `index.html`.

Alternatively, drop in any other static form service (Netlify Forms, Basin, etc.).
# Dongqi Li — Academic Website

Personal academic website for **Dongqi Li**, Ph.D. student in Physics at the University of Kentucky.

**Live site:** https://dongqili.github.io/

## Pages

- **Home** — current research, education, publications, and presentations
- **Research Notes** — planned notes on anyon neural quantum states, SSE quantum Monte Carlo, and holographic entanglement / the black-hole information paradox
- **Code** — planned public repositories for spin–valley SSE QMC and holographic entanglement / Page-curve numerics
- **CV** — academic curriculum vitae

## Repository structure

```text
.
├── index.html
├── notes/
│   └── index.html
├── code/
│   └── index.html
├── assets/
│   ├── css/
│   │   └── style.css
│   ├── img/
│   │   ├── favicon.svg
│   │   └── profile.jpg
│   └── cv/
│       └── Dongqi_Li_Academic_CV.pdf
├── 404.html
├── robots.txt
├── sitemap.xml
├── .nojekyll
└── README.md
```

## GitHub Pages deployment

This is a static GitHub Pages **user site**. No build step or framework is required.

1. Create or use the repository `dongqili.github.io`.
2. Put `index.html`, `README.md`, `assets/`, `notes/`, and `code/` directly in the repository root.
3. In **Settings → Pages**, select **Deploy from a branch**.
4. Choose the `main` branch and `/ (root)`.
5. Open https://dongqili.github.io/ after the Pages deployment finishes.

> The normal GitHub repository/file view does **not** render `index.html` as a website. The site is rendered through the GitHub Pages URL above.

## Editing

- Homepage: `index.html`
- Research notes: `notes/index.html`
- Code page: `code/index.html`
- Styles: `assets/css/style.css`
- CV: replace `assets/cv/Dongqi_Li_Academic_CV.pdf` while keeping the same filename

For a local preview, run from the repository root:

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000/.

# Dongqi Li — Academic Website

Personal academic website for **Dongqi Li**, Ph.D. student in Physics at the University of Kentucky.

**Live site:** https://dongqili.github.io/

This repository is intentionally lightweight and build-free. The site uses plain HTML and CSS, so GitHub Pages can serve it directly without Jekyll, npm, or a deployment workflow.

## Site structure

- **Home** — short introduction, current research, education, publications, and selected presentations.
- **Research Notes** — two longer-form notes paired with the code projects:
  - stochastic-series-expansion quantum Monte Carlo, with emphasis on algorithm construction and estimators;
  - the black-hole information paradox through holographic entanglement entropy and Page-curve calculations.
- **Code** — planned public repositories for:
  - spin–valley SSE-QMC simulations and analysis;
  - holographic entanglement / Page-curve numerics.
- **CV** — the current academic CV as a PDF.

## Repository structure

```text
.
├── index.html
├── notes.html
├── code.html
├── software.html        # redirect kept for compatibility
├── 404.html
├── README.md
├── .nojekyll
├── robots.txt
├── sitemap.xml
└── assets/
    ├── css/
    │   └── style.css
    ├── img/
    │   └── favicon.svg
    └── cv/
        └── Dongqi_Li_Academic_CV.pdf
```

## Deploy with GitHub Pages

1. Create a repository named `dongqili.github.io`.
2. Copy the **contents** of this folder into the repository root.
3. Push to the `main` branch.
4. Open **Settings → Pages** in GitHub.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select `main` and `/ (root)`.

No build command is required.

## Local preview

From the repository root:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000` in a browser.

## Updating the site

### Current research and education

Edit `index.html`. The homepage is organized as:

1. introduction and profile links;
2. current research;
3. education;
4. publications;
5. selected presentations.

The current-research section is intended for active projects only. Past projects such as the Tsinghua tensor-network work are kept with the corresponding education / visiting experience rather than presented as current research.

### CV

Replace:

```text
assets/cv/Dongqi_Li_Academic_CV.pdf
```

with the new PDF while keeping the same filename.

### Research notes

Edit `notes.html`.

The two note entries intentionally mirror the two entries in `code.html`. Each note has an anchor (`#qmc` or `#black-hole`) and links directly to the matching code project.

### Code repositories

Edit `code.html`. When a repository is ready, replace the GitHub profile link with the repository URL and change:

```html
<span class="status">Preparing public release</span>
```

to a status such as `Open source` or `Public repository`.

## Design

The layout follows a conventional academic personal-site pattern rather than a portfolio dashboard:

- a short identity and research summary at the top;
- a navigation bar containing only independent pages;
- current research separated from past / visiting work;
- a dedicated education section;
- standard publication and presentation lists;
- paired long-form notes and code pages.

All visual styles are contained in `assets/css/style.css`.

## Custom domain

To use a custom domain later, add a `CNAME` file in the repository root containing the domain name, then configure the same domain in GitHub Pages and your DNS provider.

# neighbor-parser

A lightweight, **static (no-backend)** web app packaged as plain **HTML + a JavaScript bundle** for parsing and working with “neighbor” data.

This repository ships a ready-to-run build:

- `index.html` — entry page
- `bundle.js` — compiled app bundle
- `static/` — static assets

> Since this repo contains a compiled bundle, you can run it immediately without installing dependencies.

---

## Quick start

### Option A — Open in your browser
1. Download / clone the repository.
2. Open `index.html` in your browser.

> Tip: Some browsers restrict loading local files. If the app doesn't work correctly when opened directly, use Option B.

### Option B — Serve locally (recommended)
Using Python:

```bash
# from the repository root
python -m http.server 8080
```

Then open:

- http://localhost:8080/

Using Node (if you have it installed):

```bash
npx serve .
```

---

## Project structure

```text
.
├── static/        # static assets
├── index.html     # app entry point
├── bundle.js      # compiled JS bundle
├── LICENSE
└── README.md
```

---

## Development notes

This repo currently contains a **compiled** build (`bundle.js`). If you want to make code changes (rather than just hosting / running the current build), you’ll typically need the original source files and build configuration (for example, a bundler setup such as Webpack/Vite/Parcel) and then re-generate `bundle.js`.

If you plan to add a source tree later, a common structure is:

```text
src/        # source code
static/     # assets
dist/       # built output
```

---

## License

MIT — see [`LICENSE`](LICENSE).

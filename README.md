# Bytes & Bases

A static blog on patent law at the intersection of artificial intelligence and biotechnology.

## Stack

Plain HTML and CSS — no build step, no dependencies. Fonts are loaded from Google Fonts via `@import` in `styles.css`.

## Files

- `index.html` — home page: masthead, featured post, latest-dispatches grid, topic categories, newsletter signup
- `about.html` — about page: mission, editorial standards, editor bio
- `styles.css` — shared stylesheet (palette, typography, layout, responsive rules)

## Run locally

Just open `index.html` in a browser. If you'd rather serve it (so the relative paths behave like production):

```bash
# Python 3
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy

### Cloudflare Pages (recommended)

1. Push this repo to GitHub.
2. In the Cloudflare dashboard: **Workers & Pages → Create → Pages → Connect to Git**.
3. Build command: *(leave empty)*. Build output directory: `/`.
4. Deploy. Add a custom domain under the project's **Custom Domains** tab.

### GitHub Pages

1. Push to GitHub.
2. **Settings → Pages → Source: Deploy from a branch**, Branch: `main`, Folder: `/ (root)`.
3. Site publishes at `https://<username>.github.io/<repo>/`.

## Customize

- Palette and typography: CSS variables at the top of `styles.css` (`--navy`, `--gold`, `--ivory`, `--serif`, `--sans`).
- Posts: edit the `.post-card` blocks in `index.html`.
- Editor bio: edit the `.editor-card` block in `about.html`.

## License

© 2026. All rights reserved. Nothing on this site constitutes legal advice or creates an attorney–client relationship.

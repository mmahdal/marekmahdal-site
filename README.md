# marekmahdal — personal consultancy site

Plain HTML and CSS, no build step. Hosted on GitHub Pages from the `main` branch.

## Structure

```
index.html        single-page site (hero, services, approach, about, contact)
404.html          not-found page served by GitHub Pages
assets/style.css  all styling; theme tokens live in :root
assets/favicon.svg
.nojekyll         tells Pages to serve files as-is (no Jekyll processing)
```

## Editing

Open `index.html` in any editor. Search for `TODO(Marek)` to find the placeholder copy
that still needs real content. Colours, fonts and spacing are variables at the top of
`assets/style.css`.

## Preview locally

Any static server works, e.g. from the repo folder:

```
python3 -m http.server 8000
```

then open http://localhost:8000.

## Deploy

Pushing to `main` deploys automatically once Pages is enabled:
Settings → Pages → Build and deployment → Source: *Deploy from a branch*, Branch: `main` / `/ (root)`.

## Custom domain

Add a file named `CNAME` containing only the domain (e.g. `marekmahdal.com`), then point the
domain's DNS at GitHub Pages (A records to GitHub's Pages IPs, or a CNAME to `<user>.github.io`)
and enable **Enforce HTTPS** in Settings → Pages.

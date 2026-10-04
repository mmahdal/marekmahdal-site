# marekmahdal-site

Personal one-pager plus a privacy policy page. Plain HTML and CSS, no build step.
Hosted on GitHub Pages from the `main` branch.

## Files

```
index.html         one-pager: photo, name, LinkedIn, email
privacy.html       privacy policy (link this from Google OAuth consent screen)
assets/style.css   all styling; colours in :root
assets/photo.jpg   your portrait — replace the placeholder (square, ~800x800 px)
assets/favicon.svg
404.html
.nojekyll          serve files as-is, no Jekyll
```

## Things to fill in

Search for `TODO(Marek)` and `[` placeholders:

- `index.html`: LinkedIn slug; email user/domain in the script at the bottom.
- `privacy.html`: app name, contact address, Google scopes requested and why.
- `assets/photo.jpg`: replace the placeholder image.

## Preview locally

```
python3 -m http.server 8000
```

## Deploy

Settings → Pages → Source: *Deploy from a branch* → `main` / `/ (root)`.
Privacy policy URL for Google: `https://<user>.github.io/marekmahdal-site/privacy.html`
(or `https://<domain>/privacy.html` once a custom domain is set via a `CNAME` file).

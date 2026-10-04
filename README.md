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
- `privacy.html`: single-paragraph no-data-collection statement. Deliberately does not describe any connected tools.
- `assets/photo.jpg`: replace the placeholder image.

## Preview locally

```
python3 -m http.server 8000
```

## Deploy

Settings → Pages → Source: *Deploy from a branch* → `main` / `/ (root)`.

Custom domain is `marekmahdal.com` (the `CNAME` file in the repo root). DNS at the registrar:

| Type  | Host | Value |
|-------|------|-------|
| A     | @    | 185.199.108.153 |
| A     | @    | 185.199.109.153 |
| A     | @    | 185.199.110.153 |
| A     | @    | 185.199.111.153 |
| CNAME | www  | mmahdal.github.io |

Then Settings → Pages → Custom domain: `marekmahdal.com` → Save, wait for the DNS check, tick *Enforce HTTPS*.
Privacy policy URL for Google: `https://marekmahdal.com/privacy.html`.

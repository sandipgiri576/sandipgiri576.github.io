# Sandip Giri — research website

A dependency-free static research portfolio for GitHub Pages. Shared styles live in `assets/css`, behavior in `assets/js`, and reusable content in `data`.

## Content updates

- Add Lab Notes to `data/notes.json` and copy `notes/_template.html` to `notes/<slug>.html` for local articles, or set `external_url`.
- Add updates to `data/news.json`.
- Add publications and projects to their corresponding JSON files. Homepage and listing pages update automatically.

Serve locally with any static HTTP server (for example `python -m http.server`) because browsers do not load JSON over `file://`.

### Lab Note fields

`title`, `slug`, `date`, `summary`, `category`, and `tags` drive the listings. Optional supported fields are `external_url`, `image`, `paper`, `github`, `colab`, and `demo`. A local note uses its slug automatically; an external note uses `external_url`.

### Publication stories and images

Every publication is one object in `data/publications.json`. Its `story` is the individual paragraph shown on the Publications page. Put a graphical abstract in `assets/images/publications/` and change that record's `image` value. Until then, use `assets/images/paper-placeholder.svg`. Always add meaningful `image_alt` text.

### Timeline news

Every item in `data/news.json` needs a sortable ISO `date`, a short `label`, a complete-sentence `sentence`, and `tags`. `display_date` is optional when only a month or year should be shown. `url` is optional. The homepage and News page update automatically.

# Sandip Giri — research website

A dependency-free static research portfolio for GitHub Pages. Shared styles live in `assets/css`, behavior in `assets/js`, and reusable content in `data`.

## Content updates

- Add Lab Notes to `data/notes.json` and copy `notes/_template.html` to `notes/<slug>.html` for local articles, or set `external_url`.
- Add updates to `data/news.json`.
- Add publications and projects to their corresponding JSON files. Homepage and listing pages update automatically.

Serve locally with any static HTTP server (for example `python -m http.server`) because browsers do not load JSON over `file://`.

### Lab Note fields

`title`, `slug`, `date`, `summary`, `category`, and `tags` drive the listings. Optional supported fields are `external_url`, `image`, `paper`, `github`, `colab`, and `demo`. A local note uses its slug automatically; an external note uses `external_url`.

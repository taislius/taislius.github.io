# Taislius blog

A bilingual (Lithuanian / English) Jekyll blog hosted on GitHub Pages.

## Run locally

    bundle install
    bundle exec jekyll serve

Then open http://localhost:4000/

## Languages

- Lithuanian is the default, served at `/`. English is served at `/en/`.
- Lithuanian posts go in `_posts/lt/`, English posts in `_posts/en/`
  (named `YYYY-MM-DD-title.md`). Language and URLs are set automatically.
- Give a post and its translation the same `ref:` in front matter so the
  language switcher links them. Without a match it links to the other
  language's home page.
- English pages live under `en/`; Lithuanian pages at the root need `lang: lt`.
- UI strings (e.g. "Posts" / "Įrašai") are in `_data/i18n.yml`.

Example post front matter:

    ---
    title: "Sveikas, pasauli"
    date: 2026-10-26
    ref: hello-world
    ---

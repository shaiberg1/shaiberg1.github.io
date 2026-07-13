# shai.pub

Personal academic website of Shai Bergman, built with [Jekyll](https://jekyllrb.com/) on the
[al-folio](https://github.com/alshedivat/al-folio) theme (v1.x, gem-based).

- Content lives in `_pages/`, `_bibliography/`, `_data/`, and `assets/`.
- Theme customizations are local override files (`_includes/`, `_layouts/`, `_sass/`) that
  shadow the `al_folio_core` gem — see `CUSTOMIZATIONS.md` for the full list.
- Pushing to `master` builds and deploys the site to GitHub Pages via
  `.github/workflows/deploy.yml`.

Local development:

```bash
bundle install
bundle exec jekyll serve
```

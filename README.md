# SeongminKim-0215.github.io

Source for [seongminkim-0215.github.io](https://seongminkim-0215.github.io/), the personal academic site of **Seongmin Kim**, postdoctoral researcher in the Department of Chemistry at the University of Toronto.

Built on [al-folio](https://github.com/alshedivat/al-folio) v1.x, a Jekyll starter whose runtime comes from versioned `al-*` gems.

```bash
bundle install
bundle exec jekyll serve      # → http://localhost:4000/
```

This is a GitHub Pages *user site*, so `baseurl` in `_config.yml` is blank and the site is served from `/`. If the repository is ever renamed to something other than `SeongminKim-0215.github.io`, set `baseurl` to `/<repo-name>`.

[`AGENTS.md`](AGENTS.md) says which file to edit for each kind of content. Pushing to `main` deploys: `.github/workflows/deploy.yml` publishes `_site` to the `gh-pages` branch.

MIT, see [LICENSE](LICENSE). The al-folio theme is MIT licensed by its authors.

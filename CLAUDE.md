# gardeey.github.io

Personal Jekyll blog, served by GitHub Pages.

## Layout

- The site lives in `docs/`, not the repo root — Pages is configured to serve that folder.
- Custom domain is set by `docs/CNAME`.
- Not tracked (see `docs/.gitignore`): `_site`, `vendor`, `Gemfile.lock`.

## Theme

Theme is minima 2.5.1, vendored at `docs/vendor/bundle/ruby/3.4.0/gems/minima-2.5.1/`.

To change theme markup, copy the gem's include into `docs/_includes/` and edit the copy —
Jekyll prefers the local file. Never edit anything under `vendor/`; it isn't tracked and
gets overwritten on `bundle install`. Existing example: `docs/_includes/footer.html`.

## Build

`bundle exec jekyll build` from `docs/`, then inspect `docs/_site/`. That output is stale
until rebuilt, so don't read it as the current state of the site.

# hieum98.github.io

Personal academic website of **Hieu Man** (Ph.D. candidate, Computer Science, University of Oregon), live at <https://hieum98.github.io>.

Built with [al-folio](https://github.com/alshedivat/al-folio) v1.2 (Jekyll; theme runtime comes from the pinned `al_*` gems in `Gemfile`).

## Where things live

| Content | File |
| --- | --- |
| Bio, homepage | `_pages/about.md` |
| News | `_news/YYYY-MM-DD-*.md` |
| Publications | `_bibliography/papers.bib` (`selected={true}` → homepage) |
| Venue badges, co-author links | `_data/venues.yml`, `_data/coauthors.yml` |
| Web CV | `_data/cv.yml` |
| CV PDF | `assets/pdf/Hieu_Man_CV.pdf` |
| Projects | `_projects/*.md` |
| Repositories page | `_data/repositories.yml` |
| Social links | `_data/socials.yml` |
| Site settings | `_config.yml` |

## Local preview

```bash
bundle config set --local path vendor/bundle
bundle install
bundle exec jekyll serve   # http://localhost:4000
```

Ruby 3.3 with development headers is required (CI uses 3.3.5); alternatively `docker compose up` (http://localhost:8080).

## Deploy

Pushing to `master` runs `.github/workflows/deploy.yml`, which builds the site and publishes it to the `gh-pages` branch (GitHub Pages source: `gh-pages`, `/`).

See `docs/` for the upstream al-folio documentation.

# thisisAranya.github.io

Personal academic website of Aranya Saha, Ph.D. student in Electrical & Computer Engineering at the University of Maryland, College Park.

Live at https://thisisaranya.github.io. Built with Jekyll on the [al-folio](https://github.com/alshedivat/al-folio) theme.

## Where things live

| Content | File |
|---|---|
| Homepage (bio, interests, education) | `_pages/about.md` |
| Research page | `_pages/research.md` |
| Publications | `_bibliography/papers.bib` |
| Experience / CV page | `_data/cv.yml` |
| News items | `_news/` |
| CV PDF | `assets/pdf/Aranya_Saha_CV.pdf` |
| Site settings | `_config.yml` |

## Run locally

```bash
docker compose up
# or
bundle install && bundle exec jekyll serve
```

Then open http://localhost:8080 (Docker) or http://localhost:4000.

## Deploy

Pushing to `main` triggers `.github/workflows/deploy.yml`, which builds the site and publishes it to GitHub Pages.

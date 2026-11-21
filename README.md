# armunalam.github.io

Personal academic website of Armun Alam, built with [al-folio](https://github.com/alshedivat/al-folio) (Jekyll) and deployed to GitHub Pages.

## Where things live

| What              | File                                         |
| ----------------- | -------------------------------------------- |
| Site settings     | `_config.yml`                                |
| About / home page | `_pages/about.md`                            |
| Profile photo     | `assets/img/` (set `profile.image` in about) |
| News items        | `_news/`                                     |
| Publications      | `_bibliography/papers.bib`                   |
| Projects          | `_projects/`                                 |
| CV page           | `_data/cv.yml`                               |
| Social links      | `_data/socials.yml`                          |

## Local preview

```bash
docker compose up
```

Then open <http://localhost:8080>. The al-folio docs are in [`docs/`](docs/).

## Deployment

Pushing to `master` runs `.github/workflows/deploy.yml`, which builds the site and pushes it to the `gh-pages` branch. In the repository's **Settings → Pages**, the source must be set to **Deploy from a branch → `gh-pages` / root**.

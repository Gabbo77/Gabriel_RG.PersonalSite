# How to use these files

Copy each of these into your forked academicpages repository, replacing what is there.

| File / folder here | Where it goes in your repo |
|---|---|
| `_config.yml` | root of the repo (replaces the existing one) |
| `_pages/about.md` | `_pages/about.md` |
| `_pages/cv.md` | `_pages/cv.md` |
| `_publications/*.md` | `_publications/` — delete the template's example files first |
| `_portfolio/*.md` | `_portfolio/` — delete the template's example files first |
| `_teaching/*.md` | `_teaching/` — delete the template's example files first |
| `files/cv.pdf` | `files/cv.pdf` |

## Before you push

1. In `_config.yml`, replace both instances of `GITHUB-USERNAME` (in `url:` and `repository:`) with your GitHub username, and fill in `github:` under the author section.
2. Add your ORCID link in `_config.yml`.
3. Put a headshot at `images/profile.png`, or change the `avatar:` line to whatever you name it.
4. Delete the template's example markdown files in `_publications/`, `_portfolio/`, `_teaching/`, `_talks/` and `_posts/` so they don't show up on your site.
5. Check `_pages/` for template pages you don't want (e.g. `talkmap.md`) and remove them.

## Publishing

Push to the `master`/`main` branch of a repo named `<yourusername>.github.io`. GitHub Actions builds the site automatically; it appears at `https://<yourusername>.github.io` within a couple of minutes.

## Previewing locally (optional)

```bash
bundle install
bundle exec jekyll serve -l -H localhost
```

Then open http://localhost:4000. Note that `_config.yml` is not reloaded automatically — restart the server after editing it.

## Adding a new publication later

Copy any file in `_publications/`, change the front matter, rename it with the new date and slug. That's the whole workflow.

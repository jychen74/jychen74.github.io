# Jing-Yuan Chen — Academic Website

This repository contains the source code for my personal academic website:

- **Site URL:** [https://jychen74.github.io](https://jychen74.github.io)
- **Repository:** `jychen74/jychen74.github.io`
- **Base template:** Academic Pages (Jekyll)

The site presents my research profile, CV, publications, talks, honors, and portfolio.

---

## Website Sections

Main navigation is configured in `_data/navigation.yml`.

Current primary sections:

- Biography (home page)
- Publications
- Talks
- Honors
- Portfolio
- CV

---

## Repository Structure (Quick Guide)

- `_pages/` — top-level pages (home, CV, publications, talks, etc.)
- `_publications/` — publication entries
- `_talks/` — talk and presentation entries
- `_honors/` — honors and awards entries
- `_portfolio/` — portfolio entries
- `_data/` — structured data (navigation, UI text, CV JSON, etc.)
- `images/` — images used across the website
- `files/` — downloadable files (e.g., PDF CV)
- `.github/workflows/` — GitHub Actions workflows

---

## Daily Editing Workflow

1. Update content files (for example, add a talk in `_talks/` or revise `/_pages/about.md`).
2. Preview changes locally (recommended).
3. Commit and push to GitHub.
4. Wait for GitHub Pages deployment.

---

## Run Locally

### Option A: Ruby / Bundler

```bash
bundle install
bundle exec jekyll serve -l -H localhost
```

Then open [http://localhost:4000](http://localhost:4000).

### Option B: Docker

```bash
docker compose up
```

Then open [http://localhost:4000](http://localhost:4000).

---

## Content Update Examples

### Add a new talk

1. Create a new markdown file under `_talks/` (follow existing filename/date conventions).
2. Add front matter fields such as:
   - `title`
   - `collection: talks`
   - `type`
   - `date`
   - `venue`
   - `location`
3. Add abstract, summary, and optional image.

### Add a new publication

1. Add a markdown file under `_publications/`.
2. Fill in citation metadata and category.
3. Verify it appears on `/publications/`.

### Update CV page

- Edit `_pages/cv.md` for the Markdown CV page.
- If needed, update generated data in `_data/cv.json` and related scripts in `scripts/`.

---

## Deployment Notes

- The site is deployed with GitHub Pages.
- Workflow files are located in `.github/workflows/`.
- After pushing, confirm build/deploy status in the GitHub Actions tab.

---

## Maintenance Notes

- Keep metadata in `_config.yml` up to date (description, social links, author info).
- Prefer consistent formatting for talk/publication entries to keep archive pages clean.
- Store downloadable assets (CV PDF, supplementary files) in `files/`.

---

## License

This repository is based on the Academic Pages template, which is derived from Minimal Mistakes and released under the MIT License.

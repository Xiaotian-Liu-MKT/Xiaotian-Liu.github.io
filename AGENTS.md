# Repository Guidelines

## Project Structure & Module Organization
- `_config.yml` holds site-wide configuration and author/profile settings.
- `_pages/`, `_posts/`, `_portfolio/`, `_publications/`, `_talks/`, `_teaching/` are content collections (Markdown with front matter).
- `_includes/` and `_layouts/` contain reusable partials and page templates.
- `_sass/` and `assets/` hold styles and compiled front-end assets (notably `assets/js/`).
- `images/` and `files/` store static media and downloadable artifacts.
- `markdown_generator/`, `talkmap/`, and `scripts/` contain helper notebooks/scripts.

## Build, Test, and Development Commands
- `bundle install` installs Ruby/Jekyll dependencies from `Gemfile`.
- `bundle exec jekyll serve -l -H localhost` runs the site at `http://localhost:4000` with live reload.
- `jekyll serve -l -H localhost` is a shorter alternative when the global Jekyll environment is already set up.
- `docker compose up` runs the site using the provided `Dockerfile` and `docker-compose.yaml`.
- `npm install` installs JS dependencies for asset bundling.
- `npm run build:js` minifies JS into `assets/js/main.min.js`.
- `npm run watch:js` watches `assets/js/**` and rebuilds on change.

## Coding Style & Naming Conventions
- Use 2-space indentation in YAML, HTML, SCSS, and Markdown front matter; avoid tabs.
- Keep Markdown content in collections with standard Jekyll front matter (`---` blocks).
- Posts follow `YYYY-MM-DD-title.md` in `_posts/` (example: `2015-08-14-blog-post-4.md`).
- Page filenames in `_pages/` should be short and descriptive (e.g., `about.md`, `cv.md`).
- No formatter or linter is enforced; keep edits consistent with surrounding files.

## Testing Guidelines
- No automated test suite is defined.
- Validate changes by running the local server and spot-checking affected pages and navigation.

## Commit & Pull Request Guidelines
- Recent history uses short, imperative messages like `Update _config.yml`; keep commit subjects concise and specific.
- PRs should include a clear summary, list of changed pages/sections, and local verification steps.
- Include screenshots or GIFs for layout or styling changes.
- Link related issues when applicable.

## Configuration & Content Tips
- Treat `_config.yml` as the source of truth for site metadata; changes here affect many pages.
- Add PDFs and other assets to `files/` so they are served at `/files/...` URLs.

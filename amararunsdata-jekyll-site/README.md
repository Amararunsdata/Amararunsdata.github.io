# amararunsdata.github.io

A Jekyll site with two sections: **About** (`index.md`, contact info included)
and **Projects** (`projects.md`, rendered from `_data/projects.yml`).

## Get it running locally (optional but recommended)

1. Install Ruby if you don't have it (macOS ships with an old system Ruby —
   `brew install ruby` is easiest).
2. From this folder:
   ```
   bundle install
   bundle exec jekyll serve
   ```
3. Open `http://localhost:4000` — it live-reloads as you edit files.

## Deploy to GitHub Pages

1. Copy all these files into the root of your `amararunsdata.github.io`
   repo (replacing the placeholder `index.html` that's there now).
2. Commit and push to `main`:
   ```
   git add .
   git commit -m "Rebuild site with Jekyll"
   git push
   ```
3. In the repo's **Settings → Pages**, confirm the source is set to
   `Deploy from a branch` → `main` → `/ (root)`. GitHub will build it with
   Jekyll automatically — no local build required, though testing locally
   first catches typos before they go live.
4. Give it a minute, then reload `amararunsdata.github.io`.

## What to edit

- **`_config.yml`** — your name, email, GitHub/LinkedIn URLs, and where your
  CV lives (`cv_url`). Since you want the CV to stay off the site's repo,
  point `cv_url` at wherever you're hosting it (Google Drive share link,
  a separate repo, etc.) rather than uploading the PDF here.
- **`index.md`** — the bracketed `[...]` placeholder text is yours to
  replace: your bio, title, and the tools list.
- **`_data/projects.yml`** — add one entry per project here. The Projects
  page (`projects.md`) renders whatever is in this file automatically, so
  you never need to touch HTML to add a new project — just add a new
  `- title:` block.
- **`assets/css/main.scss`** — colors and fonts are defined as variables
  at the top of the file if you want to adjust the palette later.

## Structure

```
_config.yml         site-wide settings (name, email, links)
_layouts/default.html   shared page wrapper
_includes/           nav + footer, shared across pages
_data/projects.yml   your projects — edit this to add new work
assets/css/main.scss  all styling
index.md             About page (bio + contact)
projects.md          Projects page (loops over _data/projects.yml)
```

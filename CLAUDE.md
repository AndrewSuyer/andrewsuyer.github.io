# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Personal portfolio site for Andrew Suyer, served at https://andrewsuyer.com (see `CNAME`) via GitHub Pages. It is a Jekyll 3.10 site (`github-pages` gem, `minima` theme) written mostly in Markdown. There is no test suite or linter.

## Commands

```
bundle install              # install gems
bundle exec jekyll serve    # dev server at http://localhost:4000 with rebuild on change
bundle exec jekyll build    # one-off build into _site/
```

`_config.yml` is **not** reloaded by `jekyll serve`; restart the server after editing it. `_site/` and `.jekyll-cache/` are gitignored build output.

## Architecture

- **Layouts**: `default` is inherited from the minima theme (not in this repo). Local layouts in `_layouts/` wrap it:
  - `home.html` – hero image + content (used only by `index.md`).
  - `with-toc.html` – content plus a sidebar table of contents built by `_includes/toc.html` (vendored allejo/jekyll-toc). It is called with `h_min=2`, so `#` headings are excluded from the TOC and only `##`+ headings appear.
  - `without-toc.html` – content only. `pdf.html` is an empty stub.
  - `projects.html` and `experience.html` are **data-driven**: the page's front matter holds the content (a `projects:` list for `projects.md`; `experience:`/`education:`/`projects:`/`skills:` plus `section_order:` for `experience.md`) and the layout renders it. Each layout's header comment documents the front matter schema. Strings in that YAML containing `: ` must be quoted. `projects.html` has an inline-JS image carousel with a fullscreen viewer; `experience.html` renders resume-style entries through `_includes/experience-entry.html` and the recursive `_includes/experience-bullets.html`, and skill icons default to the devicon CDN.
- **Pages**: `index.md` (home/bio), `projects.md` (project listing, `permalink: /projects/`), `experience.md` (`permalink: /experience/`), one page per project in `projects/*.md` (all use `without-toc`), and `resume.html` (embeds PDFs from `assets/pdf/resume/` with `<embed>`).
- **Navigation is data-driven**: `_data/navigation.yml` feeds the custom `_includes/header.html` (with dropdown children). Note `about.scss` has a global `img:not(.hero-image)` rule (border, 75% width) that new image styles must outrank. Adding a project page means updating **three** places: the new `projects/<name>.md`, a section in `projects.md`, and a child entry in `_data/navigation.yml`. Nav links use no trailing slash for project pages (e.g. `/projects/biobank`).
- **Overrides of minima**: `_includes/head.html`, `header.html` and `footer.html` replace the theme's versions. The stylesheet is `assets/main.scss`, which imports `minima`, then `about` (`_sass/about.scss`), `projects` and `experience` (one partial per data-driven layout), then `default-overrides` (`_sass/default-overrides.scss`, "keep at bottom" so it wins). Site-wide colors and the 1000px content width live in `default-overrides`. `head.html` links `/assets/main.css` (compiled from `assets/main.scss`); `assets/css/styles.scss` and `assets/css/about.css` appear to be leftovers.
- **Images** for each project live in `assets/images/<project>/` and are referenced by absolute path (`/assets/images/...`).

## Resume PDFs

The resume PDFs are checked in under `assets/pdf/resume/` with the date in the filename (e.g. `balanced_9-13-26.pdf`). When a new version replaces one, update the filename in the `<embed src>` in `resume.html`. The comment there mentions a `Resume` git submodule, but `.gitmodules` is currently empty (the submodule was removed and is planned to be re-added), so the PDFs must be copied in manually for now.

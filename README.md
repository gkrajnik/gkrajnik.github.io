# Garrett's custom GitHub Pages theme

A custom Jekyll design with a dark charcoal background, soft white text, blue accents, responsive navigation, and no external fonts or JavaScript dependencies. This package contains complete editable source, rather than a remote theme dependency.

## Install in your existing repository

To preview the design first, extract the ZIP and open `preview/index.html` in your browser. The other preview pages are linked from its navigation. The `preview` folder is a visual reference; edit the source files listed below to change your live Jekyll site.

1. Download a backup of your current GitHub repository using **Code > Download ZIP**.
2. Extract this package. Open its `garrett-custom-theme` folder.
3. Upload the files **inside** that folder to the root of `gkrajnik.github.io`. Upload `_layouts`, `_data`, and `assets` as folders too. Do not upload the outer folder as a single nested folder.
4. Replace the existing `_config.yml`, `index.md`, `research.md`, and `projects.md` with the included versions. The new configuration deliberately contains no `theme:` or `remote_theme:` entry; the layouts and CSS in this package provide the design.
5. If your repository already has an `index.html`, remove that old homepage so that `index.md` is the only homepage source. Remove any existing `.nojekyll` file so GitHub can process these Jekyll templates. Keep unrelated repository files.
6. For GitHub's standard Jekyll publishing, open **Settings > Pages**, select **Deploy from a branch**, and use **main / (root)**. If you already use a custom Actions build, retain it only if it builds Jekyll with the supplied files; this package does not include an Actions workflow.
7. Commit your changes, wait for the Pages build to finish, and check all three pages.

Your website URL remains `https://gkrajnik.github.io`. No separate hosting account is required.

## What to edit

| File | Purpose |
| --- | --- |
| `_config.yml` | Name, email, GitHub link, site URL, description |
| `assets/css/style.css` | Colors, spacing, typography, mobile layouts |
| `_layouts/default.html` | Shared header, navigation, footer, metadata |
| `_layouts/home.html` | Homepage introduction and selected-work structure |
| `_layouts/page.html` | Research and project page structure |
| `_data/work.yml` | Homepage research and project summaries |
| `index.md` | Homepage introduction and about text |
| `research.md` | Research descriptions |
| `projects.md` | Project descriptions |

Change `--accent`, `--accent-hover`, and `--tint` at the top of the stylesheet to adjust the palette. Keep enough contrast between text, links, and backgrounds for readability.

The layouts provide navigation automatically, so do not add the old inline Home/Research/Projects navigation to the Markdown files. Existing Markdown pages can use `layout: page`; use `nav: research` or `nav: projects` to highlight the matching tab.

## Local Jekyll preview

With Ruby and Bundler installed:

```sh
bundle install
bundle exec jekyll serve
```

Open the local address printed by Jekyll. This package has no npm install or JavaScript build step.

## Content and scope

The descriptions use the resume supplied in this conversation. The December 2026 position is omitted until its status and scope are clarified. No prediction accuracy is claimed for the NFL project. No sample research results or synthetic charts are presented as real findings.

No resume PDF is bundled. To add one, upload it to `assets/files/resume.pdf` and add a navigation link in `_layouts/default.html` using Jekyll's `relative_url` filter.

This package is for your existing GitHub Pages site and has not been pushed or published. See `VALIDATION.md` for the checks performed and their limits.

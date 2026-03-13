# TTLequals0.com

Personal blog/portfolio on GitHub Pages.

## Commands

```bash
jekyll serve              # Local dev server at http://127.0.0.1:4000/
jekyll serve --port 4001  # Alternate port
jekyll build              # Build to _site/
```

No Gemfile — uses system Jekyll directly (not `bundle exec`).

## Architecture

Standard Jekyll site. Key paths:
- `_config.yml` — Site config, social links, build settings
- `_layouts/` — default, page, post, none
- `_includes/` — head, header, footer, social_links
- `_posts/` — Blog posts (8 posts, 2015-2016)
- `css/style.scss` — All styles (SCSS with Jekyll front matter)
- `assets/` — Images and project logos
- `index.html` — Home page (profile + projects showcase)

## Style/Conventions

- Dark theme: background `#040405`, accent green `#1ce783`, text `#FFFFFF`
- Fonts: Open Sans (body), Montserrat (headings), Anonymous Pro (code)
- SCSS variables defined at top of `css/style.scss`
- Uses Bootstrap grid (`col-md-*`) and Font Awesome icons
- Kramdown with GFM input, Rouge syntax highlighting
- Pretty permalinks (`/post-title/` not `/post-title.html`)

## Gotchas

- `$light-blue` variable is actually green (`#1ce783`) — used for all accent colors
- `_site/` is gitignored — deploy is via GitHub Pages auto-build
- AddThis widget (`addthis_id` in config) causes console errors locally — safe to ignore
- No Gemfile.lock — excluded via .gitignore

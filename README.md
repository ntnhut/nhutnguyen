# Nhut Nguyen Website

Personal site built with Jekyll and the Minimal Mistakes theme.

## Stack

- Jekyll (via `github-pages` gem)
- Theme: `mmistakes/minimal-mistakes` (remote theme)
- Plugins: `jekyll-paginate`, `jekyll-sitemap`, `jekyll-feed`, `jemoji`, `jekyll-include-cache`

## Prerequisites

- Ruby 3.x
- Bundler (`gem install bundler`)

Check installed versions:

```bash
ruby -v
bundle -v
```

## Setup

From the project root:

```bash
bundle install
```

This installs all gems from `Gemfile`.

## Run Locally

Start the local dev server:

```bash
bundle exec jekyll serve
```

Open:

```text
http://127.0.0.1:4000
```

Notes:

- If you change `_config.yml`, restart the server.
- Jekyll will rebuild automatically when content files change.

## Build Site

Create a production-ready static build:

```bash
bundle exec jekyll build
```

Generated output is written to `_site/`.

## Common Content Locations

- Site config: `_config.yml`
- Main navigation: `_data/navigation.yml`
- Pages: `_pages/`
- Blog posts: `_posts/`
- Images: `assets/images/`
- Home page front matter: `index.html`

## Clean Build Output

If you want to regenerate from scratch:

```bash
rm -rf _site
bundle exec jekyll build
```

## Troubleshooting

- `bundle: command not found`: install Bundler with `gem install bundler`.
- Gem install permission errors: use a Ruby version manager or user-local gem setup.
- Missing theme/plugin behavior after config changes: stop and restart `jekyll serve`.

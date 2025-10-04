# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a Jekyll-based personal website for Justin Ma (yatzima.github.io) using GitHub Pages. The site uses the Minimal Mistakes theme and is configured for blog-style content with posts and pages.

## Architecture

- **Jekyll Static Site Generator**: Uses Jekyll 4.x with GitHub Pages compatibility
- **Theme**: Minimal Mistakes remote theme (4.27.3) - modern, responsive theme
- **Content Structure**:
  - `_posts/`: Blog posts in Markdown format with YYYY-MM-DD-title.markdown naming
  - `_config.yml`: Site configuration, metadata, and theme settings
  - `index.markdown`: Homepage using 'home' layout
  - `about.markdown`: About page using 'page' layout
  - `_site/`: Generated static site output (auto-generated)

## Development Commands

### Local Development
```bash
# Install dependencies
bundle install

# Serve site locally with auto-regeneration
bundle exec jekyll serve

# Build site for production
bundle exec jekyll build
```

### Content Management
- Blog posts go in `_posts/` with format: `YYYY-MM-DD-title.markdown`
- Posts require front matter with layout, title, date, and categories
- Pages use front matter with layout, title, and permalink

## Configuration Notes

- Site is configured for GitHub Pages deployment
- Uses `github-pages` gem for compatibility
- Minimal Mistakes theme provides layouts: default, home, archive, single, page, posts, categories, tags, collection, compress
- Author info and social links configured in `_config.yml`
- Theme supports multiple skins: default, air, aqua, contrast, dark, dirt, neon, mint, plum, sunrise
- Requires `jekyll-include-cache` plugin for optimal performance
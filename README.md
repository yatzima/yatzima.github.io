# Justin Ma's Personal Website

Personal website and blog built with Jekyll and the Minimal Mistakes theme, hosted on GitHub Pages.

🔗 **Live Site**: [yatzima.github.io](https://yatzima.github.io)

## About

This is the personal website of Justin Ma, Data Scientist at Rambøll. The site showcases professional background, projects, and technical blog posts related to data science and machine learning.

## Tech Stack

- **Static Site Generator**: Jekyll 4.x
- **Theme**: [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes) (modern, responsive)
- **Hosting**: GitHub Pages
- **Ruby**: 3.1.4+ (managed with [mise](https://mise.jdx.dev))

## Local Development

### Prerequisites
- Ruby 3.1.4+ (install with `mise use ruby@3.1.4`)
- Bundler

### Setup
```bash
# Clone the repository
git clone https://github.com/yatzima/yatzima.github.io.git
cd yatzima.github.io

# Install dependencies
bundle install

# Serve locally
bundle exec jekyll serve
```

The site will be available at `http://localhost:4000`

## Project Structure

```
├── _config.yml          # Site configuration
├── _posts/              # Blog posts
├── _pages/              # Static pages (About, etc.)
├── assets/
│   ├── files/           # Documents (CV, etc.)
│   ├── images/          # Images and graphics
│   └── css/             # Custom stylesheets
├── _data/               # Data files (YAML, JSON)
├── index.markdown       # Homepage
├── Gemfile              # Ruby dependencies
└── .gitignore           # Git ignore rules
```

## Content Management

### Adding Blog Posts
Create new files in `_posts/` with format: `YYYY-MM-DD-title.markdown`

```yaml
---
layout: single
title: "Your Post Title"
date: 2024-01-01
categories: [data-science, machine-learning]
---

Your content here...
```

### Adding Pages
Create new files in `_pages/` with appropriate front matter:

```yaml
---
layout: single
title: "Page Title"
permalink: /page-url/
---

Your content here...
```

## Deployment

The site automatically deploys to GitHub Pages when changes are pushed to the `master` branch.

## License

Content is personal and proprietary. Jekyll theme is MIT licensed.

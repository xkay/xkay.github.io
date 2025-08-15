# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

This is a Jekyll-based personal website. All commands should be run from the `docs/` directory:

```bash
cd docs/
bundle install          # Install dependencies
bundle exec jekyll serve # Run development server (localhost:4000)
bundle exec jekyll build # Build the site
```

## Architecture Overview

This is a personal portfolio website built with Jekyll using the Pudhina theme. The site structure follows Jekyll conventions:

- **Content files**: Written in Markdown with YAML front matter
  - `index.md` - Homepage with personal introduction
  - `quotes.md` - Inspirational quotes page
  - `blog.md` - Blog listing page (if used)
  - `resume.md` - Resume page (currently commented out in navigation)

- **Layout system**: Located in `_layouts/`
  - `default.html` - Base template with header, analytics, and scripts
  - `page.html` - Standard page layout
  - `poem.html` - Special layout for poem content

- **Includes**: Reusable components in `_includes/`
  - `header.html` - Site navigation and social links
  - `externals/` - Google Analytics, styling, and script includes
  - `meta_tags/` and `page/` - SEO and page-specific components

- **Posts**: Blog posts in `_posts/` following Jekyll naming convention (YYYY-MM-DD-title.md)

- **Static assets**: CSS, images, and vendor files in `assets/`

## Site Configuration

Key settings in `_config.yml`:
- Site title, description, and URL
- Author information (GitHub, LinkedIn, email)
- Syntax highlighting configuration
- Markdown processor (kramdown)

## Content Management

- Navigation is defined in `_includes/header.html`
- Currently only "Quotes" page is active in navigation
- Resume and Blog pages exist but are commented out
- Social links automatically generated from author config
- Images stored in `assets/img/`

## Theme Customization

This uses a modified version of the Pudhina theme:
- Main styling in `assets/css/main.css`
- Responsive design with clean, minimal aesthetic
- Font Awesome icons for social links
- Highlight.js for syntax highlighting with configurable themes
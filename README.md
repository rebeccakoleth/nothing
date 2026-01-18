# Personal Blog

A private Jekyll blog using the Tale theme.

## Setup Instructions

### Option 1: Use Tale as a Remote Theme (Recommended)
1. Uncomment the `remote_theme: chesterhow/tale` line in `_config.yml`
2. Add `gem "jekyll-remote-theme"` to your Gemfile (already included but commented)
3. This will automatically pull the Tale theme from GitHub

### Option 2: Clone Tale Theme Directly
1. Go to https://github.com/chesterhow/tale
2. Download or clone the theme
3. Copy the `_layouts`, `_includes`, and `assets` folders into this repo

## Local Development

1. Install dependencies:
   ```bash
   bundle install
   ```

2. Run the site locally:
   ```bash
   bundle exec jekyll serve
   ```

3. View at: http://localhost:4000

## Creating a Private GitHub Repository

1. Go to https://github.com/new
2. Name your repository (e.g., `private-blog`)
3. Select "Private"
4. Don't initialize with README (we already have one)
5. Click "Create repository"

6. In your terminal, from this directory:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/private-blog.git
   git push -u origin main
   ```

## Writing Posts

Create new posts in the `_posts` folder with the naming format:
`YYYY-MM-DD-title-of-post.md`

Start each post with front matter:
```yaml
---
layout: post
title: "Your Post Title"
date: 2026-01-18
---
```

## Customization

Edit `_config.yml` to change:
- Site title
- Your name
- Email
- Description
- Other settings

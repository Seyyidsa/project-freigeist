# Project Freigeist - Jekyll Website

Your static HTML website has been successfully transformed into a Jekyll-powered website! Now you can easily create pages using Markdown files.

## Quick Start

1. **Install dependencies:**
   ```bash
   bundle install --path vendor/bundle
   ```

2. **Start the development server:**
   ```bash
   bundle exec jekyll serve --host 0.0.0.0 --port 4000
   ```

3. **View your site at:** http://localhost:4000

## Creating New Content

### Creating a New Blog Post

Create a new file in the `_posts` folder with the format: `YYYY-MM-DD-title.md`

Example: `_posts/2024-09-02-my-new-post.md`

```markdown
---
layout: post
title: "My New Post"
date: 2024-09-02
category: "Philosophy"
tags: ["creativity", "AI"]
lang: en
excerpt: "A brief description of your post"
---

Your content goes here in Markdown format.

## Heading 2

This is a paragraph with some **bold** and *italic* text.

- List item 1
- List item 2
```

### Creating a New Page

Create a new `.md` file in the root directory:

```markdown
---
layout: page
title: "About"
permalink: /about/
lang: en
---

# About Page

Your page content in Markdown.
```

### Language Support

The site supports both English and German:

- **English pages:** Set `lang: en` in front matter
- **German pages:** Set `lang: de` in front matter

German pages will automatically use the Jersey 25 font and retro styling.

## Directory Structure

```
├── _config.yml          # Site configuration
├── _layouts/            # HTML templates
├── _includes/           # Reusable HTML components
├── _posts/             # Blog posts
├── _sass/              # Sass stylesheets
├── assets/             # CSS, JS, images
├── Gemfile             # Ruby dependencies
├── index.md            # Homepage
├── projekt.md          # German project page
├── explanation.md      # English explanation page
├── resources.md        # Resources page
└── writing.md          # Writing/blog index
```

## Key Features

✅ **Markdown Support**: Write content in Markdown instead of HTML
✅ **Dual Language**: Supports both English and German with different styling
✅ **Blog System**: Automatic post generation with categories and tags
✅ **SEO Friendly**: Built-in SEO tags and sitemap
✅ **Responsive Design**: Mobile-friendly layouts
✅ **Development Server**: Live reload during development

## Customization

- **Colors & Styling**: Edit files in `_sass/` folder
- **Layout**: Modify files in `_layouts/` and `_includes/`
- **Configuration**: Update `_config.yml`
- **Navigation**: Edit `_includes/header.html`

## Deployment

The site generates static HTML files in the `_site` folder, which can be deployed to any web server or hosting platform like GitHub Pages, Netlify, or Vercel.

## Adding Content Examples

**For a German philosophy post:**
```markdown
---
layout: post
title: "🌀 Neue Gedanken zum Freigeist"
date: 2024-09-02
category: "Philosophy"
tags: ["philosophie", "ki", "bewusstsein"]
lang: de
---

Ihr deutscher Inhalt hier...
```

**For an English creativity post:**
```markdown
---
layout: post
title: "💭 Thoughts on Creative AI"
date: 2024-09-02
category: "Creativity"
tags: ["creativity", "AI", "innovation"]
lang: en
---

Your English content here...
```

Happy blogging! 🚀
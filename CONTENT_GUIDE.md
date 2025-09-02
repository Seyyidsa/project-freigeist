# Content Management Guide

## 📁 **Easy-to-Maintain Folder Structure**

```
project-freigeist/
├── 📄 *.md                    # Static pages (index, explanation, resources, etc.)
├── 📂 _posts/                 # Blog posts (Jekyll standard)
│   └── YYYY-MM-DD-title.md   # All posts with date-based naming
├── 📂 templates/              # Post templates for easy creation
│   ├── philosophy-post.md    # Template for philosophy posts
│   ├── creativity-post.md    # Template for creativity posts
│   └── weekly-post.md        # Template for weekly posts
├── 📂 _data/                  # Site configuration data
│   ├── navigation.yml        # Menu structure
│   └── site.yml             # Site settings & categories
├── 📂 _layouts/               # HTML templates
├── 📂 _includes/              # Reusable components
├── 📂 _sass/                  # Styling (SCSS)
└── 📂 assets/                 # CSS, images, downloads
```

## ✍️ **How to Add New Content**

### Creating a New Philosophy Post

1. **Copy the template:**
   ```bash
   cp templates/philosophy-post.md _posts/2024-09-02-my-philosophy-post.md
   ```

2. **Edit the file:**
   ```markdown
   ---
   title: "🌀 My Deep Thoughts on AI"
   date: 2024-09-02
   category: philosophy
   tags: ["philosophy", "AI", "consciousness"]
   ---
   
   Your content here...
   ```

### Creating a New Creativity Post

1. **Copy the template:**
   ```bash
   cp templates/creativity-post.md _posts/2024-09-02-creative-ideas.md
   ```

2. **Edit and publish!**

### Creating a Weekly Update

1. **Copy the template:**
   ```bash
   cp templates/weekly-post.md _posts/2024-09-02-woche-XX.md
   ```

2. **Update with weekly insights**

### Adding a New Page

1. **Create in the root directory:**
   ```bash
   touch about.md
   ```

2. **Add front matter:**
   ```markdown
   ---
   layout: page
   title: "About"
   permalink: /about/
   lang: en  # or "de" for German
   ---
   
   Your page content...
   ```

## 🎯 **Benefits of This Structure**

✅ **Jekyll Standard**: Uses Jekyll's expected folder structure
✅ **Templates Ready**: Copy-paste templates for consistent formatting  
✅ **Category System**: Posts automatically organized by category in front matter
✅ **Data-Driven**: Navigation and settings in YAML files
✅ **Simple & Clean**: Easy to understand and maintain
✅ **Future-Proof**: Standard Jekyll structure works everywhere

## 🔧 **Customization**

### Adding a New Post Category

1. **Create template:**
   ```bash
   cp templates/philosophy-post.md templates/new-category-post.md
   ```

2. **Update template category:**
   ```yaml
   category: new-category
   ```

3. **Add to `_data/site.yml`:**
   ```yaml
   categories:
     new-category:
       name: "New Category"
       icon: "🆕"
   ```

### Updating Navigation

Edit `_data/navigation.yml` to add/remove menu items for each language.

### Changing Site Settings

Edit `_data/site.yml` to update titles, descriptions, and social links.

## 🚀 **Quick Commands**

```bash
# Start development server
bundle exec jekyll serve

# Create new philosophy post
cp templates/philosophy-post.md _posts/$(date +%Y-%m-%d)-my-philosophy-post.md

# Create new creativity post
cp templates/creativity-post.md _posts/$(date +%Y-%m-%d)-my-creativity-post.md

# Create new weekly update  
cp templates/weekly-post.md _posts/$(date +%Y-%m-%d)-woche-$(date +%V).md

# Build for production
bundle exec jekyll build
```

This structure makes it super easy to manage your content while keeping everything organized! 🎉
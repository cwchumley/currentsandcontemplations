# Content Migration Guide

## Overview
This guide will help you migrate content from your existing Wix site at https://www.currentsandcontemplations.com/ to your new Hugo site.

## Migration Checklist

### 1. ✅ Content Structure Setup
- [x] Created blog post templates with proper Hugo front matter
- [x] Set up categories and tags structure
- [x] Configured Hugo settings for blog functionality

### 2. Content to Migrate

Based on your existing site, here are the posts that need content migration:

#### Blog Posts:
1. **Cloud Peak Wilderness Trip, July, 2024, pt. 1** → `content/posts/cloud-peak-wilderness-july-2024-pt1.md`
2. **Fall Upper Colorado Fishing Trip, pt. 2** → `content/posts/fall-upper-colorado-pt2.md`
3. **Fall Upper Colorado Fishing Trip, pt. 1** → `content/posts/fall-upper-colorado-pt1.md`
4. **Boulder Creek Adventure** → `content/posts/boulder-creek-adventure.md`
5. **Early Season Reflections** → `content/posts/early-season-reflections.md`

#### Categories on original site:
- All Posts (5)
- Fishing (3)
- Upper Colorado (2)
- William Forks (1)

#### Tags on original site:
- fishing (3)
- upper colorado (2)
- 2023 (1)
- boulder creek (1)
- fall (1)
- front range fishing (1)
- williams fork (1)

### 3. Manual Content Migration Steps

Since your site is on Wix, you'll need to manually copy content:

1. **Visit each blog post on your live site**
2. **Copy the full text content**
3. **Save any images** used in posts to `static/images/posts/`
4. **Update the Hugo markdown files** with the real content

### 4. Image Migration

For each blog post:
1. Right-click and save images from your Wix site
2. Save them to `static/images/posts/[post-name]/`
3. Update markdown files to reference local images: `![Alt text](/images/posts/post-name/image.jpg)`

### 5. Quick Migration Commands

```bash
# Create images directory structure
mkdir -p static/images/posts/cloud-peak-wilderness
mkdir -p static/images/posts/upper-colorado
mkdir -p static/images/posts/boulder-creek

# Test your Hugo site locally
hugo server -D

# Build the site
hugo
```

### 6. Content Migration Priority

**High Priority:**
1. Cloud Peak Wilderness Trip (your featured post)
2. Upper Colorado series (popular content)

**Medium Priority:**
3. Boulder Creek Adventure
4. Early Season Reflections

### 7. SEO Considerations

When migrating content, preserve:
- Original publish dates
- URL structure (use Hugo aliases if needed)
- Meta descriptions
- Image alt tags

### 8. Post-Migration Tasks

After content migration:
1. Test all internal links
2. Verify image loading
3. Check mobile responsiveness
4. Test search functionality
5. Validate HTML/CSS
6. Set up 301 redirects for old URLs

## Content Migration Template

For each post, follow this template:

```markdown
---
title: "[Original Title]"
date: [YYYY-MM-DD]T[HH:MM:SS]-[TZ]
draft: false
tags: ["tag1", "tag2", "tag3"]
categories: ["Category1", "Category2"]
description: "[SEO description]"
---

# [Post Title]

[Introduction paragraph]

## [Section 1]

[Content...]

![Image Alt Text](/images/posts/post-name/image.jpg)

[More content...]

## [Section 2]

[Content...]

---

*[Optional footer/series information]*
```

## Need Help?

If you need assistance with any part of the migration:
1. Check Hugo documentation: https://gohugo.io/documentation/
2. PaperMod theme docs: https://github.com/adityatelange/hugo-PaperMod
3. Test changes locally with `hugo server -D` before deploying 
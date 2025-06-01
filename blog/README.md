# Blog Guide

This directory contains the blog section of the website.

## Directory Structure

```
blog/
├── index.html          # Main blog listing page
├── posts/             # Individual blog posts
│   ├── template.html  # Template for new posts
│   └── *.html        # Individual blog posts
├── images/           # Images used in blog posts
└── README.md        # This file
```

## Creating a New Blog Post

1. **Copy the template:**
   ```bash
   cp posts/template.html posts/your-post-name.html
   ```

2. **Edit your new post:**
   - Replace all placeholders in square brackets `[LIKE THIS]`
   - Update the title, date, reading time, and meta description
   - Write your content using standard HTML elements
   - Update the current URL at the bottom of the page

3. **Add your post to the blog index:**
   - Open `index.html`
   - Add a new blog post entry following the existing format:
   ```html
   <div class="blog-post-item">
     <div class="post-date">Month DD, YYYY</div>
     <h2 class="post-title">
       <a href="posts/your-post-name.html">Your Post Title</a>
     </h2>
     <p class="post-excerpt">
       A brief description of your post...
     </p>
     <a href="posts/your-post-name.html" class="read-more">Read more →</a>
   </div>
   ```

4. **Add images (if needed):**
   - Place images in the `images/` directory
   - Reference them in your post as: `../images/your-image.jpg`

## Style Guidelines

- Keep the design minimalistic and consistent with the main website
- Use proper heading hierarchy (h1 for title, h2 for main sections, h3 for subsections)
- Include reading time estimates (roughly 200-250 words per minute)
- Add meaningful meta descriptions for SEO (150-160 characters)

## URL Structure

- Blog index: `/blog/`
- Individual posts: `/blog/posts/post-name.html`

## Tips

- Use descriptive, SEO-friendly URLs (e.g., `journaling-in-ai.html` instead of `post1.html`)
- Include the current page URL at the bottom for easy reference
- Test all navigation links before publishing
- Consider adding Open Graph meta tags for better social media sharing 
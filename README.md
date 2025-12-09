# Muhammad Arbab's Personal Website

Personal academic website: https://arbab-ml.github.io

Based on [Jon Barron's website template](https://jonbarron.info/).

## Project Structure

```
arbab-ml.github.com/
├── index.html          # Main homepage
├── stylesheet.css      # Site styling
├── CNAME              # Custom domain config
├── images-me/         # Personal images
├── data-me/           # Personal data
├── blog/
│   ├── index.html     # Blog listing page
│   ├── images/        # Blog images
│   └── posts/
│       ├── template.html  # Template for new posts
│       └── *.html         # Individual blog posts
└── README.md          # This file
```

## Creating a New Blog Post

1. **Copy the template:**
   ```bash
   cp blog/posts/template.html blog/posts/your-new-post-name.html
   ```

2. **Edit your new post (`your-new-post-name.html`):**
   - **Metadata (HTML Head):**
     - Update `<title>[POST TITLE] - Muhammad Arbab</title>`
     - Update `<meta name="description" content="[POST DESCRIPTION]">`
   - **Post Header (HTML Body):**
     - Update `<h1 class="post-title">[POST TITLE]</h1>`
     - Update `<time>[DATE - Month DD, YYYY]</time> · [READING TIME] min read`
   - **Markdown Content:**
     - Locate `<script type="text/markdown" id="markdown-source">`
     - Write your blog post in Markdown inside this tag
   - **Filename in URL:**
     - Update `Current page: /blog/posts/[FILENAME].html` at the bottom

3. **Add your post to the blog index (`blog/index.html`):**
   ```html
   <div class="blog-post-item">
     <div class="post-date">Month DD, YYYY</div>
     <h2 class="post-title">
       <a href="posts/your-new-post-name.html">Your Post Title</a>
     </h2>
     <p class="post-excerpt">
       A brief description of your post...
     </p>
     <a href="posts/your-new-post-name.html" class="read-more">Read more →</a>
   </div>
   ```

4. **Add images (if needed):**
   - Place images in `blog/images/`
   - Reference in Markdown: `![Alt text](../images/your-image.jpg)`

## Style Guidelines

- Keep the design minimalistic and consistent
- Use proper heading hierarchy (h1 for title, h2 for sections, h3 for subsections)
- Include reading time estimates (~200-250 words per minute)
- Add meta descriptions for SEO (150-160 characters)
- Use descriptive, SEO-friendly URLs (e.g., `journaling-in-ai.html`)

## URL Structure

- Homepage: `/`
- Blog index: `/blog/`
- Blog posts: `/blog/posts/post-name.html`

## Technical Notes

- Blog posts use Markdown rendered client-side via `Marked.js`
- No build step required - just edit HTML files directly
- Test navigation links before publishing

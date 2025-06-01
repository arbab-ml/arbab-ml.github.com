# Blog Guide

This directory contains the blog section of the website.

## Directory Structure

```
blog/
├── index.html          # Main blog listing page
├── posts/             # Individual blog posts
│   ├── template.html  # Template for new posts (uses Markdown)
│   └── *.html        # Individual blog posts (containing Markdown)
├── images/           # Images used in blog posts
└── README.md        # This file
```

## Creating a New Blog Post (Markdown Workflow)

1.  **Copy the template:**
    ```bash
    cp posts/template.html posts/your-new-post-name.html
    ```

2.  **Edit your new post (`your-new-post-name.html`):**
    *   **Metadata (HTML Head):**
        *   Update the `<title>[POST TITLE] - Muhammad Arbab</title>`.
        *   Update the `<meta name="description" content="[POST DESCRIPTION]">`.
    *   **Post Header (HTML Body):**
        *   Update `<h1 class="post-title">[POST TITLE]</h1>`.
        *   Update `<time>[DATE - Month DD, YYYY]</time> · [READING TIME] min read`.
    *   **Markdown Content:**
        *   Locate the `<script type="text/markdown" id="markdown-source">` tag.
        *   Write your entire blog post content in Markdown format *inside* this script tag, replacing the example Markdown.
        *   You can use standard Markdown syntax (headings, lists, code blocks, etc.).
    *   **Filename in URL:**
        *   At the bottom, update `Current page: /blog/posts/[FILENAME].html` to reflect the new filename (e.g., `your-new-post-name.html`).

3.  **Add your post to the blog index (`blog/index.html`):**
    *   Open `blog/index.html`.
    *   Add a new blog post entry following the existing format. Make sure the `href` points to your new HTML file:
    ```html
    <div class="blog-post-item">
      <div class="post-date">Month DD, YYYY</div> <!-- Match the date in your post -->
      <h2 class="post-title">
        <a href="posts/your-new-post-name.html">Your Post Title</a> <!-- Match the title -->
      </h2>
      <p class="post-excerpt">
        A brief description of your post... <!-- Match the meta description -->
      </p>
      <a href="posts/your-new-post-name.html" class="read-more">Read more →</a>
    </div>
    ```

4.  **Add images (if needed):**
    *   Place images in the `blog/images/` directory.
    *   Reference them in your Markdown content using standard Markdown image syntax: `![Alt text](../images/your-image.jpg)` (note the `../images/` path from within the `posts` directory).

## Style Guidelines

-   The HTML structure and CSS handle the overall styling.
-   Focus on semantic Markdown for your content.
-   Keep the design minimalistic and consistent with the main website.
-   Include reading time estimates (roughly 200-250 words per minute).
-   Add meaningful meta descriptions for SEO (150-160 characters).

## URL Structure

-   Blog index: `/blog/`
-   Individual posts: `/blog/posts/post-name.html`

## Tips

-   Use descriptive, SEO-friendly URLs for your HTML files (e.g., `journaling-in-ai.html`).
-   Test all navigation links before publishing.
-   The Markdown is rendered client-side using `Marked.js`.

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
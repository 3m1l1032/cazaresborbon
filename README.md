# Emilio Cazares Borbon - Personal Portfolio

Personal website built with static HTML and CSS.

## Project Structure

```text
/
├── CNAME                    # Custom domain for GitHub Pages
├── README.md                # Project documentation
├── index.html               # Home / About / Experience
├── styles.css               # Shared styles used by all pages
├── images/                  # Site images and media
├── projects/
│   └── index.html           # Projects page (/projects/)
├── blog/
│   └── index.html           # Blog listing page (/blog/)
├── pages/
│   ├── projects.html        # Legacy page path (optional)
│   └── blog.html            # Legacy page path (optional)
└── posts/
    └── post-template.html   # Template for future blog posts
```

## Local Preview

1. Open [index.html](index.html) in your browser.
2. Navigate through the site using the top navigation.

Optional (recommended) local server from the repo root:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000/`.

## Content Updates

### Add a New Blog Post

1. Duplicate [posts/post-template.html](posts/post-template.html).
2. Rename it with a slug, for example: `posts/my-first-post.html`.
3. Update title, metadata, content, and footer tags in the new post file.
4. Add an entry in [blog/index.html](blog/index.html) so the post appears in the listing.

### Add or Edit Projects

1. Open [projects/index.html](projects/index.html).
2. Copy an existing `<article class="project-full">` block.
3. Update the project `id`, title, description, tags, and external links.

### Add or Edit Experience

1. Open [index.html](index.html).
2. Find the `<div class="timeline">` section.
3. Copy an existing `<article class="timeline-item">` block.
4. Update date, role, organization, and description.
5. Keep entries in reverse-chronological order.

### Update Profile Photo

1. Open [index.html](index.html).
2. Find the `<img class="hero-photo">` element.
3. Update the `src` path to your new image in [images](images).

## Deployment Notes

- The [CNAME](CNAME) file is used for the custom GitHub Pages domain.
- Keep relative paths consistent:
  - From files in [pages](pages), use `../styles.css` and `../images/...`.

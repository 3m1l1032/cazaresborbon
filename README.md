# Emilio Cazares Borbon - Personal Portfolio

A clean, minimal personal portfolio website built with HTML and CSS.

## File Structure

\`\`\`
/
├── index.html          # Home page (about, experience)
├── projects.html       # Projects showcase
├── blog.html           # Blog listing page
├── styles.css          # All styles
├── posts/              # Blog post files
│   └── post-template.html  # Template for new posts
└── README.md           # This file
\`\`\`

---

## How to Add Content

### Adding a New Blog Post

1. **Copy the template:**
   - Duplicate `posts/post-template.html`
   - Rename it to your post's slug (e.g., `posts/my-new-post.html`)

2. **Edit the post file:**
   - Update the `<title>` tag
   - Change the date and category in `.post-meta`
   - Write your title in `.post-title`
   - Add your content in `.post-content`
   - Update tags in `.post-footer`

3. **Add to blog listing:**
   - Open `blog.html`
   - Copy an existing `<article class="blog-post">` block
   - Update the date, category, title, excerpt, and links
   - Place newer posts at the top

### Adding a New Project

1. Open `projects.html`
2. Copy an existing `<article class="project-full">` block
3. Update:
   - The `id` attribute for linking
   - The gradient colors in `style="background: ..."`
   - The icon emoji
   - Title, description, and tags
   - GitHub link

**Gradient color suggestions:**
- Blue/Purple: `linear-gradient(135deg, #3b82f6, #8b5cf6)`
- Green/Cyan: `linear-gradient(135deg, #10b981, #06b6d4)`
- Orange/Red: `linear-gradient(135deg, #f59e0b, #ef4444)`
- Pink/Purple: `linear-gradient(135deg, #ec4899, #8b5cf6)`

### Adding Experience

1. Open `index.html`
2. Find the `<div class="timeline">` section
3. Copy an existing `<article class="timeline-item">` block
4. Update the date, title, company, and description
5. Place in chronological order (newest first)

### Updating Your Photo

Replace the `src` attribute in the `.hero-photo` `<img>` tag with your actual photo path:

```html
<img src="images/your-photo.jpg" alt="Emilio Cazares Borbon" class="hero-photo">

# PureGradient GitHub Pages

Live at: https://puregradient.com (custom domain), also served at https://puregradient.github.io and forwarded from https://puregradient.co.uk 

## Site Structure

```
puregradient.github.io/
├── index.html              (homepage — hero, about, blog grid)
├── team.html                (team profiles + photos, links to individual portfolios)
├── projects.html            (project showcase grid — Sim Med Suite, Computarium, Ref-Platform)
├── innovation.html          (consulting services)
├── images/                  (photos, blog thumbnails)
└── blog/
    ├── blog-template.html    (starting point for new posts)
    └── ... individual post files
```

Related standalone sites (separate repos, linked from Team page):
- `puregradient.github.io/karen` — Karen Lawson's portfolio
- `puregradient.github.io/samantha` — Samantha Lawson's portfolio

## Features Implemented ✅

- Light/Dark theme toggle (◐ button in nav), preference saved via localStorage
- Mobile hamburger menu on all pages (☰ button below 768px width)
- Auto-updating copyright year
- Responsive design for mobile
- Clean, minimal aesthetic with a gradient-contour signature motif on page headers
- Smooth transitions and hover effects
- All pages properly linked, including cross-links to team members' individual portfolio sites
- Full blog migrated from Wix — 11 posts, chronologically ordered, tagged by topic
- Blog homepage cards with thumbnail images where available

## Creating New Blog Posts

1. Copy `blog/blog-template.html`
2. Rename it (e.g., `blog/my-new-post.html`)
3. Edit the content:
   - Update `<title>` tag
   - Change the `<h1>` heading
   - Update `.post-meta` with author and date
   - Add your content in `.post-content`
4. Add a card for it on `index.html` in the blog-grid section (image + title + excerpt + meta + tags)

## Customization Tips

### Change Colors

Edit the `:root` variables in any HTML file:

```css
:root {
    --primary: #0a0a0a;      /* Text color */
    --secondary: #666;        /* Muted text */
    --accent: #0066ff;        /* Links/highlights */
    --bg: #ffffff;            /* Background */
    --border: #e5e5e5;        /* Borders */
}
```

Dark mode variables live in the adjacent `[data-theme="dark"]` block.

### Add Images

1. Add images to the `images/` folder in the repo root
2. Reference them: `<img src="/images/photo.jpg" alt="Description">`
3. Keep file sizes reasonable — aim for under ~300–500KB per image (resize to ~1200px wide, compress via squoosh.app or tinypng.com before uploading). JPG for photos, PNG only for graphics/screenshots needing transparency.

## To-Do / Future Improvements

- [ ] Finalize favicon (logo too detailed for small sizes — needs a simplified variant)
- [ ] Consider Jekyll or a static site generator if blog volume grows further
- [ ] Add RSS feed
- [ ] Add Google Analytics
- [ ] Add meta tags (Open Graph) for nicer link previews when shared on LinkedIn/Twitter
- [ ] Custom 404 page
- [ ] Add further team members
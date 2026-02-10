# PureGradient GitHub Pages

### Features Implemented ✅
- Light/Dark theme toggle (◐ button in nav)
- Auto-updating copyright year
- Responsive design for mobile
- Clean, minimal aesthetic
- Smooth transitions and hover effects
- All pages properly linked

### Creating New Blog Posts
1. Copy `blog/blog-template.html`
2. Rename it (e.g., `blog/my-new-post.html`)
3. Edit the content:
   - Update `<title>` tag
   - Change the `<h1>` heading
   - Update `.post-meta` with author and date
   - Add your content in `.post-content`
4. Add a link to it on `index.html` in the blog-grid section

### Customization Tips

#### Change Colors
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

#### Add Images
To add images to blog posts or pages:
1. Create an `images` folder in your repo
2. Add images there
3. Reference them: `<img src="/images/photo.jpg" alt="Description">`

## To-Do / Future Improvements
- [ ] Add actual blog post content from Wix site
- [ ] Add team member photos
- [ ] Add favicon
- [ ] Consider Jekyll for easier blog management
- [ ] Add RSS feed
- [ ] Add Google Analytics (optional)

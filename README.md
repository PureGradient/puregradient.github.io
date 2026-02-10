# PureGradient GitHub Pages Site

## What's Included

### Main Pages
- **index.html** - Homepage with blog overview
- **team.html** - Team member profiles
- **innovation.html** - Innovation consulting services
- **toolbox.html** - Toolbox page

### Blog
- **blog/blog-template.html** - Template for creating new blog posts
- **blog/doha-trip.html** - Sample blog post (placeholder)

### Features Implemented ✅
- Light/Dark theme toggle (◐ button in nav)
- Auto-updating copyright year
- Responsive design for mobile
- Clean, minimal aesthetic
- Smooth transitions and hover effects
- All pages properly linked

## How to Use

### Upload to GitHub
1. Clone your `puregradient.github.io` repo
2. Copy all files to the root of your repo
3. Commit and push:
   ```bash
   git add .
   git commit -m "Add complete site with theme toggle"
   git push
   ```
4. Wait a few minutes for GitHub Pages to build
5. Visit https://puregradient.github.io

### File Structure
```
puregradient.github.io/
├── index.html
├── team.html
├── innovation.html
├── toolbox.html
└── blog/
    ├── blog-template.html
    ├── doha-trip.html
    └── (add more blog posts here)
```

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

#### Custom Domain
To point puregradient.com to GitHub Pages:
1. In your repo: Settings → Pages → Custom domain
2. Enter: puregradient.com
3. In your domain registrar's DNS settings:
   - Add A records pointing to GitHub's IPs:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153
   - Or add CNAME record: puregradient.github.io

## To-Do / Future Improvements
- [ ] Add actual blog post content from Wix site
- [ ] Add team member photos
- [ ] Add favicon
- [ ] Consider Jekyll for easier blog management
- [ ] Add RSS feed
- [ ] Add Google Analytics (optional)

## Theme Toggle
The theme toggle:
- Saves preference in localStorage
- Works across all pages
- Smoothly animates color changes
- Uses ◐ symbol (half-moon) for the button

## Questions?
Everything is self-contained in the HTML files - no build process needed! Just edit the HTML directly and push to GitHub.

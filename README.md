# pRadar Website

Product landing page for pRadar - Singapore Property Tracker.

## Files

| File | Description |
|------|-------------|
| `index.html` | Main landing page |
| `privacy-policy.html` | Privacy policy page |
| `logo.png` | App logo (you need to add this) |
| `intro_output_appstore.mp4` | App preview video (you need to add this) |
| `favicon.png` | Browser favicon (optional) |

## Setup

1. **Add required assets:**
   ```
   website/
   ├── index.html          ✅ Ready
   ├── privacy-policy.html ✅ Ready
   ├── logo.png            ❌ Add your app logo (recommended: 512x512)
   ├── intro_output_appstore.mp4  ❌ Add your video
   └── favicon.png         ❌ Optional (recommended: 32x32)
   ```

2. **Update App Store link:**
   - In `index.html`, replace `href="#"` in the App Store buttons with your actual App Store URL
   - Example: `href="https://apps.apple.com/app/pradar/id123456789"`

3. **Update contact info:**
   - In `privacy-policy.html`, replace `[Your Contact Email]` and `[Your Website URL]`
   - In `index.html` footer, update the support email

## Deployment Options

### Option 1: GitHub Pages (Free)
```bash
# Create a new repo or use existing
git init
git add .
git commit -m "Add website"
git remote add origin https://github.com/yourusername/pradar-website.git
git push -u origin main

# Enable GitHub Pages in repo settings
# Your site will be at: https://yourusername.github.io/pradar-website/
```

### Option 2: Cloudflare Pages (Free)
1. Push to GitHub
2. Connect repo to Cloudflare Pages
3. Deploy

### Option 3: Vercel (Free)
```bash
npm i -g vercel
vercel
```

### Option 4: Netlify (Free)
1. Drag and drop the `website` folder to netlify.com

## Preview Locally

```bash
# Using Python
cd website
python -m http.server 8000
# Open http://localhost:8000

# Using Node.js
npx serve website
```

## Features

- **Hero Section**: Video preview with iPhone frame mockup
- **Features Grid**: 6 key features with icons
- **Data Source Badge**: URA official data source
- **CTA Section**: Download call-to-action
- **Responsive**: Works on mobile and desktop
- **Dark Theme Hero**: Modern gradient background

## Customization

### Colors
Edit CSS variables in `index.html`:
```css
:root {
    --primary: #007AFF;
    --secondary: #34C759;
    /* ... */
}
```

### Video Autoplay
The video is set to autoplay, loop, and mute by default:
```html
<video autoplay loop muted playsinline>
```

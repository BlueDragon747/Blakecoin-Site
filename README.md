# Blakecoin Website

A static version of the Blakecoin website optimized for GitHub Pages hosting.

## Overview

This repository contains a static version of the Blakecoin website (blakecoin.org), converted from WordPress to work with GitHub Pages. This eliminates hosting costs while maintaining full control over the content.

## Structure

- `index.html` - Homepage
- `about-blakecoin/` - About Blakecoin page
- `software/` - Software downloads page
- `merged-mining/` - Blake Ecosystem page
- `assets/` - CSS, JavaScript, images, and fonts
- `.github/workflows/` - GitHub Actions deployment workflow

## GitHub Pages Deployment

### Method 1: Automatic Deployment (Recommended)

1. Push this repository to GitHub
2. Go to **Settings > Pages** in your GitHub repository
3. Under "Build and deployment", select **GitHub Actions** as the source
4. The site will automatically deploy on every push to the main/master branch

### Method 2: Manual Deployment

1. Push this repository to GitHub
2. Go to **Settings > Pages** in your GitHub repository
3. Under "Build and deployment", select **Deploy from a branch**
4. Select the `main` or `master` branch and `/ (root)` folder
5. Click Save

## Custom Domain (Optional)

To use a custom domain (e.g., blakecoin.org):

1. Go to **Settings > Pages** in your GitHub repository
2. Under "Custom domain", enter your domain name
3. Create a DNS record pointing your domain to GitHub Pages:
   - For apex domain (blakecoin.org): Create A records pointing to:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153
   - For www subdomain (www.blakecoin.org): Create a CNAME record pointing to `yourusername.github.io`
4. The `CNAME` file is already included in this repository

## Updating Content

1. Edit the HTML files directly
2. Update links and content as needed
3. Commit and push changes
4. The site will automatically update (if using GitHub Actions) or within a few minutes

## Local Development

To test locally, simply open `index.html` in a web browser, or use a local server:

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js
npx serve .
```

Then visit `http://localhost:8000` in your browser.

## Features

- Static HTML (no database or server-side code needed)
- Responsive design using Customizr theme
- Font Awesome icons
- All assets self-hosted (no external dependencies)
- SEO-friendly structure

## Credits

- Original website: blakecoin.org
- Theme: Customizr (WordPress theme adapted for static use)
- Icons: Font Awesome

## License

This static website is provided as-is for the Blakecoin community. Original theme and assets retain their respective licenses.
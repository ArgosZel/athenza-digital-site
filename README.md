# Athenza Digital Static Website

Professional landing page for Athenza Digital website optimization services.

## Live Demo
Once deployed, the site will be available at:
- GitHub Pages URL: `https://[your-username].github.io/[repository-name]/`
- Custom domain: `https://athenzadigital.com` (after DNS configuration)

## Features
- Fully responsive design (mobile, tablet, desktop)
- Brand‑consistent colors and typography (Inter font)
- Performance‑optimized (Tailwind CSS via CDN, no heavy frameworks)
- Contact form with client‑side validation
- Privacy policy page
- Custom 404 page
- SEO‑friendly meta tags

## File Structure
```
├── index.html          # Main landing page
├── privacy.html        # Privacy policy
├── 404.html            # Custom 404 page
├── CNAME               # Custom domain configuration
├── .nojekyll           # Disable Jekyll processing
├── assets/
│   ├── logo-colored.png   # Colored logo variant
│   └── logo-white.png     # White logo variant (for dark backgrounds)
└── README.md           # This file
```

## Deployment Instructions

### Option A: Deploy via GitHub Pages (Recommended)
1. Create a new **public** repository on GitHub (e.g., `athenza-digital-site`).
2. Upload all files from this folder to the repository.
3. Go to **Settings → Pages**.
4. Under **Source**, select `Deploy from a branch` → `main` (or `master`) branch → `/ (root)`.
5. Click **Save**. Your site will be live at `https://[username].github.io/athenza-digital-site/` within 1‑2 minutes.
6. To use a custom domain (`athenzadigital.com`):
   - In the same Pages settings, enter `athenzadigital.com` under **Custom domain**.
   - Update your DNS at your domain registrar (Hostinger) with the GitHub Pages IPs:
     ```
     A records → 185.199.108.153
                 185.199.109.153
                 185.199.110.153
                 185.199.111.153
     CNAME record (optional) www → [username].github.io
     ```
   - Wait for DNS propagation (up to 24 hours, usually <1 hour).
   - Enable **Enforce HTTPS** in GitHub Pages settings.

### Option B: Deploy via Netlify (Alternative)
1. Sign up at [netlify.com](https://netlify.com) (free tier).
2. Drag & drop this folder onto the Netlify dashboard.
3. Netlify will provide a `.netlify.app` URL instantly.
4. For custom domain, follow Netlify's domain setup guide.

### Option C: Deploy via Cloudflare Pages
1. Sign in to Cloudflare Dashboard, go to **Pages**.
2. Connect your GitHub repository or upload this folder.
3. Configure build settings: no build command, output directory `/`.
4. Deploy. Free CDN and custom domain support included.

## Updating the Site
- Edit `index.html` for content changes.
- Logo files are in `assets/` – replace with new versions if needed.
- To change colors, update the `tailwind.config` section in `<head>`.
- After pushing changes to GitHub, the site auto‑updates within seconds.

## Form Handling
The contact form is currently client‑only (shows an alert). For production, connect to a form service:

1. **Formspree** (free tier): Replace `form` action with your Formspree endpoint.
2. **Netlify Forms**: If deploying on Netlify, add `data-netlify="true"` to the form tag.
3. **Custom backend**: Point to your own API endpoint.

## Performance Notes
- Tailwind CSS loaded via CDN (fast, no build step).
- Images are PNG logos; consider converting to WebP for smaller size.
- No external analytics scripts included; add Google Analytics if needed.

## Brand Assets
Colors (from brand guide):
- Deep Navy: `#051025`
- Royal Purple: `#7732A8`
- Slate Gray: `#555E6D`
- Off‑White: `#F3F4F4`

Font: **Inter** (loaded from Google Fonts)

## License
Proprietary – for Athenza Digital use only.

---

**Last Updated:** April 18, 2026  
**Built by:** Argos (OpenClaw Agent)
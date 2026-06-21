# AC Energy Partners — Website

ACΞNERGY — Manufacturer Representation • Energy Infrastructure • Market Development

This repository contains the static website for acenergypartners.com (GitHub Pages). The site is a minimal HTML/CSS site with a typographic (SVG) logo.

## Contents
- `index.html` — Home page (header, hero, Services, Industries, Why ACENERGY)
- `about.html` — About page
- `services.html` — Services & Industries
- `contact.html` — Contact information
- `styles.css` — Site styles
- `logo.svg` — SVG logo (ACΞNERGY / P A R T N E R S)
- `CNAME` — Custom domain: `acenergypartners.com`

## Local preview
To preview the site locally, open `index.html` in your browser, or run a simple HTTP server:

Python 3:
```
python3 -m http.server 8000
```
Then open http://localhost:8000

(Stop the server with Ctrl+C.)

## Publish (GitHub Pages)
1. Ensure the repository is pushed to GitHub (main branch).
2. Keep `CNAME` in the repo root with the single line:
```
acenergypartners.com
```
3. In the repo Settings → Pages:
   - Source: Branch `main` and folder `/ (root)`
   - Confirm the Custom domain is `acenergypartners.com` (or let the `CNAME` file handle it).
4. Add DNS records at your domain registrar:
   - A 185.199.108.153
   - A 185.199.109.153
   - A 185.199.110.153
   - A 185.199.111.153
   - CNAME `www` → `<your-github-username>.github.io`
5. Wait for DNS to propagate. GitHub Pages will provision HTTPS automatically once DNS is detected.

## How to update content
- Edit the HTML files (index/about/services/contact) and `styles.css`.
- Replace `logo.svg` with an updated SVG/PNG if needed.
- Commit and push:
```
git add .
git commit -m "Update site content"
git push origin main
```
Changes publish automatically.

## Logo & fonts
- `logo.svg` uses the Optos font if available. For consistent rendering, either host the webfont, embed it into the SVG, or use the provided font-independent SVG (if provided).
- If you want, convert text in the SVG to paths (I can do this) to avoid font dependency.

## Optional improvements
- Add a LICENSE file (e.g., MIT) if you want to specify reuse terms.
- Add a simple contact form integration (Formspree, Netlify Forms) instead of mailto.
- Add analytics (Google Analytics or Plausible) or a privacy policy page.

## Contact
If you want me to:
- create a ZIP of the site files — say: “ZIP please”
- push these files into a GitHub repo for you — provide `owner/repo` and confirm
- convert the SVG text to paths or embed the Optos font — say which option

Maintainer: mahdivid007 / AC Energy Partners  
Email: info@acenergypartners.com

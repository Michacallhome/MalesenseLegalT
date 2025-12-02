# MailSense Legal and Support Site

A simple static website for MailSense legal documentation and support information, designed for GitHub Pages hosting.

## Overview

This repository contains the legal and support pages for the MailSense mobile application. The site is built with plain HTML and inline CSS—no build tools, no JavaScript, no frameworks—making it perfect for GitHub Pages deployment.

## Main Pages

The site consists of four primary pages:

### 1. MailSenseHome.html
- **Purpose:** Landing page and app overview
- **Content:** Introduction to MailSense, feature highlights, and navigation to other pages

### 2. MailSensePrivacySummary.html
- **Purpose:** Privacy policy summary
- **Content:** What information MailSense collects, how it's used, user rights, and Google API compliance
- **Note:** Links to the full detailed privacy policy at privacy.html

### 3. MailSenseTerms.html
- **Purpose:** Terms of Service
- **Content:** Legal agreement, acceptable use, disclaimers, liability limitations, and platform-specific terms

### 4. MailSenseSupport.html
- **Purpose:** Support and contact information
- **Content:** How to contact support, response expectations, and helpful information

## File Structure

```
MalesenseLegalT/
├── index.html                      # Auto-redirects to MailSenseHome.html
├── MailSenseHome.html              # Main landing page
├── MailSensePrivacySummary.html    # Privacy policy summary
├── MailSenseTerms.html             # Terms of Service
├── MailSenseSupport.html           # Support page
├── privacy.html                    # Full detailed Privacy Policy (legacy)
├── terms.html                      # Legacy terms file (for backward compatibility)
├── support.html                    # Legacy support file (for backward compatibility)
├── test.html                       # Test file (not part of main site)
├── css/
│   └── style.css                   # External CSS (pages use inline CSS instead)
└── README.md                       # This file
```

## Features

- **Inline CSS:** All main pages have CSS embedded directly, so they work when opened locally or on any web server
- **Consistent Navigation:** All four main pages have identical navigation bars with the current page highlighted
- **Responsive Design:** Mobile-friendly layouts that work on phones, tablets, and desktops
- **No Build Tools:** Pure HTML and CSS - no JavaScript, no frameworks, no compilation needed
- **GitHub Pages Ready:** Uses relative links throughout for seamless deployment

## Local Testing

To test the site locally before deploying:

### Option 1: Double-Click
1. Open Finder and navigate to this folder
2. Double-click `index.html` (automatically redirects to MailSenseHome.html)
3. Click navigation links to test all four pages

### Option 2: Open Any MailSense File Directly
- Double-click any of the four main pages:
  - MailSenseHome.html
  - MailSensePrivacySummary.html
  - MailSenseTerms.html
  - MailSenseSupport.html
- Navigate between pages using the top navigation bar

### Option 3: Local Web Server (Optional)
```bash
cd /path/to/MalesenseLegalT
python3 -m http.server 8000
```
Then visit: `http://localhost:8000`

## GitHub Pages Deployment

### Enable GitHub Pages

1. Push this repository to GitHub (if you haven't already)
2. Go to your repository on GitHub
3. Click **Settings**
4. Scroll down and click **Pages** in the left sidebar
5. Under "Source", select:
   - **Branch:** `main`
   - **Folder:** `/ (root)`
6. Click **Save**
7. GitHub will build and deploy your site (usually takes 1-2 minutes)

### Your Site URLs

Once deployed, your site will be accessible at:

```
https://USERNAME.github.io/REPO/
https://USERNAME.github.io/REPO/MailSenseHome.html
https://USERNAME.github.io/REPO/MailSensePrivacySummary.html
https://USERNAME.github.io/REPO/MailSenseTerms.html
https://USERNAME.github.io/REPO/MailSenseSupport.html
```

Replace `USERNAME` with your GitHub username and `REPO` with your repository name.

**Example:** If your username is `johndoe` and your repo is `mailsense-legal`, your site will be at:
```
https://johndoe.github.io/mailsense-legal/
```

## Updating Content

### Editing Legal Text

The legal content in MailSensePrivacySummary.html and MailSenseTerms.html can be updated anytime:

1. Open the relevant .html file in any text editor
2. Edit the content within the `<main>` section
3. Save the file
4. Commit and push to GitHub
5. GitHub Pages will automatically rebuild (takes 1-2 minutes)

### Styling Changes

Each page has inline `<style>` tags in the `<head>` section. To change colors, fonts, or spacing:
1. Find the `<style>` section at the top of the file
2. Modify CSS properties as needed
3. Repeat for all four main pages to maintain consistency

## Navigation

All four main pages include an identical navigation bar:
- **Home** → MailSenseHome.html
- **Privacy** → MailSensePrivacySummary.html
- **Terms** → MailSenseTerms.html
- **Support** → MailSenseSupport.html

The current page is automatically highlighted using the `class="active"` attribute (pure CSS, no JavaScript).

## Legacy Files

The following files are kept for backward compatibility:
- `privacy.html` - Full detailed privacy policy
- `terms.html` - Original terms file
- `support.html` - Original support file

These files are clearly marked with HTML comments and can be removed once all external references have been updated to the new MailSense* filenames.

## Alternative Hosting

While this site is optimized for GitHub Pages, it can also be hosted on any static file hosting service (Netlify, Cloudflare Pages, Vercel, etc.) without modification, as it uses only relative paths and standard HTML/CSS.

## Contact

For questions about MailSense:
- Email: mailsense@callhomerealty.com

## License

Copyright © 2025 MailSense. All rights reserved.

## Notes

- This is a static legal and support site - no database, no server-side code
- All pages are self-contained and can be opened directly in a browser
- The site uses relative links throughout for maximum portability
- No external dependencies or CDN resources - everything is inline or local
- Legal text can be updated anytime by editing the HTML files directly

# CalSense Legal and Support Site

A simple static website for CalSense legal documentation and support information, designed for GitHub Pages hosting.

## Overview

This repository contains the legal and support pages for the CalSense mobile application. The site is built with plain HTML and inline CSS—no build tools, no JavaScript, no frameworks—making it perfect for GitHub Pages deployment.

## Main Pages

The site consists of four primary pages:

### 1. CalSenseHome.html
- **Purpose:** Landing page and app overview
- **Content:** Introduction to CalSense, feature highlights for real estate professionals, and navigation to other pages

### 2. CalSensePrivacySummary.html
- **Purpose:** Privacy policy summary
- **Content:** What information CalSense collects (calendar data via iOS EventKit), how it's used, user rights, and data protection

### 3. CalSenseTerms.html
- **Purpose:** Terms of Service
- **Content:** Legal agreement, acceptable use, disclaimers, liability limitations, and subscription terms

### 4. CalSenseSupport.html
- **Purpose:** Support and contact information
- **Content:** FAQs, how to contact support, troubleshooting tips, and response expectations

## File Structure

```
MalesenseLegalT/
├── index.html                      # Auto-redirects to CalSenseHome.html
├── CalSenseHome.html               # Main landing page
├── CalSensePrivacySummary.html     # Privacy policy summary
├── CalSenseTerms.html              # Terms of Service
├── CalSenseSupport.html            # Support page with FAQs
├── privacy.html                    # Redirect to CalSensePrivacySummary.html
├── terms.html                      # Redirect to CalSenseTerms.html
├── support.html                    # Redirect to CalSenseSupport.html
├── test.html                       # Test file (not part of main site)
├── CNAME                           # Custom domain: callhomerealty.com
├── google259d692baaf66964.html     # Google domain verification
└── README.md                       # This file
```

## Features

- **Inline CSS:** All main pages have CSS embedded directly, so they work when opened locally or on any web server
- **Consistent Navigation:** All four main pages have identical navigation bars with the current page highlighted
- **Responsive Design:** Mobile-friendly layouts that work on phones, tablets, and desktops
- **No Build Tools:** Pure HTML and CSS - no JavaScript, no frameworks, no compilation needed
- **GitHub Pages Ready:** Uses relative links throughout for seamless deployment
- **Custom Domain:** Configured for callhomerealty.com via CNAME

## Local Testing

To test the site locally before deploying:

### Option 1: Double-Click
1. Open Finder and navigate to this folder
2. Double-click `index.html` (automatically redirects to CalSenseHome.html)
3. Click navigation links to test all four pages

### Option 2: Open Any CalSense File Directly
- Double-click any of the four main pages:
  - CalSenseHome.html
  - CalSensePrivacySummary.html
  - CalSenseTerms.html
  - CalSenseSupport.html
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
https://callhomerealty.com/
https://callhomerealty.com/CalSenseHome.html
https://callhomerealty.com/CalSensePrivacySummary.html
https://callhomerealty.com/CalSenseTerms.html
https://callhomerealty.com/CalSenseSupport.html
```

## Updating Content

### Editing Legal Text

The legal content in CalSensePrivacySummary.html and CalSenseTerms.html can be updated anytime:

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
- **Home** → CalSenseHome.html
- **Privacy** → CalSensePrivacySummary.html
- **Terms** → CalSenseTerms.html
- **Support** → CalSenseSupport.html

The current page is automatically highlighted using the `class="active"` attribute (pure CSS, no JavaScript).

## Legacy Redirects

The following files redirect to the new CalSense pages for backward compatibility:
- `privacy.html` → CalSensePrivacySummary.html
- `terms.html` → CalSenseTerms.html
- `support.html` → CalSenseSupport.html

## Alternative Hosting

While this site is optimized for GitHub Pages, it can also be hosted on any static file hosting service (Netlify, Cloudflare Pages, Vercel, etc.) without modification, as it uses only relative paths and standard HTML/CSS.

## Contact

For questions about CalSense:
- Email: support@callhomerealty.com

## License

Copyright 2025 CalSense by Call Home Realty. All rights reserved.

## Notes

- This is a static legal and support site - no database, no server-side code
- All pages are self-contained and can be opened directly in a browser
- The site uses relative links throughout for maximum portability
- No external dependencies or CDN resources - everything is inline or local
- Legal text can be updated anytime by editing the HTML files directly

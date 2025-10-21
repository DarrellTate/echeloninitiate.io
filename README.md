# 🛰️ Echelon: Initiate Protocol

[![Build and Deploy](https://github.com/DarrellTate/echeloninitiate.io/actions/workflows/pages.yml/badge.svg)](https://github.com/DarrellTate/echeloninitiate.io/actions)
[![GitHub last commit](https://img.shields.io/github/last-commit/DarrellTate/echeloninitiate.io?logo=git&color=00bcd4)](https://github.com/DarrellTate/echeloninitiate.io/commits/main)
[![GitHub release (latest by date)](https://img.shields.io/github/v/release/DarrellTate/echeloninitiate.io?logo=github&color=ff9800)](https://github.com/DarrellTate/echeloninitiate.io/releases)
[![Website Status](https://img.shields.io/website?url=https%3A%2F%2Fecheloninitiate.com&label=Live%20Site&logo=vercel&color=00e676)](https://echeloninitiate.com)

> **Project Status:** 🟢 Active  
> **Live Site:** [https://echeloninitiate.com](https://echeloninitiate.com)

---

## 🧠 Overview

**Echelon: Initiate Protocol** is a cinematic, high-concept interactive web experience currently in pre-launch.  
Built with **Next.js**, deployed via **GitHub Pages**, and integrated with **Google Analytics 4** for performance tracking.

The current version serves as a **“Phase One” Coming Soon splash portal**, designed for progressive expansion into a full interactive experience.

---

## ⚙️ Tech Stack

| Category | Technology |
|-----------|-------------|
| Framework | [Next.js 14](https://nextjs.org) |
| Language | TypeScript, JavaScript (ES6+) |
| Styling | Native CSS Modules |
| Deployment | GitHub Pages (`output: 'export'`) |
| CI/CD | GitHub Actions |
| Analytics | Google Analytics 4 (Measurement ID: `G-YBE44VQ069`) |

---

## 🛠️ Local Development Setup

Follow these steps to run the project locally or contribute changes.

### 1. Prerequisites

Make sure you have the following installed:

- [Node.js 18+](https://nodejs.org/en/download)
- [npm 9+](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
- [Git](https://git-scm.com/downloads)

Check your versions:
bash
node -v
npm -v
git --version

### 2. Clone the repository
bash
Copy code
git clone https://github.com/DarrellTate/echeloninitiate.io.git
cd echeloninitiate.io

### 3. Install dependencies
bash
Copy code
npm install
If you encounter peer dependency warnings, run:

bash
Copy code
npm install --legacy-peer-deps

### 4. Run the development server
bash
Copy code
npm run dev
Then open your browser to:

arduino
Copy code
http://localhost:3000
You’ll see the Echelon: Initiate Protocol splash screen running locally.

### 5. Build and Export for Production
bash
Copy code
npm run build
This will:

✅ Build and optimize your Next.js application.

✅ Automatically export static files to the /out directory (ready for GitHub Pages).

### 6. Export Static Site (handled automatically)
The static site export process happens automatically during the build step —
you do not need to run any extra commands.

This behavior is controlled by your project’s configuration file:

📄 File: next.config.mjs

js
Copy code
export default {
  output: 'export',
  images: { unoptimized: true },
};
These options tell Next.js to:

✅ Generate a fully static build (no Node.js server needed)

✅ Disable server-based image optimization for GitHub Pages compatibility

### 7. Run the Production Preview (optional)
After building, preview the static output locally:

bash
Copy code
npx serve out
Then visit:

arduino
Copy code
http://localhost:5000
🚀 Deployment Pipeline (CI/CD)
Every push to the main branch automatically triggers a GitHub Actions workflow that:

Installs dependencies (npm ci)

Builds and exports static content

Deploys the /out directory to GitHub Pages

You can view deployment logs here:
➡️ GitHub Actions – Pages Workflow

📈 Analytics Integration
This site uses Google Analytics 4 (GA4) for page view and engagement tracking.

Measurement ID: G-YBE44VQ069

The tracking script is embedded in the <head> of the app for all environments:

html
Copy code
<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-YBE44VQ069"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-YBE44VQ069');
</script>
🧩 Branch Workflow
Branch	Purpose
main	Production-ready code automatically deployed to GitHub Pages
feature/*	Used for feature development or experimental updates
dev (optional)	Can be used for local staging or preview builds

Standard workflow:

bash
Copy code
# Create a new feature branch
git checkout -b feature/update-homepage

# Commit your changes
git add .
git commit -m "feat(ui): update homepage animation"

# Push to remote
git push origin feature/update-homepage

# Merge to main after review
git checkout main
git merge feature/update-homepage
git push origin main
🧠 Version History
Version	Date	Notes
v1.0.0	Oct 2025	Migrated to Next.js and deployed static build
v1.0.1	Oct 2025	Added GA4 analytics and updated documentation
v1.1.0	Planned	Add interactive animations and game intro logic

🎨 Brand & Visual Identity
Asset	Description
logo.png	Full logo with title text
logo_no_text.png	Standalone geometric emblem used in-game and as favicon
favicon.png	150×150 square icon for browser tab

All branding elements © 2025 Echelon Initiative — used for both the web and Unity game assets.

🧑‍💻 Author
Darrell Tate
GitHub · Portfolio

"Enter the next phase of the protocol."
© 2025 Echelon Initiative. All rights reserved.

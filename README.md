# Dragonfly Campaign Studio

A modern, responsive campaign planning and moodboard creation tool for social media managers, content creators, and marketing teams.

## Features

- **Visual Campaign Planning**: Create and organize campaign elements visually
- **Multi-Platform Support**: Pre-configured dimensions for Instagram, TikTok, Facebook, Twitter, LinkedIn, YouTube, and Pinterest
- **Drag & Drop Interface**: Easily reorder cards with intuitive drag and drop (desktop and mobile)
- **Image Integration**: Upload images, use URL links, or search Unsplash directly
- **Project Management**: Save campaigns as projects and load them later
- **Export Options**: Export as PDF, PNG, or calendar events (ICS)
- **Scheduling**: Schedule posts with browser notifications
- **Filters**: Filter cards by platform and schedule status
- **Responsive Design**: Works on desktop, tablet, and mobile devices
- **Local Storage**: All data saved in browser's local storage

## Project Structure

```

dragonfly-campaign-studio/ ├── index.html              # Main HTML file ├── css/ │   ├── style.css          # Main styles │   └── components.css     # Component-specific styles ├── js/ │   ├── main.js            # Core functionality │   ├── drag-drop.js       # Drag and drop implementation │   ├── projects.js        # Project management │   ├── export.js          # Export functions (PDF, PNG, Calendar) │   ├── scheduling.js      # Scheduling and notifications │   └── unsplash.js        # Unsplash image search ├── netlify/ │   └── functions/ │       └── unsplash-proxy.js  # Netlify function for Unsplash API ├── .gitignore             # Git ignore file ├── README.md              # This file └── netlify.toml           # Netlify deployment config

```

## Setup Instructions

### Local Development

1. **Clone or download** this repository
2. **Open index.html** in your browser to view the site locally
3. **For development**:
   - Edit HTML in `index.html`
   - Edit styles in `css/` folder
   - Edit scripts in `js/` folder

### Unsplash API Setup (for image search)

To enable Unsplash image search, you need to:

1. Sign up for an Unsplash API key at [Unsplash Developers](https://unsplash.com/developers)
2. Create a Netlify account at [netlify.com](https://netlify.com)
3. Deploy to Netlify (see below)
4. Add your Unsplash API key as an environment variable in Netlify

## Deployment to Netlify

### Step 1: Push to GitHub
bash
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/YOUR_USERNAME/dragonfly-campaign-studio.git
git push -u origin main


Step 2: Deploy to Netlify

1. Go to Netlify.com
2. Click "New site from Git"
3. Connect to your GitHub repository
4. Deploy with these settings:
   · Build command: (leave empty)
   · Publish directory: . (dot)
5. Click "Deploy site"

Step 3: Add Unsplash API Key

1. In Netlify dashboard, go to your site
2. Go to Site settings → Environment variables
3. Add a new variable:
   · Key: UNSPLASH_ACCESS_KEY
   · Value: Your Unsplash API access key
4. Redeploy your site (trigger a new deploy)

Usage Guide

Creating Cards

1. Fill in the title and description in the sidebar
2. Select a platform (dimensions auto-adjust)
3. Click "Add to Moodboard"

Editing Cards

· Click on any card image or content to edit
· Add images via upload, URL, or Unsplash search
· Schedule posts with date/time and notifications

Managing Projects

· Click the folder icon to open Projects
· Save current moodboard as a project
· Load, export, or share projects

Exporting

· Click the share icon to open Export hub
· Export as PDF, PNG, or Calendar events
· Share campaign links

Filtering

· Click the filter icon to show filter panel
· Filter by platform or schedule status
· Clear filters individually or all at once

Browser Support

· Chrome (latest)
· Firefox (latest)
· Safari (latest)
· Edge (latest)
· iOS Safari
· Android Chrome

Technologies Used

· HTML5
· CSS3 (with CSS Grid and Flexbox)
· Vanilla JavaScript (ES6+)
· Font Awesome Icons
· jsPDF for PDF export
· html2canvas for image export
· Local Storage API
· Notifications API
· Intersection Observer
· Touch Events API

License

© 2024 Dragonfly Campaign Studio. All rights reserved.

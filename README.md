# Customer-Facing Mobile Apps Portfolio

This repository powers a GitHub Pages site showcasing mobile apps with screenshots, descriptions, and download links. It is designed for customers.

## Adding apps and screenshots

- Edit `assets/apps.json` and add:
  - `slug`: short URL-friendly identifier (e.g., `tenant-app`)
  - `screenshots`: list of image paths
  - Optional `demo`: `{ "type": "youtube" | "mp4", "url": "..." }`

- Place images under `assets/images/<slug>/`:
  - `cover.jpg` (main image)
  - `1.jpg`, `2.jpg`, `3.jpg`... (screenshots)

- The detail page is at `app.html?app=<slug>` and will render screenshots in a gallery. Clicking a screenshot opens a lightbox. If `demo` is set, a video is embedded.

## Publish via GitHub Pages

Settings → Pages → “Deploy from a branch” → Branch: `main` → Folder: `/root`.  
Site URL: `https://fayedgouda.github.io/portfolio`

## Importing projects from a CV

Paste your projects using this JSON template and commit to `assets/apps.json`, or send the CV text and I’ll convert it:

```json
{
  "name": "App Name",
  "slug": "app-name",
  "tagline": "Short value proposition",
  "description": "Customer-friendly description.",
  "platforms": ["iOS","Android"],
  "links": { "ios": "...", "android": "...", "website": "..." },
  "highlights": ["Feature 1","Feature 2"],
  "screenshots": ["assets/images/app-name/1.jpg","assets/images/app-name/2.jpg"],
  "demo": { "type": "youtube", "url": "https://www.youtube.com/watch?v=VIDEO_ID" }
}
```
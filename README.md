# Customer-Facing Mobile Apps Portfolio

This repository powers a simple GitHub Pages site to showcase mobile apps with screenshots, descriptions, and download links. It is designed for customers, not developers.

## How to add or edit apps

1. Add your app entry in [`assets/apps.json`](assets/apps.json) using this structure:
   ```json
   {
     "name": "Your App Name",
     "tagline": "Short value proposition",
     "description": "Customer-friendly description of your app (avoid technical jargon).",
     "image": "assets/images/your-app/cover.jpg",
     "platforms": ["iOS", "Android"],
     "links": {
       "ios": "https://apps.apple.com/app/id...",
       "android": "https://play.google.com/store/apps/details?id=...",
       "website": "https://yourappsite.com"
     },
     "highlights": ["Feature 1", "Feature 2", "Feature 3"]
   }
   ```

2. Place your screenshot image at `assets/images/your-app/cover.jpg`. If no image exists yet, the site will use the placeholder automatically.

3. Commit and push. The site will automatically render the updated list.

## Publish via GitHub Pages

1. Go to the repository Settings → Pages.
2. Set Source to `Deploy from a branch`.
3. Choose `main` (or your default branch) and `/root`.
4. Save. Your site will be available at:
   - `https://fayedgouda.github.io/portfolio`

## Customization

- Colors and layout: edit `assets/styles.css`
- Contact info: update the links in `index.html`

## Accessibility

- Images include alt text
- Buttons have clear labels
- High-contrast, responsive design
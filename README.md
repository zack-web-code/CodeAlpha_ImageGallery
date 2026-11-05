# LUMEN — A space for art

A responsive HTML/CSS/JavaScript gallery with 20 selected artworks: four each in Abstract, Landscape, Architecture, Photography and Other. Each work has a short interpretive story.

## Run locally

Open C:\Projects\CodeAlpha_ImageGallery in VS Code. Right-click index.html and choose Open with Live Server. Keep the same address and port to access your saved uploads.

## Faster image loading

- 320px and 640px WebP thumbnails selected for screen size.
- Grid cards request previews only when within 180px of the viewport.
- Complete 1200px artwork images load only when opened in the lightbox.
- Content-hashed image filenames and Netlify browser-cache headers.
- Two automatic retries plus a manual retry on failed cards.

## Features

Search, categories, favourites, light/dark themes, full-window lightbox, fullscreen, arrow-key navigation, and personal uploads with title, artist, category and description. Uploaded images, edits and favourites persist in IndexedDB.

Uploads stay in this browser on this device and do not become public website content. Clearing site data removes personal uploads. Keep original files as backups. Existing curated artwork IDs and database name are preserved; favourites for pieces outside this selection are excluded from the displayed count.

## Deploy

Commit the project and push to GitHub, then deploy the latest commit on Netlify. Build command: empty. Publish directory: dot (.). No dependencies or build step. The _headers file belongs beside index.html. Old unused image files can remain in an existing checkout; the gallery references only these 20 works.

## Artwork credits

See CREDITS.md for artists and source records. The public gallery and lightbox show stories without source wording. assets/exhibition contains only the selected works and their preview variants.

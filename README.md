# LUMEN Art Gallery

LUMEN is an interactive digital art gallery built with HTML, CSS, and JavaScript. It brings together a curated exhibition and a personal collection where visitors can add their own work.

**Repository:** https://github.com/zack-web-code/LUMEN_ArtGallery

## The exhibition

The gallery includes 20 selected works, with four pieces in each category: Abstract, Landscape, Architecture, Photography, and Other. Each artwork has a short accompanying story. Artist and source information is documented in [`CREDITS.md`](CREDITS.md).

## Features

- Search and category filtering
- Artwork favourites
- Responsive gallery layout and dark/light themes
- Full-window image viewer, fullscreen mode, and keyboard navigation
- Personal artwork uploads with title, artist, category, and description
- Editing and removing personal uploads
- Local persistence for uploads and favourites using IndexedDB
- Responsive image previews and lazy loading for faster browsing

Personal uploads stay in the browser on the device where they were added. They do not become part of the public exhibition and are not uploaded to a server. Clearing browser site data can remove uploaded artwork, so keep the original image files.

## Built with

- HTML5
- CSS3
- JavaScript
- IndexedDB

## Run locally

1. Clone or download this repository.
2. Open the project folder in VS Code.
3. Open `index.html` with Live Server.

No package installation or build step is required for viewing the site. Use the same local address and port when returning to access saved artwork.

## Project files

- `index.html` — Gallery page with initial styles and artwork previews
- `app.js` and `collection.js` — Gallery interactions and collection data
- `styles.css` — Stylesheet used by the credits page and as the source for home-page styles
- `assets/exhibition/` — Artwork images and responsive previews
- `CREDITS.md` — Artwork credits and source information
- `_headers` — Caching instructions for supported hosts
- `tools/sync-inline-style.cjs` — Synchronises updated styles into the home page

The first three previews are embedded for a faster initial display, while the remaining previews load as needed. Full-resolution images are loaded when an artwork is opened in the viewer.

### Updating styles

The homepage includes a copy of the CSS for faster initial rendering. After changing `styles.css`, run:

```bash
node tools/sync-inline-style.cjs
```

This keeps the embedded homepage styles in sync.

## Deployment

The project can be hosted as a static website on GitHub Pages or Netlify. No build command is required. For Netlify, set the publish directory to the repository root (`.`).

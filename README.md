# LUMEN — Digital Art Gallery

A modern, futuristic digital art gallery built with HTML, CSS and vanilla JavaScript. No build step, account or external dependencies.

## Getting started

Serve the folder with any local web server (for example the Live Server extension in VS Code) and open `index.html`.

## Features

- 44 local artworks: 8 Abstract, 8 Landscape, 8 Architecture, 10 Photography and 10 Other
- Category filters, search, and collection views (exhibition, my artwork, favourites)
- Upload, edit and delete your own artwork (JPG, PNG, WebP, GIF, AVIF up to 15 MB)
- Favourites, dark/light theme, full-window lightbox with fullscreen and arrow-key navigation
- Fully responsive, keyboard accessible, respects reduced-motion settings

## Privacy

Uploads are stored only in your browser on this device and are never sent to a server.

## Credits

The six original LUMEN Studio pieces are no longer displayed. The 44 added fine-art images are sourced from Wikimedia Commons records marked Public domain or CC0. See CREDITS.md or the Artwork credits page for individual artists, source links and licence labels.

## Expanded collection

Open the project folder in VS Code, right-click index.html, and choose **Open with Live Server**. No internet connection is needed to display the artworks. Source wording and links are removed from the exhibition and lightbox. Provenance remains in the project’s credit files. Keep using the same hostname and port to retain access to your existing browser-saved uploads and favourites.

collection.js holds the 44 new catalogue entries. assets/collection/ holds the corresponding WebP files. The existing app, theme, categories, curated artwork IDs and IndexedDB database name are retained.

## Artwork stories

Each artwork now has its own short interpretive caption directly beneath the title, also used in the lightbox. Captions describe the visual mood and composition rather than presenting invented historical events. Existing portraits and uploaded artwork remain available.

## Image loading update

The same 44 artworks are bundled as optimized WebP files. The first row loads eagerly, images decode asynchronously, and transient failures retry twice. Select an unavailable image card to try again.

# Breathe Safe Technologies

Lightweight production website for Breathe Safe Technologies, a healthy-buildings and indoor-air-quality company serving Central Florida.

## Structure

- `index.html` — page content, metadata, navigation, and Netlify form markup
- `styles.css` — responsive layout and visual design
- `script.js` — navigation, reveal effects, and inline form feedback
- `assets/` — optimized brand and photography assets
- `favicon.png` — browser icon
- `robots.txt` and `sitemap.xml` — search-engine discovery files
- `netlify.toml` — static publish directory and basic response headers

## Preview locally

From this folder, run:

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## Editing

Edit page text and metadata in `index.html`. Edit layout, typography, colors, and responsive behavior in `styles.css`. Replace photographs in `assets/` while retaining the existing filenames and image proportions when possible.

## Assessment form

The form in `index.html` uses Netlify Forms with the form name `assessment-request`, a matching hidden `form-name` field, browser validation, and the `company-website` honeypot. `script.js` submits URL-encoded form data directly to Netlify and presents an inline success or error message. No frontend secret or custom backend is required.

After deployment, submissions are available in the Netlify project’s Forms area. Notification rules can be configured in Netlify without changing public frontend code.

## Deploy to Netlify

Connect the repository to Netlify and use the repository root as the publish directory. No build command is required. Confirm that Netlify detects the `assessment-request` form after the first production deployment.

## Image provenance

- `family-room.webp` is derived from the Pexels photograph “Bright Family Room with Children by a Window” by Daniel & Hannah Snipes: https://www.pexels.com/photo/bright-family-room-with-children-by-a-window-29973441/
- `hero-interior.webp` and `workplace.webp` are optimized copies of the two Unsplash CDN images used in the approved design. Their exact photographer/source-page records were not available in the approved source. Confirm and retain those records before commercial launch, or replace the files with source-documented copies of the same approved images.
- Breathe Safe logo and favicon artwork are project brand assets.

The production images have been resized where appropriate and stripped of embedded metadata.

# Matrix Red for Jellyfin

A black and red Jellyfin custom CSS theme based on the ElegantFin structure, restyled with a darker Matrix-inspired look, red accents, stronger hover effects and compatibility across desktop, web, TV and mobile layouts.

## Preview

### Home
![Home view](screenshots/home-view.png)

### Library
![Library view](screenshots/library-view.png)

### Detail page
![Detail view](screenshots/detail-view.png)

### Cast and recommendations
![Cast view](screenshots/cast-view.png)

### Sidebar
![Sidebar view](screenshots/sidebar-view.png)

## Credits

- **Base structure:** ElegantFin v25.12.31 by **lscambo13**
- **Reskin:** Matrix Red black and red customisation
- **Platform:** Jellyfin

This theme keeps the ElegantFin layout philosophy and adapts it into a red and black visual style.

## Features

- Black and red colour palette
- ElegantFin-style layout and spacing
- Stronger red card shimmer on hover
- Red play buttons and active states
- Styled sidebar, tabs, detail pages and overlays
- Support for plugins such as MediaBar, HomeSections, MDBList, FileTransformation, Playback Reporting, Covers, Intro Skipper and Fanart

## Files

- `matrix-red.css` , the custom CSS theme file
- `screenshots/` , preview images for the repository page

## How to import the custom CSS into Jellyfin

1. Open Jellyfin in your browser.
2. Go to **Dashboard**.
3. Open **General**.
4. Scroll to **Custom CSS**.
5. Open the `matrix-red.css` file from this repository.
6. Copy all of its contents.
7. Paste the CSS into the **Custom CSS** box in Jellyfin.
8. Click **Save**.
9. Hard refresh Jellyfin with `Ctrl + F5`.
10. If the old styling still appears, clear the browser cache or reload the Jellyfin desktop app.

## Recommended GitHub structure

```text
matrix-red-jellyfin/
├── README.md
├── matrix-red.css
└── screenshots/
    ├── home-view.png
    ├── library-view.png
    ├── detail-view.png
    ├── cast-view.png
    └── sidebar-view.png
```

## Notes

- This repo is intended for GitHub upload as a simple theme repository.
- If you edit the theme later, keep screenshots updated so the repository preview matches the current CSS.
- If you fork or redistribute it, keep the ElegantFin credit in place.

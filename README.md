# The Portal Project

A community-made PC launcher and mod catalog for LEGO Dimensions, with an authentic ToyPad-inspired experience for Wii U / Cemu setups.

## Website

The project website is a lightweight static site:

- `index.html` is the English-language landing page.
- `assets/css/styles.css` contains its responsive styling.
- `assets/images/` is ready for project artwork and screenshots.
- `mods.json` provides the data shown in the community mod catalog.

To preview the website, serve the repository root with any static web server and open its local address. The mod catalog uses `fetch`, so it needs to be served over HTTP rather than opened directly as a `file://` page.

## Launcher

Use the **Get the launcher** link on the website to visit the latest project release on GitHub. If no release is available yet, check the repository for updates.

## Mod catalog format

Add catalog entries to `mods.json` using this structure:

```json
[
  {
    "id": "example-pack",
    "name": "Example Pack",
    "description": "A short description of the community mod.",
    "downloadUrl": "https://example.com/example-pack.zip"
  }
]
```

Use a direct HTTPS download URL for each published mod.

## Disclaimer

This is an unofficial, fan-made project and is not affiliated with, sponsored, authorized, or endorsed by the LEGO Group. LEGO and LEGO Dimensions are trademarks of the LEGO Group.

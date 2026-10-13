# The Portal Project

A community-made PC launcher and mod catalog for LEGO Dimensions, with an authentic ToyPad-inspired experience for Wii U / Cemu setups.

## Website

The project website is a lightweight static site:

- `index.html` is the English-language landing page.
- `assets/css/styles.css` contains its responsive styling.
- `assets/images/logo.png` is the LEGO Dimensions logo used on the page.
- `assets/images/icon.png` is used for the browser tab icon and site branding.
- `mods.json` provides the data shown in the community mod catalog.

To preview the website, serve the repository root with any static web server and open its local address. The mod catalog uses `fetch`, so it needs to be served over HTTP rather than opened directly as a `file://` page.

## Launcher

The website's launcher buttons download `assets/launcher/LEGO-Dimensions-Launcher.exe` directly. Add the Windows installer at that path when it is ready; the download buttons are prepared but the executable is not included yet.

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

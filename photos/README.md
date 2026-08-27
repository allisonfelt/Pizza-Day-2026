Photos for the site go in this folder.

## The easy way

Name your files and drop them in. Nothing else to edit.

- `hero.jpg` — the big photo at the top of the page
- `01.jpg`, `02.jpg`, `03.jpg` … up to `12` — the gallery

`.jpg`, `.jpeg`, `.png` and `.webp` all work. iPhone `.heic` files do **not** —
convert them to JPEG first (on a Mac: open in Preview, File → Export, Format
JPEG). Resize anything wider than ~2000px so the page stays quick to load.

## If you want captions

Open `index.html`, find the `PHOTOS` array near the bottom, and fill it in.
Listing anything there switches off the automatic numbering, so include every
photo you want shown:

```js
var PHOTOS = [
  { file: "01.jpg", caption: "Putting in at Steelhead" },
  { file: "02.jpg", caption: "All eight slices, accounted for" },
];
```

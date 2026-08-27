# Pizza Day 2026

A one-page site for the Russian River float trip — Sunday, August 30, 2026.
Steelhead Beach to Sunset Beach.

It's a single static file. Open `index.html` in a browser and it works; there's
no build step and no dependencies.

## Adding photos

1. Put image files in `photos/`
2. Open `index.html`, scroll to the `PHOTOS` array near the bottom, and list them:

```js
var PHOTOS = [
  { file: "steelhead.jpg", caption: "Putting in at Steelhead" },
  { file: "unicorn.jpg",   caption: "" },
];
```

## Editing the details

Everything lives in `index.html`:

| What | Where to look |
|---|---|
| Times | the `<section id="day">` timeline and the `.daybar` segments |
| Who's in which car | `<section id="cars">` |
| The shuttle steps | `<section id="shuttle">` |
| Gear and snacks, claimed vs. open | `<section id="gear">` / `<section id="snacks">` |
| Packing list | the `ITEMS` array in the script |
| Map | the `#riverline` path in `<section id="map">` |

## Publishing it

The repo is private. To put it on the web for free with GitHub Pages, make it
public (Settings → General → Danger Zone → Change visibility), then go to
Settings → Pages and set the source to `main` / `/ (root)`.

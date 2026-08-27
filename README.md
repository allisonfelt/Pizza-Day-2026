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

Live at **https://allisonfelt.github.io/Pizza-Day-2026/**

Hosting is GitHub Pages. To turn it on (one time only): Settings -> Pages ->
Source: "Deploy from a branch" -> `main` / `/ (root)` -> Save. After that every
push to `main` redeploys automatically within a minute or so.

## Link previews

`share-card.jpg` is the 1200x630 image that shows up when the link is pasted
into iMessage, Slack, etc. The Open Graph tags at the top of `index.html` point
at it with absolute URLs, because link scrapers will not resolve relative ones.
If the repo or its URL ever changes, those tags need updating too.

iMessage caches previews aggressively. If a thread is showing a stale one, add
a query string (`?v=2`) to force a refetch.

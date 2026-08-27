Put photos for the site in this folder.

Then open `index.html`, scroll to the bottom, and add each filename to the
`PHOTOS` array:

```js
var PHOTOS = [
  { file: "steelhead.jpg", caption: "Putting in at Steelhead" },
  { file: "unicorn.jpg",   caption: "" },
];
```

Any format a browser can show works (.jpg, .png, .heic won't — convert those
to .jpg first). Resize anything over ~2000px wide so the page stays fast.

# Ethereum Library

A single-page reading library for Ethereum, cryptography, and decentralized systems. Inspired by the visual style of Erik's [cypherpunkbooks.com](https://www.cypherpunkbooks.com/).

## Features

- **Animated hero** — staggered rise-in title set in Syne, with a CTA into the collection.
- **3D bookshelf** — perspective-tilted shelf of book spines; hover for a title/author caption, click to open the collection.
- **Searchable collection** — live filtering across titles and authors.
- **Grid & list views** — toggle between cover-card grid and a compact list.
- **Light / dark themes** — toggle in the nav, full palette swap via CSS variables.
- **Responsive** — adapts from mobile to desktop.
- **Zero build step** — everything is in one `index.html`. Fonts (Inter, Syne) load from Google Fonts.

## Running

Open `index.html` directly in a browser, or serve the folder:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Editing the book list

Books live in the `BOOKS` array near the bottom of `index.html`. Each entry:

```js
{ title: "Snow Crash", author: "Neal Stephenson", year: 1992,
  section: "Fiction", color: "#3d5a80", h: 380, t: 28 }
```

- `color` — spine / cover background.
- `h` — book height on the 3D shelf (px).
- `t` — book thickness on the shelf (px).
- `section` — category label (stored; not yet shown as visible headers).

## Structure

```
index.html    # markup, styles, and logic in one file
README.md
```

## License

MIT.

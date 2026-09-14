# cs2340port

Personal portfolio site for CS 2340 — built with plain HTML/CSS/JS, deployed via GitHub Pages.

## Structure

- `index.html` — landing page (name, tagline, nav)
- `about.html` — introduction / about you
- `gt-movies.html` — GT Movies Store: overview, screens/features & user stories, process, video demo
- `assets/style.css` — shared styles (light/dark theme via the toggle in the top right)
- `assets/theme.js` — light/dark theme toggle logic

## Editing content

All the text that needs to be filled in is marked in `[brackets]` and styled in italics
(`.placeholder` class) — search for `[` in `about.html` and `gt-movies.html` to find every
spot that needs real content.

To embed the demo video in `gt-movies.html`, replace the `.video-placeholder` div inside
`.video-frame` with either:

```html
<iframe src="https://www.youtube.com/embed/VIDEO_ID" title="GT Movies Store demo" allowfullscreen></iframe>
```

or, for a self-hosted video file:

```html
<video controls src="assets/demo.mp4"></video>
```

## Local preview

Just open `index.html` in a browser, or run a tiny local server from this folder:

```bash
python3 -m http.server 8000
```

then visit `http://localhost:8000`.

## Deployment

This repo is deployed with GitHub Pages from the `main` branch (root). Any push to `main`
updates the live site automatically within a minute or two.

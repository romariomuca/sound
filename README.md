# Romario — The sound of nature

Short audiovisual pieces exploring the synthetic connection between sound and nature.
In every piece, image and sound come from the same score: nothing on screen moves unless a note asks it to.
Nothing is filmed or sampled — everything is generated in code.

**Series:** Poetry · Nature · Symphony
**Best with headphones.**

## The site

A single static page, no build step and no dependencies.

```
index.html     the whole site (HTML, CSS and JavaScript in one file)
v/             the videos (4:5, 600×750, H.264 + AAC)
q/             poster frames for the grid
me.jpg         portrait for the About page
favicon.svg    tab icon
.nojekyll      tells GitHub Pages to serve the files as they are
```

Fonts (Parkinsans and IBM Plex Mono) load from Google Fonts.

### Links to a single work

Every work has its own address, for example `#sym-4` (Gong) or `#poe-1` (Infinity). `#about` opens the About page.

### Sound

Browsers keep audio locked until the visitor's first click or key press. The site opens in the
"Sound on" state and starts playing at the first click anywhere on the page. The S key toggles sound.

## Publish on GitHub Pages

1. Create a new public repository on GitHub (for example `sound-of-nature`).
2. Upload everything in this folder, keeping the `v/` and `q/` folders, or push it with git:
   ```
   git init
   git add .
   git commit -m "The sound of nature"
   git branch -M main
   git remote add origin https://github.com/<your-username>/sound-of-nature.git
   git push -u origin main
   ```
3. In the repository go to **Settings → Pages**, set **Source** to *Deploy from a branch*,
   choose `main` and `/ (root)`, and save.
4. After a minute the site is live at `https://<your-username>.github.io/sound-of-nature/`.

## Preview locally

Open a terminal in this folder and run `python3 -m http.server`, then visit http://localhost:8000.
(Opening `index.html` by double-click also works, but the live sound visualisation needs a local server.)

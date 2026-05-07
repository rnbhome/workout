# Strength Log

A personal daily strength training journal — tracks 18 exercises across mobility, lower body, and upper body work. Mobile-first, paper-journal aesthetic, single-file HTML with persistent in-browser storage.

Each exercise card shows a custom illustration with the movement's trajectory (start position → end position).

## Live demo

Once you've deployed (steps below), it'll be at `https://YOUR-USERNAME.github.io/REPO-NAME/`.

## Deploy to GitHub Pages

### One-time setup

1. Create a new repo on GitHub. Make it **public** (Pages on free accounts requires public).
2. Locally:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/REPO-NAME.git
   git push -u origin main
   ```
3. On GitHub, go to **Settings → Pages**.
4. Under **Source**, select **Deploy from a branch**, branch `main`, folder `/ (root)`. Save.
5. Wait ~1 minute. Your app is live at the URL Pages shows you.

### Updating later

Edit, then:
```bash
git add .
git commit -m "Update"
git push
```

Pages redeploys automatically.

## File structure

```
.
├── index.html          # The whole app — open this directly in a browser to test locally
├── svgs/               # 18 standalone exercise illustrations (also embedded in index.html)
│   ├── pushup-holds.svg
│   ├── thoracic-rotation.svg
│   └── ... (16 more)
└── README.md
```

## Local testing

Just open `index.html` in any browser — no build step, no server needed. Storage uses `localStorage` so your data persists per-browser.

## Tech

Plain HTML / CSS / JS. No framework, no build tools. Fonts loaded from Google Fonts (Fraunces + Inter). All 18 illustrations are inline SVG embedded in the HTML — the `svgs/` folder is just there if you want to reuse them elsewhere.

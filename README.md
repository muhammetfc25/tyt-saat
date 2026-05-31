# TYT / AYT Ultra Pro

Static exam timer web app with PWA support.

## Run locally

### Option 1: Open directly in browser
1. Open `e:\Html\Tyt-sayac\index.html` in your browser.
2. This works for UI review, but service worker features may be limited when using `file://`.

### Option 2: Use VS Code Live Server
1. Open this folder in VS Code.
2. Install the Live Server extension if needed.
3. Right-click `index.html` and choose `Open with Live Server`.
4. The app will launch at a local `http://127.0.0.1:5500/...` address.

### Option 3: Use a local HTTP server
From this folder, run one of these commands:

```powershell
python -m http.server 5500
```

or

```powershell
npx http-server . -p 5500
```

Then open `http://127.0.0.1:5500/` in your browser.

## Test / verify

- Confirm the timer UI updates when you click `BAŞLAT`.
- Switch between `TYT` and `AYT` modes.
- Check the progress bar and remaining time values.
- Test fullscreen mode by clicking the fullscreen button.
- Open DevTools > Application > Service Workers to verify `sw.js` is registered.
- Optionally install the app from browser install prompts.

## Files

- `index.html` — main app UI and script
- `manifest.json` — PWA metadata
- `sw.js` — offline caching service worker
- `icons/` — PWA icons
- `.gitignore` — ignored files for git

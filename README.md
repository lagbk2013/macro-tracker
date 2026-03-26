# Macro Tracker — Deployment Guide

## Files in this folder
- index.html     → the full app
- manifest.json  → PWA config (makes it installable)
- sw.js          → service worker (offline support)
- icons/         → app icons for home screen

---

## Hosting on GitHub Pages (free, takes ~5 minutes)

### Step 1 — Create a GitHub account
Go to https://github.com and sign up if you don't have one.

### Step 2 — Create a new repository
1. Click the "+" icon top right → "New repository"
2. Name it: macro-tracker
3. Set it to Public
4. Click "Create repository"

### Step 3 — Upload your files
1. On the new repo page, click "uploading an existing file"
2. Drag and drop ALL files from this folder:
   - index.html
   - manifest.json
   - sw.js
   - icons/icon-192.png
   - icons/icon-512.png
3. Click "Commit changes"

### Step 4 — Enable GitHub Pages
1. Go to Settings → Pages (left sidebar)
2. Under "Branch", select: main → / (root)
3. Click Save
4. Wait ~60 seconds, then your URL will appear:
   https://YOUR_USERNAME.github.io/macro-tracker/

---

## Adding to your iPhone home screen

1. Open Safari on your iPhone (must be Safari, not Chrome)
2. Go to your GitHub Pages URL
3. Tap the Share button (box with arrow pointing up)
4. Scroll down and tap "Add to Home Screen"
5. Name it "Macros" and tap Add

It will appear on your home screen like a native app —
full screen, dark mode, no browser chrome.

---

## Notes
- Your food log is saved on-device in localStorage
- Data does NOT sync across devices (private by design)
- The app works offline once loaded (service worker caches it)
- Barcode lookup requires internet connection

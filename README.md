# ⚡ Shaolin Bolt — Twitch Overlay System

A fully custom, animated overlay package built for the **Bolt Dojo** — designed for clean gameplay, real vibes, and steady improvement.  
This repository hosts all overlay files and serves them through GitHub Pages for easy OBS integration.

---

## ⚡ Live Overlay URL

Use this link in OBS as a Browser Source:

https://shaolinbolt.github.io/shaolin-bolt-overlays/

---

## ⚡ Features

- Starting Soon, BRB, Ending, Just Chatting, and Gameplay screens  
- Clean, modern, electric‑blue aesthetic  
- Lightweight HTML/CSS overlays  
- Hosted via GitHub Pages  
- Updates go live instantly in OBS

---

## ⚡ How to Use in OBS

1. Open OBS  
2. Add → Browser Source  
3. Paste the overlay URL  
4. Set:
   - Width: 1920  
   - Height: 1080  
5. Click OK  
6. Your overlay loads instantly

---

## ⚡ Editing the Overlay

All customization happens through:

- index.html  
- style.css  
- config.json

### New / important config keys
- `background` — path to the background image (string)
- `logo` — path to the logo image (string)
- `mainTitle` — main heading text (string)
- `subTitle` — secondary heading text (string)
- `mainColor` — primary color for titles (CSS color string)
- `subColor` — optional subtitle color (CSS color string). If omitted, it falls back to `mainColor`.

If config.json fails to load, the overlay now uses sensible defaults so the stream doesn't go blank.

### Fonts
The overlay loads the Montserrat font from Google Fonts. If you prefer to self-host or use a different font, update `index.html` and `style.css`.

### Accessibility
- Images include `alt` text.
- Titles use `aria-live="polite"` so screen readers get updates.
- `prefers-reduced-motion` is respected and animation is disabled for those users.

### Multiple overlays / presets
To create additional overlays (BRB, Gameplay, etc.):
- Add new JSON files (e.g., `brb.json`, `gameplay.json`) with the same keys.
- Replace `config.json` with the desired preset or host multiple configs and update index.html to accept a query parameter for switching (I can add that behavior if you want).

---

## ⚡ File Structure

shaolin-bolt-overlays/
│
├── index.html  
├── style.css  
├── config.json  
├── assets/  
│   ├── backgrounds/  
│   ├── logos/  
│   └── elements/  
└── README.md

---

## ⚡ About the Bolt Dojo

A community built on:

- Respect  
- Clean gameplay  
- No ego  
- Steady improvement  
- Electric energy

Welcome to the dojo.
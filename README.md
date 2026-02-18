# EarAssist — Audio Assist + Optional Live Captions (PWA)

EarAssist is a **browser-based hearing assist tool** powered by the **Web Audio API**.
It can boost and shape microphone audio in real time (EQ + filters + limiter + “smart gate”), and can optionally show **live captions** for situations where hearing is difficult.

**Privacy:** runs locally in your browser. No accounts. No server.  
**Note:** This is an assistive tool, not a medical device.

## What’s new in v7
- ✅ **No sticky header** (scrolls normally)
- ✅ **No horizontal side-scroll on mobile** (LP slider + layout fixed)
- ✅ Header controls are **bigger / more touch-friendly**
- ✅ Captions section included + documented

## Features
- 🎛 EQ: Gain, High‑pass, Low‑pass  
- 🧰 Filters: Presence Boost, Smart Gate (soft floor), 60 Hz Notch  
- 🛡 Assist: Calibrate Noise, Medical AGC, Limiter, Emergency Boost  
- 💬 Optional Live Captions (speech-to-text in supported browsers)  
- 📊 Visualizer: Wave / Spectrum / Split  
- 🎨 Themes: Dark / Light / Solar / Ocean / Orange  
- 💾 Presets: Save/Load to localStorage  
- 📱 PWA-ready: install to Home Screen (after caching)

## Quick Start
1. Open `index.html` in **Chrome / Edge** (recommended).
2. Allow microphone permission.
3. Choose your **Mic** and **Output**, then press **Start**.
4. Try **Assist (Medical)** preset.
5. In a quiet moment, press **Calibrate Noise**.
6. If you need text help, toggle **Live Captions**.

## Audio Quality + Stability Tips (important)
If you hear “on/off” audio or fluctuating captions:
- **Avoid speaker-to-mic feedback.** Use headphones. Speakers can re-enter the mic and confuse both the gate and captions.
- **Bluetooth can add latency/echo.** If you notice echo, try wired headphones or low‑latency earbuds.
- **Smart Gate:** if speech is being chopped, increase **floor** (softens silence) by switching to **Assist (Medical)** or turning Gate off temporarily.
- Keep **Limiter** on to prevent sudden loud spikes.

## Captions Notes
- Captions rely on the browser’s Speech Recognition API (best in Chrome).
- Recognition accuracy improves when the mic is close to the speaker’s mouth and when background audio is minimized.

## Install as a PWA
- Serve over **HTTPS** (GitHub Pages works).
- Visit the page and choose **Install / Add to Home Screen**.
- After first load, it works offline (cached by the service worker).

## Files
- `index.html` — app (single-file UI + audio + captions)
- `manifest.json` — PWA manifest
- `sw.js` — service worker cache
- `icon-192.png`, `icon-512.png` — app icons

## License
MIT (you can change this if you want).
## ⚠️ Important (Medical / Safety)
EarAssist is **not a medical device** and is **not a substitute** for professional hearing care.
Use it as an assistive tool. Keep volume at a safe level to protect your hearing.


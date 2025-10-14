# AirAssist v4 — All-In-One (PWA)

AirAssist is a **browser-based hearing assist tool** powered by the Web Audio API.  
It enhances microphone input with EQ, filters, limiter, AGC, and one-click noise calibration.  
Runs entirely offline in the browser — no backend, no account.

## ✨ Features
- 🎛 EQ: Gain, High-pass, Low-pass
- 🧰 Filters: Presence Boost, Noise Gate, 60 Hz Notch
- 🛡 Assist: Calibrate Noise, Auto-Gain (AGC), Limiter
- 💾 Presets: Save/Load to localStorage
- 🎨 Themes: Dark / Light / Solar / Ocean / Orange
- 📊 Visualizer: Wave, Spectrum, Split
- 🎤 Devices: Mic & Output selection, latency display
- ⌨️ Keyboard: S Start, X Stop, M Mute, 1/2/3 Presets

## 🚀 Quick Start
1. Open `index.html` in Chrome/Edge (or deploy on GitHub Pages).
2. Allow microphone permission.
3. Select mic + output, click **Start**.
4. Try a preset, then click **Calibrate Noise** in a quiet moment.

## 📦 As a PWA
- Already PWA-ready (manifest + service worker included).
- Deploy on GitHub Pages → visit site → “Install” / “Add to Home Screen”.
- Works offline once cached.

## 🧩 Browser Support
- Best: Chrome / Edge (supports mic + output switching).
- Firefox: works, some limitations.
- iOS Safari: mic works only over HTTPS.

## 🛠 Troubleshooting
- No mic input? → Check browser permissions.
- No sound? → Select correct output.
- High latency? → Prefer wired headphones.

## 🗺 Roadmap
- [ ] Noise suppression
- [ ] Ultra-low latency via AudioWorklet
- [ ] Scene profiles (Restaurant, Street, Lecture)
- [ ] Export/import presets
- [ ] Peak meter & clipping indicator

## 📄 License
MIT

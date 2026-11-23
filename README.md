# Veloce v1.2 — Hybrid Training, Nutrition & Recovery Tracker

Veloce v1.2 is a mobile-first web application designed for tracking hybrid strength and cardio training, daily recomp nutrition, body metrics, and recovery—with per-account Google OAuth isolation and Garmin Connect / iOS Health sync support.

---

## Files to Upload to GitHub

Upload all **4 files** from `Veloce_v1.2_GitHub_Files.zip` into the root folder of your GitHub repository (and enable **GitHub Pages** from the `main` branch):

| File | Description |
| :--- | :--- |
| `index.html` | Main web application with Google OAuth, reorderable week blocks, superset timer, recomp nutrition plan, and Garmin/iOS Health sync. |
| `veloce-icon.png` | Full-bleed `512×512` sunrise app icon (coral rose → amber → emerald mint gradient with white lightning bolt & wave) for iOS `apple-touch-icon` and browser favicon. |
| `manifest.json` | Web App Manifest enabling standalone full-screen launch and proper icon registration on iOS and Android. |
| `README.md` | Documentation and iOS Home Screen installation guide. |

---

## Features

- **Per-Account Google OAuth Sign-In:** Isolates training logs, nutrition plans, and health records per verified Google account in `localStorage`.
- **Bright Sunrise-Inspired Palettes & Modes:** Includes **Bright Dark** and **Bright Light** modes paired with four vibrant color palettes in **Settings** (`Sunrise Coral & Mint`, `Solar Citrus & Lime`, `Electric Lagoon & Sky`, and `Neon Berry & Emerald`).
- **Superset Rest Timer:** Quick `60s` and `90s` presets, customizable default rest duration, play/pause/reset controls, and Web Audio chime alerts.
- **Reorderable Weekly Training Blocks:** Seven-day hybrid split (Anterior Chain, Intervals/Tempo Run, Posterior Chain, Pool Swim/Recovery, Full Body Hybrid, Zone 2 Endurance, and Shabbat Rest/Mobility) that can be reordered on the fly.
- **Strength & Cardio Logging:** Track exercises, weights/reps, RPE, running/swimming duration, distance, average heart rate, and active calories.
- **Structured Recomp Nutrition Plan:** Built around a morning fasted window, a 12:00 high-protein first meal, afternoon protein mini-meals, training-scaled dinners, a planned evening sweet/chocolate, and flexible Shabbat guidelines.
- **Body Metrics & Net Energy Balance:** Track body weight, abdomen circumference, calories in vs. out, resting heart rate (RHR), and sleep duration.
- **Garmin Connect & iOS Health Sync:** Supports Auto-Sync Bridge URLs (Google Apps Script / webhooks / iOS Shortcuts), JSON payload pasting, file imports (`.csv`, `.xml`, `.json`), and Quick Sync entry.

---

## Add to iPhone / iPad Home Screen (with Sunrise Icon)

1. Upload `index.html`, `veloce-icon.png`, `manifest.json`, and `README.md` to your GitHub Pages repository root and wait ~1 minute for GitHub Pages to publish.
2. Remove the old **Veloce** shortcut from your iPhone Home Screen (touch and hold → **Remove App** → **Remove from Home Screen**).
3. Open your GitHub Pages URL in **Safari** on iOS.
4. Tap the **Share** button (`□↑`) → **Add to Home Screen**.
5. Confirm the sunrise lightning icon appears in the preview, tap **Add**, and move it into your **בריאות וכושר** folder.

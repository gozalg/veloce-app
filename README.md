# Veloce v1.2 — Hybrid Training, Nutrition & Recovery Tracker

Veloce v1.2 is a single-file, mobile-first web application designed for tracking hybrid strength and cardio training, daily recomp nutrition, body metrics, and recovery—with per-account Google OAuth isolation and Garmin Connect / iOS Health sync support.

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

## Quick Start

1. **Open Locally or Host on GitHub Pages:**
   - Open `index.html` directly in any modern browser, or deploy the repository via **GitHub Pages** (`Settings` → `Pages` → deploy from `main` branch).
2. **Sign In:**
   - Use the Google Sign-In button on the gate screen to open your personal workspace.
3. **Customize Appearance & Timer:**
   - Tap the gear icon (`⚙`) in the top-right header to switch between **Bright Dark** / **Bright Light**, choose a **Color Palette** (`Sunrise`, `Citrus`, `Lagoon`, or `Berry`), and configure your default rest timer and audio chime.

---

## Add to iPhone / iPad Home Screen

1. Open your hosted `index.html` URL in **Safari** on iOS.
2. Tap the **Share** button (`□↑`) in the Safari toolbar.
3. Scroll down and select **Add to Home Screen**.
4. Confirm the **Veloce** app icon and tap **Add**.

---

## Backup & Data Portability

- Use the **JSON** export button in the **Body & kcal** tab at any time to download a complete backup (`Veloce_v1.2_YYYY-MM-DD.json`) of your training logs, body metrics, and weekly block order.

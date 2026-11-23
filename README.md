# Veloce v1.0

Minimalist weekly training block planner, strength/cardio logger, and Garmin + iOS Health sync tracker built as a single-file web app (`index.html`).

## Quick Setup (GitHub Pages)

1. Upload `index.html` and `README.md` to the root of your GitHub repository.
2. Open **Settings → Pages**.
3. Under **Build and deployment → Branch**, choose `main` and `/ (root)`, then click **Save**.
4. Open `https://<your-username>.github.io/<repo-name>/` in Safari on iPhone and tap **Share → Add to Home Screen**.

## Features

- **Per-User Profile Lock:** Enter your email + 4+ character PIN to keep your logs and schedule separate per user in browser storage.
- **Movable Sun–Sat Week Blocks:** Reorder or swap **Zone 2**, **Anterior**, **Intervals/Tempo**, **Posterior**, **Swim/Recovery**, **Full Body**, and **Rest** blocks across Sunday–Saturday using `↑ / ↓` or the dropdown menu.
- **Built-In Rest Timer:** Quick `60s` and `90s` superset countdown timer with audio chime.
- **Strength, Cardio & Body/kcal Logs:** Track sets/RPE, runs/treadmill/swims, weight, abdominal circumference, net calories, and RHR/sleep.
- **Garmin & iOS Health Sync:** Supports file import (`.CSV`, `.XML`, `.JSON`), JSON payload paste, Quick Sync, and automated polling from a JSON Bridge URL.

## Automated iPhone Sync Setup (Apps Script + Shortcuts)

1. Go to [script.google.com](https://script.google.com) → **New project**, paste `Code.gs`, and click **Deploy → New deployment → Web app**.
2. Set **Execute as:** `Me` and **Who has access:** `Anyone`, then copy the Web App URL.
3. In the iPhone **Shortcuts** app, create a shortcut using **Find Health Samples** (Weight, Waist Circumference, Dietary Energy, Active/Resting Energy, Resting Heart Rate, Sleep) and **Get Contents of URL** (`POST` JSON) to send your daily summary to the Web App URL:

```json
{
  "body": [
    {
      "date": "2026-11-23",
      "w": 80.0,
      "abd": 85.0,
      "calIn": 2100,
      "calOut": 2500,
      "rhr": 55,
      "sleep": 7.5
    }
  ],
  "cardio": [
    {
      "date": "2026-11-23",
      "type": "Run",
      "min": 40,
      "dist": 6.5,
      "hr": 140,
      "kcal": 420
    }
  ]
}
```

4. Schedule the Shortcut under **Shortcuts → Automation** (e.g., daily morning or when opening Safari).
5. Open **Veloce v1.0 → Sync & Health**, paste the Web App URL into **Auto-Sync Bridge URL**, set **Auto-Pull Interval (min)** (e.g., `60`), and tap **Sync Now**.
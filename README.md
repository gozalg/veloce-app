# Veloce v1.1

Veloce v1.1 is a browser-based hybrid training, strength, cardio, body metrics, nutrition, and recovery tracker hosted on GitHub Pages (`https://gozalg.github.io/veloce-app/`).

## Authentication & Security
- **Google OAuth 2.0 Sign-In Only:** Local PIN/email sign-in has been removed. Sessions are verified via Google OAuth 2.0 and scoped per Google account (`sub`) in browser storage (`localStorage` and `sessionStorage`).
- **Google Cloud Console Setup:**
  - **Authorized JavaScript origins:** `https://gozalg.github.io`
  - **Authorized redirect URIs:** `https://gozalg.github.io/veloce-app/`
- **Client ID Visibility:** The Google OAuth Web Client ID is public in client-side code by design (no Client Secret is stored in `index.html`), and sign-in is restricted to approved origins and redirect URIs.

## Features & Controls
- **Sport App Icon & Branding:** Custom SVG sport lightning-bolt icon used in the header, sign-in card, favicon, and `apple-touch-icon`.
- **Larger Rest Timer with Icon Controls:** Preset buttons (`60s`, `90s`), larger digital readout, and icon-only Play (`▶`), Pause (`❚❚`), and Reset (`↺`) controls.
- **Settings Modal (`⚙`):** Choose the app **Theme** (`Dark` or `Light`), set default timer preset seconds, toggle audio chime (`on`/`off`), and reset weekly blocks.
- **Nutrition Tab (`Nutrition`):** Tailored for age 36 body recomposition (muscle gain + fat loss) with a morning fasted window, first meal starting at 12:00, afternoon snacks, a budgeted evening chocolate/sweet treat, and a flexible, low-restriction Shabbat approach.
- **Workout & Body Trackers:** Manage weekly blocks (`Week Blocks`), log workouts (`Strength`, `Cardio`), track weight, abdomen circumference, calories in/out, RHR, and sleep (`Body & kcal`), and export JSON backups.

## Garmin & iOS Health Sync
- **Auto-Sync Bridge URL:** Connect a JSON endpoint (webhook, shortcut, or feed) and optionally enable an auto-pull interval in minutes.
- **JSON Payload Paste / Template:** Copy the sample JSON template, paste payloads, and apply them directly.
- **File Import (`.CSV`, `.XML`, `.JSON`):** Import Garmin CSV activity exports, Apple Health XML/JSON exports, or JSON payloads.
- **Quick Sync:** Enter daily workout, calorie, body, RHR, and sleep values in one place to update logs and KPI cards.
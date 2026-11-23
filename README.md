# Veloce v1.1

Veloce v1.1 is a browser-based hybrid training, strength, cardio, body metrics, and recovery tracker hosted on GitHub Pages (`https://gozalg.github.io/veloce-app/`).

## Authentication & Security
- **Google OAuth 2.0 Sign-In Only:** Local PIN/email sign-in has been removed. Sessions are verified via Google OAuth 2.0 and scoped per Google account (`sub`) in browser storage (`localStorage` and `sessionStorage`).
- **Google Cloud Console Setup:**
  - **Authorized JavaScript origins:** `https://gozalg.github.io`
  - **Authorized redirect URIs:** `https://gozalg.github.io/veloce-app/`
- **Client ID Visibility:** The Google OAuth Web Client ID is public in client-side code by design (no Client Secret is stored in `index.html`), and sign-in is restricted to approved origins and redirect URIs.

## Features & Controls
- **Sport App Icon & Branding:** Custom SVG sport lightning-bolt icon used in the header, sign-in card, favicon, and `apple-touch-icon`.
- **Larger Rest Timer with Icon Controls:** Preset buttons (`60s`, `90s`), larger digital readout, and icon-only Play (`▶`), Pause (`❚❚`), and Reset (`↺`) controls.
- **Settings Modal (`⚙`):** Configure default timer preset seconds, audio chime (`on`/`off`), Google Client ID, and quick navigation to the sync tab or schedule reset.
- **Workout & Body Trackers:** Manage weekly blocks (`Week Blocks`), log workouts (`Strength`, `Cardio`), track weight, abdomen circumference, calories in/out, RHR, and sleep (`Body & kcal`), and export JSON backups.

## Garmin & iOS Health Sync
- **Auto-Sync Bridge URL:** Connect a JSON endpoint (webhook, shortcut, or feed) and optionally enable an auto-pull interval in minutes.
- **JSON Payload Paste / Template:** Copy the sample JSON template, paste payloads, and apply them directly.
- **File Import (`.CSV`, `.XML`, `.JSON`):** Import Garmin CSV activity exports, Apple Health XML/JSON exports, or JSON payloads.
- **Quick Sync:** Enter daily workout, calorie, body, RHR, and sleep values in one place to update logs and KPI cards.

# Veloce v1.2 — Hybrid Training, Nutrition & Recovery Tracker

Veloce v1.2 is a mobile-first web application designed for tracking hybrid strength and cardio training, daily recomp nutrition, body metrics, and recovery—with per-account Google OAuth isolation and Garmin Connect / iOS Health sync support.

---

## Files to Upload to GitHub

Upload all **4 files** from `Veloce_v1.2_GitHub_Files.zip` into the root folder of your GitHub repository (and enable **GitHub Pages** from the `main` branch):

| File | Description |
| :--- | :--- |
| `index.html` | Main web application with resilient Google OAuth initialization, reorderable week blocks, superset timer, recomp nutrition plan, and Garmin/iOS Health sync. |
| `veloce-icon.png` | Full-bleed `512×512` sunrise app icon (coral rose → amber → emerald mint gradient with white lightning bolt & wave) for iOS `apple-touch-icon` and browser favicon. |
| `manifest.json` | Web App Manifest enabling standalone full-screen launch and proper icon registration on iOS and Android. |
| `README.md` | Documentation and iOS Home Screen installation guide. |

---

## Troubleshooting Google Sign-In on GitHub Pages & iOS Home Screen

1. **Host Over `https://`:** Always open your GitHub Pages `https://` URL rather than viewing `index.html` inside a file or code preview viewer.
2. **Authorized JavaScript Origins in Google Cloud Console:** Confirm that `https://gozalg.github.io` (your exact origin, with no trailing slash or path) is listed under **Authorized JavaScript origins** for Client ID `385961340567-tv5pc07h1c0r4t3t9dlrd1v64vq225fu.apps.googleusercontent.com`.
3. **Safari & Home Screen Web App Settings:** On iOS, check **Settings → Safari** for **Prevent Cross-Site Tracking** or content blockers if the Google sign-in widget is slow or blocked, and use the **Load Google Sign-In** button if you want an immediate manual retry.

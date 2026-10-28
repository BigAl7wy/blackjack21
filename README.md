# 21 (Blackjack) — Android APK & PWA Bundle

This package contains your complete **21 (Blackjack)** game configured for **100% offline play** and ready to turn into an Android `.apk` via either **PWABuilder (No-Code)** or **Capacitor + Android Studio (Local Build)**.

## Included Files
- `index.html` & `www/index.html` — Your complete 14-step **21 (Blackjack)** game wired up with PWA metadata, app icons, and offline Service Worker registration.
- `tailwind-offline.css` & `www/tailwind-offline.css` — Pre-built offline stylesheet so the table, cards, chips, and drawers render without an internet connection.
- `manifest.json` & `www/manifest.json` — Web App Manifest configured for standalone portrait mode on Android.
- `sw.js` & `www/sw.js` — Offline-first Service Worker that caches all game assets on first launch.
- `icon-192.png` & `icon-512.png` — Custom emerald-and-gold **21** app icons.
- `package.json` & `capacitor.config.json` — Ready-to-run Capacitor configuration for Android Studio.

## Option 1: Fastest No-Code APK (PWABuilder + GitHub Pages)
1. Unzip this folder and upload the root files (`index.html`, `tailwind-offline.css`, `manifest.json`, `sw.js`, `icon-192.png`, `icon-512.png`) to a free GitHub repository and enable **GitHub Pages** in `Settings -> Pages`.
2. Copy your live `https://<username>.github.io/<repo>/` URL and paste it into https://www.pwabuilder.com/.
3. Click **Package for Stores -> Android -> Download Package** to download your signed `.apk` file ready to install on your phone.

## Option 2: Local Offline APK Build (Capacitor + Android Studio)
1. Unzip this folder on your computer and open a terminal inside it.
2. Run:
   ```bash
   npm install
   npx cap add android
   npx cap open android
   ```
3. In **Android Studio**, wait for Gradle sync to finish, then click **Build -> Build Bundle(s) / APK(s) -> Build APK(s)** to export your standalone `app-debug.apk`.

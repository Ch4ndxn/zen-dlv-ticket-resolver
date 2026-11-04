# ZEN-DLV Ticket Resolver

Android WebView app for the ZEN fleet dispatch console with background GPS tracking.

**URL:** `https://fleetops-dispatch-master-data-console.onrender.com/#/track`

## Features
- Full-screen WebView loading the dispatch console
- Background GPS via Android ForegroundService (keeps tracking when minimized)
- Persistent notification while tracking is active
- Grants Geolocation permission automatically to the WebView

## Build (GitHub Actions — no Android Studio needed)

1. Push to `main` → GitHub Actions runs automatically
2. Go to **Actions → Build Unsigned APK → latest run → Artifacts**
3. Download `ZEN-DLV-Ticket-Resolver-unsigned.zip` → extract the `.apk`

## Install on device
Since the APK is unsigned you need to allow installation from unknown sources:
1. Enable **Settings → Security → Install unknown apps** for your file manager
2. Transfer the APK to the device and tap to install

> To sign properly, generate a keystore and add signing config in `app/build.gradle`.

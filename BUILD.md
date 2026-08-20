# Cubit Head Offices — APK Build Instructions

## What this project is
Web UI (`www/`) packaged for Android via Capacitor.

- **App ID:** `inc.cubitsystems.headoffices`
- **App name:** Cubit Head Offices
- **Web dir:** `www/` (already contains the office UI)

## On a machine with Node + Android Studio

```bash
cd cubit-apk
npm install @capacitor/core@6 @capacitor/cli@6 @capacitor/android@6 --legacy-peer-deps
npx cap add android
npx cap sync android
npx cap open android
```

In Android Studio:
1. Build → Build Bundle(s) / APK(s) → Build APK(s)
2. Copy the debug APK from `android/app/build/outputs/apk/debug/`

## First test
1. Transfer APK to phone
2. Follow the **APK Run Card**
3. Kai runs **APK Acceptance Checklist**

## Release later
- Generate a release keystore (Founder holds secrets)
- Sign release APK
- Only then public drop CTA

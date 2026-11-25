# Hoops Manager — Offline Android APK Project

This project wraps the self-contained `Hoops_Manager_684eddb9.html` game inside a native Android `WebView` using `WebViewAssetLoader` so `IndexedDB` (`hm_db`), `localStorage`, and haptics run 100% offline with zero network permissions.

## Option 1: Build APK on GitHub (No Android Studio Required)
1. Create a new GitHub repository and upload all files from this ZIP.
2. Open the **Actions** tab and run **Build Offline Android APK** (or push to `main`).
3. Download the compiled `hoops-manager-offline-apk` artifact containing `app-debug.apk`, transfer it to your Android phone, and install.

## Option 2: Build Locally with Android Studio or Gradle CLI
1. Open this folder in **Android Studio**.
2. Let Gradle sync, then choose **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
3. Or from a terminal with Gradle 8.10+ & Android SDK installed:
   ```bash
   gradle assembleDebug
   ```
   Output APK: `app/build/outputs/apk/debug/app-debug.apk`.

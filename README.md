# SOLAL – Wise Words (Android project)

This is the Android Studio project for the SOLAL-branded version of the original Wise Words app. It wraps the original offline HTML app in a native Android WebView so its quote library, Mind section, category filters, search, daily quote, favourites, theme choice, copy and share behavior are retained.

## Build the APK

1. Install Android Studio (current stable) and Android SDK Platform 35.
2. Open this folder in Android Studio.
3. Let Gradle sync complete.
4. Choose **Build → Build Bundle(s) / APK(s) → Build APK(s)**.
5. Android Studio creates the debug APK at `app/build/outputs/apk/debug/app-debug.apk`.

The included GitHub Actions workflow can also build a debug APK: push this folder to a GitHub repository and run **Actions → Build SOLAL APK**. The generated APK is available as a workflow artifact.

## App details

- App name: SOLAL – Wise Words
- Package: `com.solal.wisewords`
- Minimum Android: 6.0 (API 23)
- Offline-first: app content is bundled locally; saved favourites and theme use WebView local storage.
- No account or internet permission is required.

A debug APK is suitable for personal installation/testing. A separately signed release APK is needed for Play Store distribution.

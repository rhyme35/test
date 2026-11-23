# PYRO-BENCH Native Android App

Native Kotlin + OpenGL ES 2.0 Android stress-testing app with real device thermal, battery temperature, and system RAM telemetry.

## Build a Downloadable APK (2 Options)

### Option 1: Build in the Cloud with GitHub Actions (No Local Android Studio Needed)
1. Create a new GitHub repository and upload all files from this folder (including `.github/workflows/build-apk.yml`).
2. Open the **Actions** tab in your GitHub repository and run **Build PYRO-BENCH APK** (or let it trigger automatically on push).
3. When the build finishes (~2 minutes), download **pyro-bench-debug-apk** from the run's **Artifacts** section and install `app-debug.apk` on your Android phone.

### Option 2: Build Locally (Android Studio or CLI)
- **Android Studio:** Open this folder in Android Studio, let Gradle sync, then select **Build -> Build Bundle(s) / APK(s) -> Build APK(s)**.
- **Command Line (Linux/macOS/Windows with JDK 17, Gradle 8.9+, and Android SDK 35):**
  ```bash
  gradle assembleDebug
  ```
  The installable APK will be generated at `app/build/outputs/apk/debug/app-debug.apk`.

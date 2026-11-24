# FinCalc India — Android APK Build Guide

Because `.apk` files must be compiled using the Android SDK and Gradle, this repository is pre-configured with **GitHub Actions** to compile your APK automatically in the cloud.

## Steps to Generate & Download Your APK

1. **Create a GitHub Repository**
   - Go to [github.com/new](https://github.com/new) and create a new repository (e.g., `FinCalc-India`).

2. **Upload All Project Files**
   - Extract `FinCalc-India-Android.zip` and upload all files/folders into your GitHub repository while keeping the exact folder structure:
     - `index.html`
     - `build.gradle`
     - `settings.gradle`
     - `gradle.properties`
     - `app/build.gradle`
     - `app/src/main/AndroidManifest.xml`
     - `app/src/main/java/com/fincalc/india/MainActivity.java`
     - `.github/workflows/build-apk.yml`

3. **Run the GitHub Actions Workflow**
   - Pushing the files to `main` (or `master`) will automatically start the **Build FinCalc India Android APK** workflow.
   - Or open the **Actions** tab in your GitHub repository -> click **Build FinCalc India Android APK** -> click **Run workflow**.

4. **Download & Install on Android**
   - Once the build turns green (~2 minutes), click on the workflow run.
   - Scroll down to **Artifacts** and download **`FinCalc-India-Android-APK`**.
   - Unzip it on your Android phone to get `app-debug.apk` and tap to install.

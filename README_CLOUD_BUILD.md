# Build NexaVision AI on GitHub Actions

This project includes a GitHub Actions workflow at:
`.github/workflows/android-apk.yml`

It uses a GitHub-hosted Ubuntu runner, Java 17, Gradle 8.9, and Android SDK 35 to build the debug APK. The finished APK is uploaded as a workflow artifact named `NexaVision-AI-debug-apk`.

## Phone-only route
1. Create a GitHub repository and upload the **contents of the `NexaVisionAI` folder** (not the outer ZIP folder).
2. Open the repository's **Actions** tab.
3. Select **Build NexaVision AI APK**.
4. Tap **Run workflow**.
5. Wait for the green check mark.
6. Open the workflow run and download **NexaVision-AI-debug-apk**.
7. Extract `app-debug.apk` and install it on the Android phone.

GitHub Actions is a cloud CI/CD service. This avoids requiring Android Studio to run on the phone itself. The Android project remains the same; this workflow only supplies a legitimate cloud build environment.

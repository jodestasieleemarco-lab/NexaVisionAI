# NexaVision AI — Android phase

Application ID: `com.nexavision.ai`

This is the Android WebView shell for the existing NexaVision AI prototype. The analysis engine is kept in the local web layer so the existing prototype interface can be inserted without changing the strategy.

## Data adapter
The web layer exposes a Twelve Data adapter interface. Twelve Data supports 5m, 15m, 1h and 4h intervals and forex symbols such as EUR/USD. API keys must be supplied by the user/app backend and must not be hard-coded into the APK.

## Build
Open this directory in Android Studio and sync Gradle. Build an APK with the normal Android Studio Build APK action.

Note: this environment does not have an Android SDK/Gradle installation, so an APK cannot be compiled here; the Android project source is ready for Android Studio.

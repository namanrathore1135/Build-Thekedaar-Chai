# Thekedaar Chai — Android app project

A small offline-first tea-shop manager with a Hindi + English interface and a warm chai-brown/cream design.

## Included
- Billing and order history
- Menu and selling-price / per-item-cost management
- Daily sales, order count, expense and estimated-profit dashboard
- Expense tracking
- Customer records
- JSON backup and restore
- Local on-device storage (no account or server required)

## Build the APK
1. Install **Android Studio** (current stable) and its Android SDK (API 35).
2. Open this folder in Android Studio.
3. Let Gradle sync and install any requested Android SDK components.
4. Select **Build → Build Bundle(s) / APK(s) → Build APK(s)**.
5. Android Studio will show the APK location, usually `app/build/outputs/apk/debug/app-debug.apk`.
6. Transfer that APK to your Android phone and install it. If prompted, allow installation from that source.

## Important notes
- This deliverable is the complete Android Studio project source, not a compiled APK binary. The build environment used to prepare it did not have the Android SDK or Gradle installed, so an APK could not be compiled here.
- Records are stored locally in the app's WebView storage on that device. Clearing app data or uninstalling may erase records; use **Reports → Download backup** regularly.
- Profit is an estimate: order item costs are captured at the time of sale, then recorded expenses are subtracted. Enter realistic per-item costs in the menu.
- This starter version has no cloud sync, GST invoice compliance, online payments, or multi-device sharing.

## Cloud build (no Android Studio required on your computer)
This project includes `.github/workflows/build-apk.yml`.
1. Create a GitHub repository and upload the contents of this project.
2. Open the repository's **Actions** tab and run **Build Thekedaar Chai APK** (or push to `main`).
3. Open the completed workflow run and download the `ThekedaarChai-APK` artifact.
4. Extract the artifact to get `app-debug.apk`.

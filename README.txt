DASSY TAILORING BOOK — ANDROID APK BUILD PROJECT

This package prepares the existing DASSY v3.1 web app for an Android APK build using GitHub Actions (cloud build). You do not need Android Studio on your phone.

IMPORTANT DATA NOTE
The APK will have its own app storage. Customer/measurement/order data stored in Chrome on the website will not automatically appear in the APK. Before switching, open the current website and use its Settings backup/export feature. Keep that backup safely. After installing the APK, use the app's import/restore feature if available. Test with a small sample first and do not uninstall or clear the old website until your data is confirmed safe.

PHONE-ONLY BUILD OVERVIEW
1. Sign in or create a free GitHub account at https://github.com/.
2. In GitHub, create a new repository named dassy-tailoring-book. Choose Private if you prefer; GitHub Actions should be enabled.
3. Extract this ZIP on your phone using Files / ZArchiver.
4. Upload the extracted project contents to the repository's main branch. Include the hidden .github/workflows/build-apk.yml file. If your file manager hides dot-folders, turn on show hidden files.
5. Open the repository's Actions tab. Select “Build DASSY Android APK” and tap “Run workflow” (or wait for the first push build).
6. When the workflow finishes successfully, open that run, scroll to Artifacts, and download “DASSY-Tailoring-Book-APK”. Extract the downloaded artifact ZIP; inside is app-debug.apk.
7. Tap app-debug.apk to install. Android may ask you to allow installs from that browser or file manager. Only allow it for this trusted download, then turn the permission off again afterwards.

BUILD NOTES
- Package/application ID: com.dassy.tailoringbook
- App version: 3.1.0
- This workflow creates a debug APK for direct testing and sharing. It is not a signed Play Store release bundle (AAB).
- Keep the GitHub repository private if you do not want the source publicly visible. Anyone who can access a debug APK can install it; share it only with people you trust.
- This project does not add Google sign-in or cloud sync.

Odia Mart - Ready project (Android)

This ZIP contains the Flutter app source configured for "Odia Mart" (local fake data, no login).

IMPORTANT:
- This archive contains the Flutter source (lib/), pubspec.yaml, and assets/.
- Some CI systems (like CodeMagic) expect platform folders (android/) present. 
  If your CI fails due to missing platform files, add this pre-build script step on CodeMagic:

    flutter pub get
    flutter create .

- CodeMagic build steps (Android debug):
  1. Upload this repository/ZIP to CodeMagic.
  2. In project settings -> Pre-build script, add:
       flutter pub get
       flutter create .
  3. Start a build for Android (Debug).
  4. After build completes, download the generated APK.

If you prefer, you can also run locally on a PC:
  flutter pub get
  flutter create .
  flutter build apk --debug

App details:
- App display name: Odia Mart
- Package name suggestion: com.example.odiamart (you can change in Android manifest after flutter create)
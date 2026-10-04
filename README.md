# Obscura (native rebuild)

Private offline vault: PIN (4-6 digits) + pattern + fingerprint unlock, own in-app gallery picker and viewer,
colour-coded sections, locked originals removed from the gallery, no internet permission.

## Get the APK (GitHub, no Android Studio)
1. Create a free repo on github.com (private is fine).
2. Upload ALL files of this folder, keeping the folder structure and the hidden `.github` folder
   (easiest from a computer: unzip, then drag the contents into "Add file > Upload files").
3. Open the repo > Actions tab > "Build Obscura APK" (it starts by itself after the upload; or press "Run workflow").
4. When it turns green (about 5 minutes), open the run and download the `Obscura-APK` artifact (a zip containing `app-release.apk`).
5. Unzip, copy the APK to your phone and install (allow "install unknown apps" when asked).

If the run turns red, open it and send me the red error lines; I'll fix the code.

## Notes
- Package id is `com.afaq.obscura`, so it installs next to the old app. Take your files out of the old app first.
- Files are stored in the app's private storage (sandboxed). They are not yet encrypted at rest.

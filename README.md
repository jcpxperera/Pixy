# Pixy

Simple image resizing. Resize. Save. Done.
Bulk resize JPG, PNG and WebP images at once, entirely on your device.

## Get the APK with GitHub

1. Create a new GitHub repository and push this folder to the `main` branch.
2. Open the **Actions** tab. The *Build Pixy APK* workflow runs automatically (or press **Run workflow**).
3. When it finishes (about 5 minutes), open the run and download **Pixy-apk** from *Artifacts*. Unzip it to get `Pixy.apk`.
4. Copy `Pixy.apk` to your phone and install it (allow "Install unknown apps" if asked).


## Develop locally

    npm install
    npx cap add android
    npx cap sync android
    npx cap open android

The whole app is `www/index.html`. Open it in a browser to test without Android.

## Notes
- The build is a debug-signed APK, fine for installing directly. For Play Store, add a release keystore.
- **Resize & download** saves to Documents/Pixy; if Android blocks that, it opens the share sheet so you can save to Files or Photos.

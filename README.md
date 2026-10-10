# Tape Deck: offline music player (Android)

Cassette, CD and vinyl themes. Your songs are stored on the phone and play with no internet.

## Get the APK (no Android Studio needed)
1. Create a free account at github.com and make a new repository.
2. Upload everything in this folder (drag the files onto the repo page, keep the `.github` folder).
3. Open the repo's Actions tab. The "Build APK" workflow runs by itself (about 5 minutes).
4. Open the finished run, download the `tape-deck-apk` artifact, unzip it, and you have `app-debug.apk`.
5. Copy it to your phone and open it. Allow "Install unknown apps" if Android asks.

## Build it yourself instead
Needs Node 20, Java 17 and the Android SDK:

    npm install
    npx cap add android
    npx cap sync android
    cd android && ./gradlew assembleDebug

The APK lands in `android/app/build/outputs/apk/debug/app-debug.apk`.

## Using the app
- Tap + to pick songs. Cover art, title and artist are read from the files (mp3, m4a, flac).
- Hold the rewind / fast-forward keys to scan.
- Tabs at the top switch between cassette, CD and vinyl.
- The APK is signed with a debug key. That is fine for installing on your own phone.

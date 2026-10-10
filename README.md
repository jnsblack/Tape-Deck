# Tape Deck

An offline music player for Android that looks and feels like a retro tape deck. Pick a cassette, a CD player or a vinyl turntable, and play the music already on your phone or tablet. No account and no internet needed.

## Features

- **Three looks:** cassette, CD player and vinyl turntable, with spinning reels, disc and record, a moving tonearm, and VU meters.
- **Song-change animation:** the cassette ejects, the CD tray slides out, and the record lifts off before the next song loads.
- **Album art:** shown on the cassette label, the CD face and the vinyl centre label.
- **Music library:** scans your device for songs automatically. Search, sort by title, artist or newest, and add extra files by hand with the + button.
- **Scrolling titles:** long song names scroll across the screen instead of being cut off.
- **Retro sound:** gentle tape hiss and wobble on cassette, record crackle on vinyl, clean sound on CD.
- **Controls:** previous, next, hold-to-scan rewind and fast-forward, seek bar, shuffle, repeat and volume.
- **Phones and tablets:** a two-column layout on wide screens.

## Supported audio

MP3, FLAC, WAV, AAC/M4A, OGG and Opus play directly. ALAC and AIFF are converted while the song loads, which takes a few seconds for a long track. WMA and APE are not supported.

## Install

1. Open the **Releases** page and download `app-debug.apk` from the latest release.
2. Tap the file. If Android asks, allow installs from this source.
3. If Play Protect shows a warning, tap **More details**, then **Install anyway**.
4. On first launch, allow access to music and audio so your songs can be found.

Uninstall any older version first. Each build is signed with a new test key, so Android will not update over it.

## Privacy

The app only reads the music on your device to build the library. Nothing is uploaded and no internet connection is used.

## Known limits

- Playback may stop when the screen turns off.
- This is a test build signed with a debug key.

## Build it yourself

Pushing to this repository runs the **Build APK** workflow in GitHub Actions. It builds the app, adds the small native plugin that reads your music library, and publishes the APK as a release.

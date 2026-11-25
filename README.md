# Recorder Vault

A call recording app for Android using built-in wireless ADB pairing or Shizuku.

## Features

- **Phone call recording:** Record both sides of carrier calls automatically or prompt after each call (Opus `.ogg` or AAC `.m4a`).
- **App call recording (opt-in, Android 14+):** Record supported VoIP app calls with per-app selection.
- **In-call controls:** Pause, resume, stop, or add timestamp marks while recording.
- **Playback and library:** Waveform player, per-call notes, tags, stars, search, and lossless call merging.
- **Optional privacy and backup:** Optional biometric/PIN app lock and optional Google Drive folder backup via Android's document picker.
- **Flexible setup:** Use built-in wireless ADB pairing or Shizuku, with optional notification permission (the app still works if notifications are denied).

## Requirements

- **Android 11+** (`minSdk` 30)
- **64-bit ARM (`arm64-v8a`)** device
- **Wireless debugging** enabled in Developer options for built-in ADB pairing (or an active Shizuku setup)

## Install

1. Download the APK from this repository's **Releases** page.
2. Allow installing apps from unknown sources when prompted.
3. Open **Recorder Vault** and follow the setup wizard.

**Permissions:**
- **Optional:** Notifications
- **Required:** Contacts, Phone State, Call Log, and Battery Optimization exemption

## Known limitations

- On-device transcription and summaries are not included in this build (the native Whisper and Llama engines are excluded).

## Build the APK

1. Open **GitHub Actions** in this repository.
2. Select the **Build APK** workflow and click **Run workflow**.
3. Enter a version and run the workflow; the APK appears in **Releases**.

## Legal & disclaimer

**Recording phone calls may be subject to complex and varying laws in different countries and jurisdictions.** You may need consent from all parties before recording. The developers and contributors are **not responsible** for any misuse or legal consequences. Learn more: [Telephone call recording laws](https://en.wikipedia.org/wiki/Telephone_call_recording_laws). **This is not legal advice** — consult a legal professional for your situation. It is **your responsibility** to verify that Recorder Vault's behavior on your device complies with your local laws, and to stop immediately any activity that would constitute a legal infraction.

## Credits & attribution

Recorder Vault is a modified fork of CallVault, which is a modified fork of [ShizuCallRecorder](https://github.com/kitsumed/ShizuCallRecorder) by [kitsumed (Med)](https://github.com/kitsumed); the original project's name, trademarks, and logos are the property of their owner and are used here only for this required attribution. The ADB pairing/mDNS code is adapted from [RikkaApps/Shizuku](https://github.com/RikkaApps/Shizuku) (Apache-2.0). Both CallVault and ShizuCallRecorder are licensed under the GNU General Public License v3.0 with Additional Terms under Section 7.

Built on the work of:

- [scrcpy](https://github.com/Genymobile/scrcpy) — the fallback audio-capture server
- [libadb-android](https://github.com/MuntashirAkon/libadb-android) — the embedded ADB client

## License

Licensed under the [GNU General Public License v3.0](LICENSE) with Additional Terms under Section 7, see the [LICENSE](LICENSE) file.

> Recorder Vault is **not affiliated with, endorsed by, or supported by** kitsumed/ShizuCallRecorder, Shizuku, scrcpy, or Google/Android. "Android" is a trademark of Google LLC.

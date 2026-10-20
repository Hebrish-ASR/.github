<p align="center"><img src="https://raw.githubusercontent.com/Hebrish-ASR/.github/main/profile/banner.png" alt="Hebrish עבריש: dictation that gets the Hebrew words right" width="100%"></p>

<p align="center">
<a href="https://hebrish.app"><img src="https://img.shields.io/badge/Website-hebrish.app-0f6b5c?style=for-the-badge" alt="Website: hebrish.app"></a>
<a href="https://hebrish.app/download#fdroid"><img src="https://img.shields.io/badge/Android-F--Droid-0f6b5c?style=for-the-badge&logo=android&logoColor=white" alt="Android: F-Droid"></a>
<a href="https://hebrish.app/get/android"><img src="https://img.shields.io/badge/Android-APK-0f6b5c?style=for-the-badge&logo=android&logoColor=white" alt="Android: APK"></a>
<a href="https://hebrish.app/get/ubuntu"><img src="https://img.shields.io/badge/Linux-.deb-0f6b5c?style=for-the-badge&logo=ubuntu&logoColor=white" alt="Linux: .deb"></a>
<a href="https://hebrish.app/get/windows"><img src="https://img.shields.io/badge/Windows-.zip-0f6b5c?style=for-the-badge&logo=windows&logoColor=white" alt="Windows: .zip"></a>
</p>

**Dictation that gets the Hebrew words right.**

Hebrish is a non-profit umbrella for open speech tools that handle code-switched English–Hebrew: English speech with Hebrew words mixed in, as used by English-speaking immigrants in Israel and across the Jewish world.

## The model: Jachnun

**Jachnun** is the Hebrish speech recognition model, a fine-tune of NVIDIA Parakeet TDT 0.6B v2. Stock English models mangle the Hebrew words in an English sentence; Jachnun writes them in a consistent romanized spelling, and runs fully on the device, with no audio sent anywhere. The current release is **Jachnun v1.0**; later retrains will be v1.1, v1.2 and so on.

It is trained on one speaker's voice so far, so expect it to work best for voices like that one. Model card and benchmarks: [hebrish.app/model](https://hebrish.app/model). Weights: [huggingface.co/Hebrish/Jachnun](https://huggingface.co/Hebrish/Jachnun).

## Get the app

| Platform | Install |
| --- | --- |
| Android (recommended) | F-Droid: [add the Hebrish repository](https://fdroid.hebrish.app/repo?fingerprint=EF8C2D63D994A10CD489A978585510B47E47452EC09248591CB2C0F39C2BC1FA), then search for **Hebrish** |
| Android | Direct APK: [hebrish.app/get/android](https://hebrish.app/get/android) |
| Linux (Ubuntu) | `.deb`: [hebrish.app/get/ubuntu](https://hebrish.app/get/ubuntu) |
| Windows | `.zip`: [hebrish.app/get/windows](https://hebrish.app/get/windows) |

The download links always point at the latest release. All releases: [Hebrish-App releases](https://github.com/Hebrish-ASR/Hebrish-App/releases).

### F-Droid

1. Install [F-Droid](https://f-droid.org/) (or Droid-ify / Neo Store).
2. On your phone, open [this link](https://fdroid.hebrish.app/repo?fingerprint=EF8C2D63D994A10CD489A978585510B47E47452EC09248591CB2C0F39C2BC1FA) with F-Droid and confirm **Add repository**.
3. Search for **Hebrish** and install it. Updates then arrive like any other app's.

To add it by hand: **Settings → Repositories → +**, repository `https://fdroid.hebrish.app/repo`, fingerprint `EF8C2D63D994A10CD489A978585510B47E47452EC09248591CB2C0F39C2BC1FA`. Full instructions with a QR code: [hebrish.app/download](https://hebrish.app/download#fdroid).

## Repositories

| | |
| --- | --- |
| Website | [hebrish.app](https://hebrish.app) |
| Apps (Android, Linux, Windows) | [Hebrish-App](https://github.com/Hebrish-ASR/Hebrish-App) |
| Keyboard | [Hebrish-Keyboard](https://github.com/Hebrish-ASR/Hebrish-Keyboard): HeliBoard fork with Hebrish dictation in the mic key |
| F-Droid repository | [Hebrish-FDroid](https://github.com/Hebrish-ASR/Hebrish-FDroid) |
| Models and datasets | [huggingface.co/Hebrish](https://huggingface.co/Hebrish) · [full collection](https://huggingface.co/collections/Hebrish/hebrish-english-hebrew-code-switching-6ad6143c7de198780425709f) |
| Benchmark | [English-Hebrew-Codeswitching-ASR-Benchmark](https://github.com/Hebrish-ASR/English-Hebrew-Codeswitching-ASR-Benchmark) |
| Full index | [English-Hebrew-Code-Switching-Index](https://github.com/danielrosehill/English-Hebrew-Code-Switching-Index) |

Developed by [Daniel Rosehill](https://danielrosehill.com) · [contact](https://www.danielrosehill.com/contact/form).

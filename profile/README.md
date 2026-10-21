<p align="center"><img src="https://raw.githubusercontent.com/Hebrish-ASR/.github/main/profile/banner.png" alt="Hebrish עבריש: dictation that gets the Hebrew words right" width="100%"></p>

<p align="center">
<a href="https://hebrish.app"><img src="https://img.shields.io/badge/Website-hebrish.app-0f6b5c?style=for-the-badge" alt="Website: hebrish.app"></a>
<a href="https://hebrish.app/download#fdroid"><img src="https://img.shields.io/badge/Android-F--Droid-0f6b5c?style=for-the-badge&logo=android&logoColor=white" alt="Android: F-Droid"></a>
<a href="https://hebrish.app/get/android"><img src="https://img.shields.io/badge/Android-APK-0f6b5c?style=for-the-badge&logo=android&logoColor=white" alt="Android: APK"></a>
<a href="https://hebrish.app/get/ubuntu"><img src="https://img.shields.io/badge/Linux-.deb-0f6b5c?style=for-the-badge&logo=ubuntu&logoColor=white" alt="Linux: .deb"></a>
<a href="https://hebrish.app/get/windows"><img src="https://img.shields.io/badge/Windows-.zip-0f6b5c?style=for-the-badge&logo=windows&logoColor=white" alt="Windows: .zip"></a>
</p>

**Dictation that gets the Hebrew words right.**

Hebrish is a not-for-profit project building open speech tools for code-switched English–Hebrew: English speech with Hebrew words mixed in, as used by English-speaking immigrants in Israel and across the Jewish world. Stock English models mangle the Hebrew words in an English sentence. The Hebrish models write them in one consistent romanized spelling and run on the device, so no audio is sent anywhere.

## The models

The models are named after Israeli favourites. Every Sabich, Jachnun and Shakshuka model is at **v1.0**; later retrains will be v1.1, v1.2 and so on. See every model on one page in the **[Hebrish Models Space](https://huggingface.co/spaces/Hebrish/Hebrish-Models)**, or let [hebrish.app/models/choose](https://hebrish.app/models/choose) pick one for your device.

| Line | What it does | Variants |
| --- | --- | --- |
| **Sabich** (recommended) | Code-switching plus tech vocabulary, brand names and numbers. The default in the apps. | [Sabich](https://huggingface.co/Hebrish/Sabich) (Parakeet TDT 0.6B v2) · [-Qwen3-ASR-1.7B](https://huggingface.co/Hebrish/Sabich-Qwen3-ASR-1.7B) and [-Canary-Qwen-2.5B](https://huggingface.co/Hebrish/Sabich-Canary-Qwen-2.5B) for desktop GPUs · [-Parakeet-110M](https://huggingface.co/Hebrish/Sabich-Parakeet-110M) for small devices · [-asr4all-S](https://huggingface.co/Hebrish/Sabich-asr4all-S) and [-M](https://huggingface.co/Hebrish/Sabich-asr4all-M) for wearables |
| **Jachnun** | Code-switching only, without the tech vocabulary. In the apps next to Sabich. | [Jachnun](https://huggingface.co/Hebrish/Jachnun) (Parakeet TDT 0.6B v2) |
| **Shakshuka** | Streaming: the words appear while you are still talking. | [Shakshuka](https://huggingface.co/Hebrish/Shakshuka) (Nemotron Speech Streaming 0.6B) |
| Whisper Hebrish | Whisper fine-tunes, where the project started. | [Small ACFT](https://huggingface.co/Hebrish/Whisper-Hebrish-Small-ACFT) for FUTO Keyboard · [large-v3-turbo](https://huggingface.co/danielrosehill/Whisper-Hebrish) |
| Token classifier | Finds romanized Hebrew words in English text, for text-to-speech. | [Hebrew-Latin-Token-Classifier](https://huggingface.co/Hebrish/Hebrew-Latin-Token-Classifier) |

On-device builds (sherpa-onnx, ONNX, GGUF, MLX) are in their own `-<format>` repos under [huggingface.co/Hebrish](https://huggingface.co/Hebrish). The weights are gated: request access on the repository page, or write to [access@hebrish.app](mailto:access@hebrish.app). The apps download the models from Hebrish's own CDN and need no access request. Model cards and benchmarks: [hebrish.app/models](https://hebrish.app/models).

So far the models are trained on one speaker's voice. Want them to learn yours? [Contribute recordings](https://hebrish.app/support).

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
| Models overview | [Hebrish Models Space](https://huggingface.co/spaces/Hebrish/Hebrish-Models) |
| Models and datasets | [huggingface.co/Hebrish](https://huggingface.co/Hebrish) · [full collection](https://huggingface.co/collections/Hebrish/hebrish-english-hebrew-code-switching-6ad6143c7de198780425709f) |
| Benchmark | [English-Hebrew-Codeswitching-ASR-Benchmark](https://github.com/Hebrish-ASR/English-Hebrew-Codeswitching-ASR-Benchmark) |
| Full index | [English-Hebrew-Code-Switching-Index](https://github.com/danielrosehill/English-Hebrew-Code-Switching-Index) |

Developed by [Daniel Rosehill](https://danielrosehill.com) · [contact](https://www.danielrosehill.com/contact/form).

# Cortex for Mac — downloads

**Readiness for your mind.** Your watch knows if your body is ready; Cortex knows if your mind is, and protects it.
This repository only hosts the app downloads. Website: https://cortex-mind-rho.vercel.app

## Install

1. Download the latest `Cortex-<version>-arm64.dmg` from [Releases](../../releases/latest).
2. Open it and drag **Cortex** to **Applications**.
3. Open Cortex. This preview isn't notarized yet, so macOS may block it the first time: go to
   **System Settings → Privacy & Security** and choose **Open Anyway**.
4. First launch installs Python and the on-device libraries (about 1.5 GB), then the speech and voice
   models (about 2 GB). Once, into `~/Library/Application Support/Cortex`.
5. Optional: **Settings (⌘,)** → paste your own Anthropic API key to turn on the Claude coach and recall
   grading. It's encrypted with your macOS Keychain. Without a key, Cortex runs fully on-device.

**Requirements:** an Apple Silicon Mac (M1 or later).

## Privacy

Speech, voice and eye tracking run on your Mac. Camera frames, audio and screenshots are never stored;
only counts and short summaries are kept, in `~/.cortex`. With your own key, conversation text and today's
numbers go to Anthropic for the coach. The brain map is modeled from screen content and eye data; it is not
a brain measurement or a medical device.

## Notices

Includes [uv](https://github.com/astral-sh/uv) (MIT OR Apache-2.0), three.js (MIT), MediaPipe (Apache-2.0).
Brain surface derived from the MNI ICBM152 2009 template: Copyright (C) 1993–2004 Louis Collins, McConnell
Brain Imaging Centre, Montreal Neurological Institute, McGill University.

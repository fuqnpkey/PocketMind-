# PocketMind 🧠✨
*Your fully offline, privacy-focused AI assistant with voice control and local plugins*

[![License: GPLv3](https://img.shields.io/badge/License-GPLv3-blue.svg)](LICENSE)
[![Codemagic CI](https://api.codemagic.io/apps/YOUR_REAL_APP_ID/status_badge.svg)](https://codemagic.io/apps)

<p align="center">
  <img src="https://i.imgur.com/Jq6yxgQ.png" width="300" alt="PocketMind Logo">
</p>

---

## 📚 Table of Contents
- [Features](#-features)
- [Requirements](#-requirements)
- [Quick Start](#-quick-start)
- [Plugins](#-plugins)
- [Contribution](#-contribution)
- [Troubleshooting & FAQ](#-troubleshooting--faq)
- [License](#-license)
- [Credits](#-credits)

---

## 🌟 Features
- **100% Offline** – No cloud dependency, no data leaks
- **Voice Control** – Vosk-based STT/TTS (no internet required)
- **Local AI** – GPT4All integration for private conversations
- **Plugins** – Calculator, alarms, notes with expandable architecture
- **System Control** – Manage apps/settings via natural voice commands
- **Privacy First** – All data stays on-device (encrypted storage)

---

## 🛠 Requirements

### Development
- Java 17+
- Android Studio Flamingo (2022.2.1) or newer
- Android SDK 34 (Android 14)
- Gradle 8.0+

### Runtime
- Android 8.0+ (API 26)
- 2GB+ RAM recommended for AI models
- 500MB storage for base models

---

## 🚀 Quick Start

### For Users
1. Download the latest APK from [Releases](https://github.com/fuqnpkey/PocketMind-/releases)
2. Enable "Unknown Sources" in Android settings
3. Install and launch

### For Developers
```bash
# Clone repository
git clone https://github.com/fuqnpkey/PocketMind-.git
cd PocketMind-

# Build debug APK
./gradlew assembleDebug

# Install to connected device
adb install app/build/outputs/apk/debug/app-debug.apk

# (Optional) Download default AI model
mkdir -p app/src/main/assets/
wget https://gpt4all.io/models/ggml-gpt4all-j-v1.3-groovy.bin -P app/src/main/assets/
# Shuragram - Secure Messenger with Circumvention Features

<div align="center">

![Shuragram Logo](assets/icon.png)

**Secure. Private. Unblockable.**

[![Expo](https://img.shields.io/badge/Expo-51.0.0-black?style=flat-square&logo=expo)](https://expo.dev)
[![React Native](https://img.shields.io/badge/React_Native-0.74.0-blue?style=flat-square&logo=react)](https://reactnative.dev)
[![License](https://img.shields.io/badge/License-GPLv3-green?style=flat-square)](LICENSE)
[![Platform](https://img.shields.io/badge/Platform-Android%20%7C%20iOS-lightgrey?style=flat-square)]()

</div>

---

## 📖 About Shuragram

Shuragram is a secure messaging application designed to provide private communication even in regions with strict internet censorship. Built with React Native and Expo, it incorporates advanced circumvention techniques to bypass network restrictions while maintaining end-to-end encryption for user privacy.

### ✨ Key Features

- **🔒 End-to-End Encryption** - Optional E2EE for messages (toggle on/off per conversation)
- **🎥 Voice & Video Calls** - WebRTC-based calls with TURN server support
- **📸 Rich Media** - Send images, videos, and voice messages
- **🚀 Circumvention Technologies**:
  - Domain Fronting - Mask traffic as popular CDN requests
  - Packet Fragmentation - Bypass DPI by splitting large packets
  - Proxy Support - Built-in SOCKS5/HTTP proxy configuration
  - Traffic Obfuscation - Imitate regular HTTPS web traffic
- **🌙 Modern UI** - Dark theme by default, Telegram-inspired design
- **🔐 Local Storage** - Encrypted SQLite database on device

---

## 🛡️ Circumvention Features

Shuragram includes built-in tools to bypass network restrictions **without requiring external VPN services**:

| Feature | Description |
|---------|-------------|
| **Domain Fronting** | Requests go to popular CDNs (Cloudflare, Google) with modified Host headers |
| **Packet Fragmentation** | Splits large packets into MTU-sized fragments to avoid DPI detection |
| **Proxy Integration** | Native SOCKS5/HTTP proxy support with credentials |
| **Traffic Masking** | Wraps all traffic in HTTP/HTTPS-compatible formats |

> ⚠️ **Note**: Users are responsible for complying with local laws when using circumvention features.

---

## 📱 Screenshots

<div align="center">
  
| Chat Screen | Settings | Voice Call |
|-------------|----------|------------|
| *(Coming soon)* | *(Coming soon)* | *(Coming soon)* |

</div>

---

## 🚀 Installation

### Download APK (Android)

1. Go to [Releases](https://github.com/yourusername/shuragram/releases)
2. Download the latest `.apk` file
3. Enable "Install from unknown sources" on your device
4. Open the APK and install

### Build from Source

#### Prerequisites
- Node.js 18+ and npm
- Expo CLI
- Git

#### Steps

```bash
# Clone the repository
git clone https://github.com/yourusername/shuragram.git
cd shuragram

# Install dependencies
npm install

# Install Expo CLI
npm install -g expo-cli eas-cli

# Start development server
npm start

# Build APK (requires Expo account)
eas build -p android --profile production

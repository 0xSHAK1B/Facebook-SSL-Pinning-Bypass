# Facebook SSL Pinning Bypass for Android (2026) – Intercept & Capture HTTPS Traffic

[![Telegram](https://img.shields.io/badge/💬_Chat_on_Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white&labelColor=121212&color=26A5E4&logoWidth=20)](https://t.me/MUH4MM4DSH4KIB)
![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)
![ARM64](https://img.shields.io/badge/ARM64--v8a-Supported-blue?style=for-the-badge)
![x86_64](https://img.shields.io/badge/x86__64-Supported-blue?style=for-the-badge)

> Bypass Facebook SSL certificate pinning on Android by patching `libcoldstart.so` — intercept, inspect, and analyze HTTPS network traffic on both **rooted** and **non-rooted** devices.

---

## 📖 Overview

This project provides a **patched `libcoldstart.so`** library for the Facebook Android app with SSL/TLS certificate pinning disabled, enabling security researchers and developers to capture and analyze Facebook HTTPS traffic using standard MITM proxy tools.


---

## 🎥 Proof of Concept

<img width="720" height="1640" alt="Image" src="https://github.com/user-attachments/assets/698cb8c5-3b0e-43d6-8a8c-555ed66640ad" />
https://github.com/user-attachments/assets/f445a346-3a36-4ad6-b860-1e3930144a39

▶️ [**Watch the Full Video Demonstration**](https://github.com/user-attachments/assets/f445a346-3a36-4ad6-b860-1e3930144a39)

---

## 📋 Supported Facebook Version

| App | Version | Patched Library | Status |
|-----|---------|-----------------|--------|
| Facebook | **549.0.0.61.62** | `libcoldstart.so` | ✅ Bypassed |

> For the **latest patched `libcoldstart.so`**, [contact me on Telegram](https://t.me/MUH4MM4DSH4KIB).

---

## ⚙️ Supported Architectures

| Architecture | Support |
|---|---|
| `arm64-v8a` | ✅ |
| `x86_64` | ✅ |

---

## 📱 Requirements

### Option A: Physical Android Device

- Android phone or tablet (**rooted or non-rooted**)
- A traffic interception proxy tool:
  - [Proxypin](https://proxypin.com) — free, lightweight
  - [Reqable](https://reqable.com) — feature-rich, modern UI

### Option B: Android Emulator (PC)

- Windows PC with one of the following emulators installed:
  - [Nox Player](https://www.bignox.com/) — root access enabled
  - [LDPlayer](https://www.ldplayer.net/) — root access enabled
- A desktop MITM proxy tool:
  - [Burp Suite](https://portswigger.net/burp) — industry standard
  - [Mitmproxy](https://mitmproxy.org/) — open source
  - [Reqable](https://reqable.com)
  - [Proxypin](https://proxypin.com)

> **Note:** Root access must be enabled in the emulator to replace the native library.

---

## 🚀 Bypass Procedure

### Step 1 — Push the Patched Library

Replace the original `libcoldstart.so` with the patched version using ADB:

```bash
adb push D:\patched\libcoldstart.so /data/data/com.facebook.katana/lib-compressed/libcoldstart.so
```

### Step 2 — Set Correct Permissions (if needed)

```bash
adb shell chmod 755 /data/data/com.facebook.katana/lib-compressed/libcoldstart.so
```

### Step 3 — Configure Your Proxy

Set up your preferred MITM proxy tool (Proxypin, Reqable, Burp Suite, or Mitmproxy) and install/trust its CA certificate on the device or emulator.

### Step 4 — Launch & Capture

Open the Facebook app and start intercepting HTTPS requests and responses in your proxy tool.

> **Tip:** Force-stop Facebook before launching it after the library replacement to ensure the patched library is loaded.

---


**Target path:**
```
/data/data/com.facebook.katana/lib-compressed/libcoldstart.so
```

---


## 📬 Contact & Latest Builds

For the **most up-to-date** patched `libcoldstart.so` for Facebook, reach out directly:

[![Telegram](https://img.shields.io/badge/💬_Chat_on_Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white&labelColor=121212&color=26A5E4&logoWidth=20)](https://t.me/MUH4MM4DSH4KIB)

---

## 🏷️ Tags

`facebook ssl pinning bypass` · `facebook certificate pinning` · `facebook mitm` · `facebook traffic interception` · `facebook burp suite` · `facebook proxy android` · `facebook https decrypt` · `meta facebook security` · `android ssl bypass no root` · `libcoldstart.so patch` · `facebook api reverse engineering` · `facebook ssl bypass 2025`

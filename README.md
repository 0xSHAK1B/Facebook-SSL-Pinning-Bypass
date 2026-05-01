# Facebook SSL Pinning Bypass 2026 – Intercept HTTPS Traffic on Android (Root & No Root)

[![Telegram](https://img.shields.io/badge/💬_Chat_on_Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white&labelColor=121212&color=26A5E4&logoWidth=20)](https://t.me/MUH4MM4DSH4KIB)
![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)
![ARM64](https://img.shields.io/badge/ARM64--v8a-Supported-blue?style=for-the-badge)
![x86_64](https://img.shields.io/badge/x86__64-Supported-blue?style=for-the-badge)
![Last Updated](https://img.shields.io/badge/Updated-May_2026-brightgreen?style=for-the-badge)

> **Bypass Facebook's SSL/TLS certificate pinning on Android** to intercept, capture, and analyze HTTPS network traffic using proxy tools like Burp Suite, mitmproxy, Reqable, or Proxypin — works on both **rooted** and **non-rooted** devices. Working as of **2026**.


---

## Proof of Concept

<img width="720" height="1640" alt="Facebook SSL Pinning Bypass PoC – Intercepted HTTPS Traffic" src="https://github.com/user-attachments/assets/5b812211-5c1b-4d23-8407-0e9960ecc57e" />

▶️ [**Watch the Full Video Demonstration**](https://github.com/user-attachments/assets/47bd4817-d327-40bc-9fb4-84961d4d40de)

---

## Supported Facebook Version

| App | Version | Architecture | Status |
|-----|---------|--------------|--------|
| Facebook for Android | **558.0.0.70.72** | `arm64-v8a` | ✅ Bypassed — [contact on Telegram](https://t.me/MUH4MM4DSH4KIB) |
| Facebook for Android | **558.0.0.70.72** | `x86_64` | ✅ Bypassed — [contact on Telegram](https://t.me/MUH4MM4DSH4KIB) |
| Facebook for Android | **470.0.0.61.82** | `arm64-v8a` | ✅ Bypassed (Demo — [available in Releases](../../releases)) |

> **Want the latest version (558.0.0.70.72)?** For the **latest patched APK**, [contact me on Telegram](https://t.me/MUH4MM4DSH4KIB). The demo APK (v470.0.0.61.82) is available in [Releases](../../releases) to test the bypass.

---

## Requirements

### Option A: Physical Android Device (No Root Required)

- Android phone or tablet running **Android 7.0+**
- MITM proxy tool installed on the same device or on your local network:
  - [**Reqable**](https://reqable.com) — modern UI, excellent mobile support
  - [**Proxypin**](https://proxypin.com) — free, lightweight, no-root option

### Option B: Android Emulator on PC

- Windows, macOS, or Linux PC with an Android emulator:
  - [**Nox Player**](https://www.bignox.com/) — popular Android emulator with root toggle
  - [**LDPlayer**](https://www.ldplayer.net/) — fast Android emulator optimized for performance
- Desktop MITM proxy tool:
  - [**Burp Suite**](https://portswigger.net/burp) — industry-standard web security testing proxy
  - [**mitmproxy**](https://mitmproxy.org/) — open-source, scriptable HTTPS proxy
  - [**Reqable**](https://reqable.com) — cross-platform HTTP debugging proxy
  - [**Proxypin**](https://proxypin.com) — lightweight proxy with mobile support

---

## How to Bypass Facebook SSL Pinning (Step-by-Step)

### Step 1: Download the Patched APK

Download the **demo APK** (v470.0.0.61.82) from this repository's [Releases](../../releases) section to test the bypass. For the **latest patched APK** (v558.0.0.70.72), [contact me on Telegram](https://t.me/MUH4MM4DSH4KIB).

Choose the correct architecture for your device:
- **`arm64-v8a`** — Most modern Android phones and tablets
- **`x86_64`** — Android emulators (Nox Player, LDPlayer, etc.)

### Step 2: Install the Patched Facebook APK

- **Uninstall** the official Facebook app if already installed (signatures will conflict)
- **Enable** "Install from Unknown Sources" in your Android settings
- **Install** the downloaded patched APK

### Step 3: Configure Your MITM Proxy

1. Open your proxy tool (Burp Suite, mitmproxy, Reqable, or Proxypin)
2. **Export** the proxy's CA certificate
3. **Install and trust** the CA certificate on your Android device:
   - Go to **Settings → Security → Install certificates from storage**
   - On Android 11+, you may need to move the cert to the system trust store (root required) or use your proxy tool's built-in certificate installer
4. **Configure** your device's Wi-Fi proxy settings to point to the proxy

### Step 4: Capture Facebook HTTPS Traffic

1. Launch the patched **Facebook** app
2. Browse your feed, open Marketplace, send messages, or interact normally
3. Watch **decrypted HTTPS requests and responses** appear in your proxy tool in real time

> **Tip:** Make sure to install and trust the proxy's CA certificate on your device for full HTTPS decryption.

---


## Related Projects

- [**Instagram SSL Pinning Bypass**](https://github.com/0xSHAK1B) — Intercept Instagram HTTPS traffic on Android
- [**Threads SSL Pinning Bypass**](https://github.com/0xSHAK1B) — Capture Threads API requests and responses
- [**Messenger SSL Pinning Bypass**](https://github.com/0xSHAK1B) — Bypass Messenger certificate pinning
- [**TikTok SSL Pinning Bypass**](https://github.com/0xSHAK1B) — Bypass TikTok BoringSSL certificate pinning
- [**Snapchat SSL Pinning Bypass**](https://github.com/0xSHAK1B) — Decrypt Snapchat HTTPS traffic on Android

---

## Contact & Latest Builds

For the **most up-to-date** SSL pinning bypassed Facebook APK and support:

[![Telegram](https://img.shields.io/badge/💬_Chat_on_Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white&labelColor=121212&color=26A5E4&logoWidth=20)](https://t.me/MUH4MM4DSH4KIB)

---


## Tags

`facebook ssl pinning bypass` · `facebook ssl pinning bypass 2026` · `facebook certificate pinning bypass android` · `facebook mitm proxy` · `facebook https traffic interception` · `facebook burp suite android` · `facebook https decrypt` · `facebook proxy no root` · `meta facebook security research` · `facebook api reverse engineering` · `facebook ssl bypass no root` · `facebook frida bypass` · `facebook network traffic capture` · `facebook ssl unpinning` · `bypass ssl pinning facebook android` · `facebook apk ssl bypass` · `facebook mitmproxy` · `facebook reqable proxy` · `libcoldstart.so patch` · `meta fizz tls bypass` · `facebook penetration testing` · `android ssl pinning bypass 2026` · `intercept facebook traffic` · `facebook security audit` · `facebook certificate bypass arm64` · `facebook https interception android` · `facebook graphql api intercept` · `facebook marketplace api` · `facebook native binary patch`

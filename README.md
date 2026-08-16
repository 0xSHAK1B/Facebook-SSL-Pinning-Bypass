<div align="center">

# 🔓 Facebook Android SSL Pinning Bypass

**Intercept, capture & analyze Facebook HTTPS traffic on Android — no root required**

[![Download APK](https://img.shields.io/badge/⬇_Download_APK_(v574.0.0)-1877F2?style=for-the-badge&logo=facebook&logoColor=white)](../../releases/latest) &nbsp; [![Telegram](https://img.shields.io/badge/Telegram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/MUH4MM4DSH4KIB)

![Android](https://img.shields.io/badge/Android_10--14+-3DDC84?style=flat-square&logo=android&logoColor=white)
![ARM64](https://img.shields.io/badge/arm64--v8a-blue?style=flat-square)
![Version](https://img.shields.io/badge/Facebook-v574.0.0.40.71-1877F2?style=flat-square&logo=facebook&logoColor=white)
![Root](https://img.shields.io/badge/Root-Not_Required-brightgreen?style=flat-square)

<img width="578" height="1280" alt="Facebook Android SSL Pinning Bypass PoC – Traffic Captured" src="https://github.com/user-attachments/assets/eb0ae045-d88a-4872-b0db-d528e8f0dfda" />

*Live capture — Facebook Android HTTPS traffic intercepted in cleartext, v574.0.0.40.71.*

</div>

> **Bypass SSL/TLS certificate pinning** in Facebook for Android and pipe the full HTTPS stream — login, GraphQL, and Messenger flows — into **Burp Suite · mitmproxy · Reqable · Proxypin.** Tap a section below to expand.

---

<details open>
<summary><b>📦 Supported version</b></summary>

<br>

| App | Package | Version | ABI | Status |
|-----|---------|:-------:|:---:|:------:|
| Facebook for Android | `com.facebook.katana` | **574.0.0.40.71** | `arm64-v8a` | ✅ [**Download**](../../releases/latest) |

The patched APK lives in the [**Releases**](../../releases/latest) section. Need the newest build or another version? [Message me on Telegram](https://t.me/MUH4MM4DSH4KIB).

</details>

<details>
<summary><b>🎯 What you can capture</b></summary>

<br>

- **Login & authentication** — `b-graph.facebook.com` / `b-api.facebook.com` auth, access tokens, 2FA
- **GraphQL** — `/graphql` doc-id queries powering feed, profile, groups, and Marketplace
- **Messaging** — Messenger sync, MQTT realtime, thread and message endpoints
- **Feed & Reels** — ranking requests and story/reel media URLs
- **Media & CDN** — photo/video delivery and the upload pipeline
- **Ads, Pixel & telemetry** — ad payloads and analytics/tracking beacons

</details>

<details>
<summary><b>⚙️ Requirements</b></summary>

<br>

**Android device — Android 10, 11, 12, 13, 14+.** No root required (rooted devices supported too); ARM device (`arm64-v8a`), which covers virtually all modern phones and tablets.

**Emulator (PC):** Nox / LDPlayer / MEmu / BlueStacks — enable **ARM translation**, since this build ships `arm64` native libraries and x86/x86_64 emulators need the translation layer.

**Proxy tool** — [Burp Suite](https://portswigger.net/burp) · [mitmproxy](https://mitmproxy.org/) · [Reqable](https://reqable.com) · [Proxypin](https://proxypin.com)

</details>

<details>
<summary><b>🚀 How to bypass — step by step</b></summary>

<br>

1. Uninstall the official Facebook app (signatures conflict).
2. Download the patched APK from [**Releases**](../../releases/latest) and install it on your device or emulator.
3. Install and trust your proxy's CA certificate: **Settings → Security → Encryption & credentials → Install a certificate → CA certificate**.
4. Set the Wi-Fi proxy: **Settings → Wi-Fi → (network) → Proxy → Manual** → your PC's IP and port.
5. Launch Facebook — decrypted HTTPS streams into your proxy in real time.

> Force-stop and relaunch the app if traffic doesn't appear immediately.

</details>

<details>
<summary><b>💼 Need a custom bypass?</b></summary>

<br>

Custom SSL pinning bypass · automated patching scripts · full reverse-engineering projects — for any Android or iOS app. [**Message me on Telegram →**](https://t.me/MUH4MM4DSH4KIB)

</details>

<details>
<summary><b>⚠️ Disclaimer</b></summary>

<br>

For **educational and security-research purposes only**. Not affiliated with, endorsed by, or connected to Meta, Facebook, or their subsidiaries. All trademarks belong to their respective owners. You are responsible for complying with your local laws and the app's Terms of Service, and should only analyze traffic on accounts and devices you own or are authorized to test. Provided "as is", without warranty of any kind.

</details>

<details>
<summary><b>🔗 Related projects</b></summary>

<br>

| App | Platform | Repository |
|-----|----------|------------|
| Facebook | iOS | [Facebook iOS SSL Pinning Bypass](https://github.com/0xSHAK1B/Facebook-iOS-SSL-Pinning-Bypass) |
| Instagram | Android | [Instagram SSL Pinning Bypass](https://github.com/0xSHAK1B/Instagram-SSL-Pinning-Bypass) |
| Threads | Android | [Threads SSL Pinning Bypass](https://github.com/0xSHAK1B/Threads-SSL-Pinning-Bypass) |
| Meta Business Suite | Android | [Meta Business Suite SSL Pinning Bypass](https://github.com/0xSHAK1B/Meta-Business-Suite-SSL-Pinning-Bypass) |
| Messenger | Android | [Messenger SSL Pinning Bypass](https://github.com/0xSHAK1B/Messenger-SSL-Pinning-Bypass) |
| TikTok | Android | [TikTok SSL Pinning Bypass](https://github.com/0xSHAK1B/TIKTOK-SSL-Pinning-Bypass) |

</details>

---

<div align="center">

### 💖 Support This Project

Please **⭐ star the repo** — it helps others find it and keeps the builds coming.

| Currency | Address |
|:---------|:--------|
| **BTC / ETH** | `0xea9a566a5123c3a1b8d60f8bdd845835716668f0` |
| **USDT (TRC-20)** | `THssAZhUQEEsw15211rAaRLGRjSWXMX4PW` |

[![Telegram](https://img.shields.io/badge/@MUH4MM4DSH4KIB-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/MUH4MM4DSH4KIB)

</div>

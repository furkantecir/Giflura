# Privacy Policy for Giflura Browser Extension

**Last Updated:** November 5, 2026  
**Developer:** Furkan Tecir  
**Contact:** [furkantecir.com.tr](https://furkantecir.com.tr) | [GitHub Profile](https://github.com/furkantecir)  
**Extension:** Giflura (Chrome Web Store Extension ID: `phkmdcjiafaacblfhdkfemobdbmpefid`)

---

## 1. Overview and Core Philosophy

Giflura is a client-side media studio browser extension designed to convert videos from supported platforms (such as X / Twitter) and local files into animated GIFs and animated WhatsApp stickers (`.webp`).

**Privacy is our fundamental design principle.** Giflura operates entirely on the client side (inside your browser). We do not collect, transmit, sell, or monetize any personal information, browsing history, or media content.

---

## 2. Information Collection and Use

### No Personal Data Collected
- **Zero Personal Data:** Giflura does not collect names, email addresses, IP addresses, location data, or device identifiers.
- **Zero Telemetry & Analytics:** We do not include any tracking software, telemetry SDKs, Google Analytics, cookies, or remote scripts.
- **Zero Remote Media Upload:** All video processing, frame extraction, palette generation, and WebP/GIF encoding happen strictly inside your browser's memory using WebAssembly (FFmpeg WASM). Your videos and stickers never leave your machine and are never uploaded to any cloud server.

---

## 3. Browser Permissions and Why They Are Needed

In accordance with Chrome Web Store Developer Program Policies, here is an explicit breakdown of all permissions requested by Giflura and their single, legitimate purpose:

| Permission | Purpose |
| :--- | :--- |
| `host_permissions` (`https://twitter.com/*`, `https://x.com/*`, `https://*.twimg.com/*`, `https://web.whatsapp.com/*`) | Required exclusively to display the "GIF / Sticker" capture button above video players on X/Twitter and to enable sending the user's generated stickers directly to WhatsApp Web upon the user's explicit action. No page content or chat history is ever read, stored, or transmitted. |
| `webRequest` | Used locally to capture video stream headers (such as fragmented HLS / MP4 manifests) from video players on X/Twitter so they can be decoded locally by the FFmpeg WebAssembly engine. No network traffic is logged or sent anywhere. |
| `tabs` | Used solely to identify the active tab when launching the studio editor and to communicate between the background service worker and the studio interface. |
| `downloads` | Required to save the generated `.gif`, `.webp` sticker, `.wastickers` pack, or `.zip` archive directly to your computer's local "Downloads" folder when you click the download button. |
| `clipboardWrite` | Used exclusively when you explicitly click "Copy Sticker" in the studio, allowing you to paste (`Ctrl+V`) the sticker directly into messaging applications. |
| `storage` | Uses `chrome.storage.local` strictly on your device to remember your UI preferences (such as selected language, default framing mode, and timeline settings). Data remains on your device. |
| `scripting` | Required in Manifest V3 to inject the video capture buttons and the studio dialog into the web page. |

---

## 4. Third-Party Sharing and Remote Code

- **No Third Parties:** We do not share, sell, rent, or trade any user data with any third-party services, advertisers, or data brokers.
- **No Remote Code:** Giflura contains 100% locally bundled code. No scripts, styles, or WebAssembly binaries are loaded from remote servers or CDNs, ensuring full compliance with Chrome Web Store security standards.

---

## 5. Data Retention and Deletion

Because Giflura does not collect or transmit any data to external servers, there is no server-side data retention. Any local preferences stored in `chrome.storage.local` are automatically removed when you uninstall the extension from your browser.

---

## 6. Children's Privacy

Giflura does not collect any personal information from any user, including children under the age of 13.

---

## 7. Changes to This Privacy Policy

If we update this Privacy Policy in the future, the revised policy will be posted at this public URL with an updated "Last Updated" date.

---

## 8. Contact Information

If you have questions, feedback, or concerns regarding this Privacy Policy or Giflura, please contact the developer:

- **Developer:** Furkan Tecir
- **Website:** [https://furkantecir.com.tr](https://furkantecir.com.tr)
- **GitHub:** [https://github.com/furkantecir](https://github.com/furkantecir)
- **Repository:** [https://github.com/furkantecir/Giflura](https://github.com/furkantecir/Giflura)

---

# Gizlilik Politikası (Türkçe)

**Son Güncelleme:** 5 Kasım 2026  
**Geliştirici:** Furkan Tecir  
**İletişim:** [furkantecir.com.tr](https://furkantecir.com.tr) | [GitHub Profili](https://github.com/furkantecir)  
**Uzantı:** Giflura (Chrome Web Mağazası Kimliği: `phkmdcjiafaacblfhdkfemobdbmpefid`)

### 1. Genel Bakış ve Gizlilik İlkesi
Giflura, X (Twitter) üzerindeki videoları ve yerel medya dosyalarını GIF ve hareketli WhatsApp çıkartmalarına (`.webp`) dönüştüren istemci taraflı bir tarayıcı eklentisidir.

Giflura **tamamen çevrimdışı ve tarayıcınızın içinde** çalışır. Hiçbir kişisel veri, gezinme geçmişi veya medya içeriği toplanmaz, kaydedilmez, harici sunuculara iletilmez veya üçüncü taraflarla paylaşılmaz.

### 2. İzinlerin Kullanım Amacı
- **Ana Makine İzinleri (X/Twitter, WhatsApp Web):** Yalnızca video oynatıcıların üzerine "GIF / Sticker" düğmesi eklemek ve kullanıcının isteğiyle çıkartmayı WhatsApp Web'e aktarmak için kullanılır.
- **webRequest:** Video akış adreslerini (HLS/MP4) yerel WebAssembly motoruna aktarmak için kullanılır. Trafik izlenmez veya kaydedilmez.
- **tabs & scripting:** Stüdyo penceresini açmak ve aktif sekmeyle iletişim kurmak için kullanılır.
- **downloads:** Oluşturulan GIF veya çıkartmaları bilgisayarınıza kaydetmek için kullanılır.
- **clipboardWrite:** "Panoya Kopyala" butonuna basıldığında çıkartmayı panoya almak için kullanılır.
- **storage:** Dil ve arayüz tercihlerinizi tarayıcınızda yerel olarak saklamak için kullanılır.

### 3. İletişim
Gizlilik politikasıyla ilgili tüm sorularınız için geliştirici Furkan Tecir ile [furkantecir.com.tr](https://furkantecir.com.tr) veya [GitHub](https://github.com/furkantecir) üzerinden iletişime geçebilirsiniz.

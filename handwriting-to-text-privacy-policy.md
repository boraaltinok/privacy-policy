# Privacy Policy — Handwriting to Text: Scan

**Effective date:** July 16, 2026
**Last updated:** July 16, 2026

This Privacy Policy explains how **NEXTLINE YAZILIM LİMİTED ŞİRKETİ** ("NEXTLINE", "we", "us", or "our") handles information in connection with the mobile application **Handwriting to Text: Scan** (the "App").

We built this App to do one thing: turn a photo of handwriting into editable text. We have written this policy to describe honestly what actually happens to your data — including the fact that the images you choose to scan are sent to our processing backend and to a third‑party AI provider in order to transcribe them.

If you have any questions, contact us at **support@nextline.software**.

---

## 1. Summary (the short version)

- The App does **not** require you to create an account. There is no name, email, or password sign‑up. We use an **anonymous** identifier only.
- When you scan a page, the **image is transmitted off your device** to our backend and to a third‑party AI vision provider (OpenRouter) so it can be transcribed into text. This is the core function of the App and cannot be done fully on‑device.
- We do **not** permanently store your scanned images on our servers. Images are transmitted, processed, and discarded. Only the **resulting text** is briefly cached (about one hour) to make premium unlock and retries work.
- Saved conversions in your **Library are stored locally on your device** (premium items only). Free previews are never saved anywhere.
- We use **Firebase**, **OpenRouter**, **RevenueCat**, and **Amplitude** as service providers. Details below.

---

## 2. Information We Process

### 2.1 Content you provide (handwriting images)

When you capture a photo with the camera or import one from your photo library, the image is:

1. Compressed on your device;
2. Sent to our secure backend (a **Firebase Cloud Function**);
3. Forwarded to a **third‑party AI vision model via OpenRouter** for transcription;
4. Returned to your device as text.

**Image retention:** We do not save your scanned images to a database or file store. The image data exists only transiently for the duration of processing and is not persisted on our backend. The AI provider processes the image to generate the transcription; we do not control and cannot guarantee that provider's internal, transient handling of request data, but we do not authorize them to retain or train on your images. (See Section 4.)

### 2.2 Transcribed text

The text produced from your handwriting is:

- Returned to your device;
- **Cached on our backend for approximately one hour** (a short time‑to‑live) so that, for example, a premium purchase can unlock the full text without re‑running the scan, and so retries work. After the cache window the text is deleted automatically;
- Saved **locally on your device** in the App's Library **only if you are a premium user** (free previews are never persisted anywhere).

### 2.3 Anonymous identifier

To operate fair‑use limits and connect your device to our backend, we use **Firebase Anonymous Authentication**. This creates a random anonymous user ID for your app installation. It is **not** tied to your name, email address, phone number, or any real‑world identity, and we do not ask you for those.

### 2.4 Usage and fair‑use data

To enforce free/premium limits, we store minimal counters associated with your anonymous ID on our backend (Firebase), such as: number of free scans used, number of conversions, and the date of your last conversion. This does not include the content of your handwriting or your transcriptions beyond the short cache described above.

### 2.5 Diagnostics and analytics

- **Crash diagnostics** (via Firebase Crashlytics): if the App crashes, we collect crash reports, which may include device model, operating system version, app version, and technical stack traces. This does not include your handwriting content.
- **Product analytics** (via Firebase Analytics and Amplitude): we may collect anonymized/aggregated app‑usage events (for example, which screens are opened or that a conversion occurred) and standard technical/device information to understand how the App is used and improve it. Analytics events do not include the content of your handwriting or transcriptions.

### 2.6 Purchase data

If you buy a subscription, the transaction is handled by the **App Store / Google Play** and by **RevenueCat** (our subscription‑management provider). We receive purchase status (for example, whether a subscription is active) associated with an anonymous purchaser ID. **We never receive or store your full payment card details** — those are handled by the app store.

### 2.7 Technical/network data

Like any app that connects to the internet, our servers and service providers may process standard technical data such as IP address, device type, and operating system version as part of delivering network requests and preventing abuse.

---

## 3. How We Use Information

We use the information above only to:

- Transcribe the handwriting images you choose to scan;
- Provide, maintain, and improve the App's features;
- Enforce free/premium usage limits and prevent abuse;
- Process and restore subscriptions;
- Diagnose crashes and fix bugs;
- Understand aggregate usage to improve the product.

We do **not** sell your personal information. We do not use your handwriting content for advertising.

---

## 4. Third‑Party Service Providers

The App relies on the following processors. Each has its own privacy practices:

| Provider | Purpose | What it processes |
|----------|---------|-------------------|
| **Google Firebase** (Google LLC) — Anonymous Authentication, Cloud Functions, Cloud Firestore, Crashlytics, Analytics | Anonymous identity, backend processing, short‑lived text cache, usage counters, crash reports, analytics | Anonymous ID, usage counters, transient image during processing, short‑lived transcribed text, crash/analytics data |
| **OpenRouter** (and the underlying AI vision model provider it routes to, e.g. Google Gemini) | AI transcription of handwriting images | The handwriting image is sent for transcription during processing |
| **RevenueCat** | Subscription and purchase management | Anonymous purchaser ID, subscription status |
| **Amplitude** | Product analytics | Anonymized app‑usage events, device/technical data |
| **Apple App Store / Google Play** | Payment processing and subscription billing | Payment and billing information (handled by the store, not by us) |

The most important disclosure: **your scanned handwriting images are transmitted to our Firebase backend and to OpenRouter's AI vision model for the sole purpose of transcribing them.** This is unavoidable for the App to work, because the transcription is performed by a cloud AI model, not on your device.

We recommend reviewing the privacy policies of Google/Firebase, OpenRouter, RevenueCat, Amplitude, and your app store.

---

## 5. Data Stored on Your Device

The following stays on your device and is not sent to us (except as part of a scan you initiate):

- **Your Library of saved conversions** (premium only) — stored in a local on‑device database;
- **App preferences** (for example, output language, onboarding completion);
- **Local usage counters** used for display.

Deleting the App removes this local data from your device.

---

## 6. Notifications

The App may schedule **local notifications** on your device (for example, reminders). These are generated on your device by the operating system. The App does **not** use remote push notifications and does not collect a push token for that purpose.

---

## 7. Data Retention

- **Scanned images:** not persisted on our backend; discarded after processing.
- **Transcribed text cache:** automatically deleted after approximately one hour (time‑to‑live).
- **Anonymous ID and usage counters:** retained while your installation remains active, to maintain fair‑use limits.
- **Crash/analytics data:** retained per our providers' standard retention settings.
- **Local Library and preferences:** retained on your device until you delete them or uninstall the App.

---

## 8. Children's Privacy

The App is not directed to children under 13 (or the minimum age required in your jurisdiction). We do not knowingly collect personal information from children. If you believe a child has provided information to us, contact **support@nextline.software** and we will address it.

---

## 9. Security

We use industry‑standard measures to protect data in transit (encryption over HTTPS/TLS) and rely on the security of established providers (Google Firebase, OpenRouter, RevenueCat, Amplitude). No method of transmission or storage is 100% secure, but we minimize what we collect and retain.

---

## 10. Your Rights

Depending on your location, you may have rights to access, correct, or delete personal data. Because we operate on an anonymous basis and do not collect your name or email, the primary way to remove locally stored data is to delete the App. For any request regarding backend data associated with your anonymous ID, contact **support@nextline.software**.

---

## 11. International Transfers

Our providers may process data on servers located outside your country. By using the App, you understand that your data (including images sent for transcription) may be processed in other jurisdictions.

---

## 12. Changes to This Policy

We may update this Privacy Policy from time to time. Material changes will be reflected by updating the "Last updated" date above. Continued use of the App after changes constitutes acceptance.

---

## 13. Contact

**NEXTLINE YAZILIM LİMİTED ŞİRKETİ**
Email: **support@nextline.software**

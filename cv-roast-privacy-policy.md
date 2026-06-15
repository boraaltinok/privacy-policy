# **Privacy Policy**

This Privacy Policy applies to the **Resume Analysis: CV Roast** mobile application (the "Application") created by **NEXTLINE YAZILIM LİMİTED ŞİRKETİ** ("Service Provider"). The Application is offered as a Commercial service and is intended for use **"AS IS"** as an entertainment-and-feedback tool for your own résumé/CV.

By using the Application, you consent to our collection, use, and disclosure of information as described in this policy. This Privacy Policy may be updated from time to time, and we encourage you to review it periodically. Your continued use of the Application constitutes acceptance of any modifications to this policy.

---

## **1. Information Collection and Use**

### **1.1 Anonymous Account**
The Application creates an **anonymous account** for you automatically through Firebase Authentication on first launch. You are **not** required to provide an email address, name, phone number, or any other personally identifying information to use the Application. The anonymous user identifier (UID) is used to:

- Enforce fair-use limits and per-user rate limits that protect the service from abuse
- Deduplicate repeated analysis requests (idempotency)
- Correlate anonymized product-analytics events to a single device install

There is no sign-up flow, no profile, and no login screen.

### **1.2 Automatically Collected Information**
When you use the Application, the following diagnostic and product information may be automatically collected:

- **Device information**: device model, operating system version, app version, language/locale, time zone
- **Crash diagnostics**: stack traces, device state at time of crash, non-fatal error reports
- **Product analytics events**: which screens you viewed, which features you tapped, scan latency, the target role and tone you selected, subscription state (premium / free), error codes, and timestamps

We use this information to monitor stability, debug issues, and improve the Application.

### **1.3 Your CV / Résumé Content (Processed Ephemerally)**
When you actively start a scan (for example, by tapping **"Roast My CV"** after selecting a file, photo, or pasting text), the input you supplied for that single analysis is sent to our backend in order to produce the roast and the fixes:

- **Document mode**: the PDF, DOC, or DOCX you selected
- **Photo mode**: the JPG, PNG, or HEIC image of a CV you selected (HEIC is converted to JPEG on your device before upload)
- **Paste mode**: the résumé text you pasted

**Important — your CV may contain your own personal information.** A résumé typically includes your name, contact details, employment history, and education. That content is transmitted **securely over HTTPS** to our backend, parsed **in memory** to extract its text, and forwarded to the AI provider (see Section 2) solely to generate your analysis. The raw CV (text or file bytes) is held **only for the duration of that single request** and is **never written to our servers, cloud storage, or any database.** The generated analysis is returned to your device only.

### **1.4 Local Device Data (Stored Only on Your Phone)**
The following is stored **locally on your device** using on-device storage (Hive) and is **not** uploaded to our servers or synced to any cloud:

- **Roast history**: your past analyses, including the detected weak-line excerpts, roasts, suggested fixes, scores, and archetypes
- **Preferences**: default tone, appearance/theme, and similar settings

Because this data lives only on your device, you can remove it at any time by deleting individual history items inside the Application or by uninstalling the Application.

### **1.5 Fair-Use Metadata**
Per anonymous user, we store the following non-content metadata server-side to operate the fair-use system:

- Number of analyses performed within a rolling time window
- Rate-limit and idempotency records (server-only)
- Account creation and last-update timestamps

We do **not** store the contents of your CV, the weak lines, or the generated roasts/fixes in this metadata.

### **1.6 Information We Do NOT Collect**
The Application does **not** collect, request, or transmit:

- Your name, email address, phone number, or postal address as a registration step (any such details exist only inside a CV you choose to scan, and are handled as described in Section 1.3)
- Your precise or approximate location
- Microphone audio or camera live feed (the Application reads CVs from your Files and Photo Library; it does not record audio or use the live camera)
- Contacts, calendar, or health data
- Advertising identifiers (IDFA / GAID) for cross-app advertising — the Application shows no ads and performs no cross-app tracking
- Push notification tokens — remote push notifications are not used in this version. The Application may schedule occasional **on-device local reminder notifications** (for example, a nudge to finish reviewing your CV); these are generated and scheduled entirely on your device and send no data to us. You can disable them in iOS Settings → Notifications.

---

## **2. AI Processing of Your CV**

The Application uses **OpenRouter** (https://openrouter.ai), a third-party AI routing service, to analyze your CV and generate the roast and fixes. OpenRouter forwards your input to one of several large-language-model providers (such as Anthropic, OpenAI, or Google) selected at the time of your request.

### **2.1 How It Works**
- AI processing only occurs when you **explicitly start a scan**.
- Your document text (or, for image CVs, the image) is transmitted **securely over HTTPS** to our Cloud Functions backend, which then forwards it to OpenRouter.
- OpenRouter and the underlying model provider process the input solely to generate the structured analysis returned to you.
- We do **not** store the input or the output on our servers.

### **2.2 Third-Party AI Retention**
OpenRouter and the underlying model providers may briefly retain submitted inputs and outputs for service delivery, abuse monitoring, and safety evaluation, in accordance with their own published policies. Retention windows are managed by those providers and not by us. For details, please review:

- OpenRouter Privacy: https://openrouter.ai/privacy
- OpenRouter Terms: https://openrouter.ai/terms

### **2.3 You Control What You Submit**
Because your CV is sent to a third-party AI service for analysis, you should submit only your own résumé and avoid including information you do not want processed by an AI model. If your CV contains highly sensitive personal data you would rather not transmit, you can remove those lines before scanning, or paste only the sections you want analyzed. You are responsible for the content you submit.

### **2.4 Privacy on Shared Cards (PII Redaction)**
When you create a shareable card from a result, the Application **automatically redacts personal information on your device before any image is produced** — including name, email, phone number, links, and similar identifiers. Anonymization applies to exported/shared cards; inside the Application (after purchase) you continue to see your real lines and fixes. The principle is simple: **your CV is never shared — only the roast is.**

---

## **3. Third-Party Services**

The Application integrates the following third-party services. Each has its own privacy policy governing how it handles data:

| Service | Purpose | Privacy Policy |
|---|---|---|
| **Firebase Authentication** (Google) | Anonymous user identifier | https://firebase.google.com/support/privacy |
| **Cloud Functions for Firebase** (Google) | Server-side CV parsing and analysis logic | https://firebase.google.com/support/privacy |
| **Cloud Firestore** (Google) | Server-only fair-use counters and idempotency records (no client access) | https://firebase.google.com/support/privacy |
| **Firebase Remote Config** (Google) | Feature configuration (e.g., paywall availability) | https://firebase.google.com/support/privacy |
| **Firebase Crashlytics** (Google) | Crash diagnostics | https://firebase.google.com/support/privacy |
| **Firebase Analytics** (Google) | Anonymized product analytics | https://firebase.google.com/support/privacy |
| **OpenRouter** | AI CV analysis / roast & fix generation routing | https://openrouter.ai/privacy |
| **Amplitude** | Anonymized product analytics | https://amplitude.com/privacy |
| **RevenueCat** | Subscription processing | https://www.revenuecat.com/privacy |
| **Apple App Store / In-App Purchase** | Payment processing for subscriptions | https://www.apple.com/legal/privacy/ |
| **Google Fonts** | Typography (Space Grotesk, Inter) downloaded from Google's font CDN | https://policies.google.com/privacy |

We may also disclose information:

- as required by law, such as to comply with a subpoena or similar legal process;
- when we believe in good faith that disclosure is necessary to protect our rights, your safety, or the safety of others, investigate fraud, or respond to a government request;
- to trusted service providers who work on our behalf, do not have an independent right to use the information we disclose to them, and have agreed to adhere to the rules set forth in this policy.

---

## **4. Subscriptions and Payments**

The Application offers optional auto-renewing subscriptions that unlock the full roast, every fix, and unlimited scans. Subscriptions are processed by **Apple via the App Store**, with subscription state mediated by **RevenueCat**.

We do **not** receive your full payment-card or App Store account credentials. We receive only the entitlement signal (whether your account currently has an active subscription) and a non-personal subscription identifier needed to verify your entitlement on this device.

For details on payment data handling, please review Apple's and RevenueCat's privacy policies linked in Section 3.

---

## **5. Analytics and Tracking**

We use **Amplitude** and **Firebase Analytics** to understand how users move through the Application (for example: how many people complete onboarding, how often a scan succeeds, which tone is most popular). Analytics events are tied to your anonymous user identifier and contain **only metadata** — for example: screen name, target role, tone, latency, error code, subscription state, and timestamps.

Analytics events **never include**:

- The text of your CV
- The contents of your documents or photos
- The detected weak lines, roasts, or generated fixes

**No cross-app tracking:** The Application does **not** track you across other companies' apps and websites, and therefore does **not** display Apple's App Tracking Transparency prompt. We do **not** sell your data, we do **not** use it for third-party advertising, and we do **not** share it with data brokers. The Application contains no advertising. Product analytics are tied only to your anonymous identifier and are used solely to improve the Application.

---

## **6. Children**

The Application is intended for users aged 13 and older. We do not knowingly collect personal information from children under 13 years of age. If you are a parent or guardian and become aware that your child under 13 has used the Application, please contact us at [support@nextline.software](mailto:support@nextline.software) and we will take appropriate steps.

---

## **7. Data Retention and Deletion**

- **Your CV content (documents, photos, pasted text) and generated output:** Not retained on our servers. Forwarded to the AI provider only for the duration of a single analysis request.
- **Roast history and preferences:** Stored only on your device. Delete history items in the Application, or uninstall the Application, to remove them.
- **Fair-use metadata and anonymous account record:** Retained for as long as needed to operate the fair-use system and for a reasonable time thereafter.
- **Crash diagnostics:** Retained per Firebase Crashlytics defaults.
- **Analytics events:** Retained per Amplitude and Firebase Analytics defaults.

If you would like us to delete the anonymous usage record associated with your device, please contact us at [support@nextline.software](mailto:support@nextline.software). Because the account is anonymous and not tied to an email, we may need additional information from you (such as your anonymous user ID, if exposed in the Application, or your device model and approximate first-launch date) to locate the record.

You can also stop all collection of information from this device immediately by **uninstalling the Application**.

---

## **8. Security**

We take reasonable physical, electronic, and procedural safeguards to protect the information we process. All transmissions to our backend and to third-party services occur over encrypted HTTPS / TLS connections. AI provider API credentials are held server-side only and are never embedded in the Application binary.

No method of transmission or storage is 100% secure, and we cannot guarantee absolute security.

---

## **9. International Data Transfers**

The third-party services listed in Section 3 operate globally. Your information may be processed in the United States or in other countries where these providers maintain infrastructure, including the country where the underlying AI model selected by OpenRouter for your request is hosted.

---

## **10. Changes to This Privacy Policy**

This Privacy Policy may be updated from time to time. We will notify you of any changes by posting the new Privacy Policy on this page and updating the "Last Updated" date. Continued use of the Application after changes are posted constitutes your acceptance of those changes.

---

## **11. Transfer or Assignment**

We may share or transfer information in connection with any merger, sale of company assets, financing, or acquisition of all or a portion of our business to another company. In such an event, the acquiring company's use of information will be governed by the terms of this Privacy Policy unless otherwise notified.

---

## **12. Your Consent**

By using the Application, you consent to the processing of information as described in this Privacy Policy, now and as amended by us.

---

## **13. Contact Us**

If you have any questions about this Privacy Policy or about our practices, please contact us:

- **Email**: [support@nextline.software](mailto:support@nextline.software)
- **Developer**: NEXTLINE YAZILIM LİMİTED ŞİRKETİ

**Last Updated**: 15/06/2026

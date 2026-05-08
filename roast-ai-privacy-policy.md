# **Privacy Policy**

This Privacy Policy applies to the **Roast AI: Roast Generator** mobile application (the "Application") created by **NEXTLINE YAZILIM LİMİTED ŞİRKETİ** ("Service Provider"). The Application is offered as a Commercial service and is intended for use **"AS IS"** for entertainment purposes only.

By using the Application, you consent to our collection, use, and disclosure of information as described in this policy. This Privacy Policy may be updated from time to time, and we encourage you to review it periodically. Your continued use of the Application constitutes acceptance of any modifications to this policy.

---

## **1. Information Collection and Use**

### **1.1 Anonymous Account**
The Application creates an **anonymous account** for you automatically through Firebase Authentication on first launch. You are **not** required to provide an email address, name, phone number, or any other personally identifying information. The anonymous user identifier (UID) is used to:

- Track usage counters (free roast generations consumed, total generations)
- Enforce per-user rate limits to protect the service from abuse
- Correlate anonymized product analytics events to a single device install

There is no sign-up flow, no profile, and no login screen.

### **1.2 Automatically Collected Information**
When you use the Application, the following diagnostic and product information may be automatically collected:

- **Device information**: device model, operating system version, app version, language/locale, time zone
- **Crash diagnostics**: stack traces, device state at time of crash, non-fatal error reports
- **Product analytics events**: which screens you viewed, which features you tapped, generation latency, intensity selected, language mode selected, subscription state (premium / free), and timestamps

We use this information to monitor stability, debug issues, and improve the Application.

### **1.3 User-Provided Content (Processed Ephemerally)**
When you actively tap **"Roast it"**, the input you supplied for that single generation is sent to our backend in order to produce a roast:

- **Screenshot mode**: the screenshot image you selected
- **Photo mode**: the photo you selected
- **Describe mode**: the short text description you typed (max 280 characters)

This input is **not** stored on our servers. It is forwarded to the AI provider (see Section 2), used to produce the roast, and discarded after the response is returned. The generated roast text is **not** retained on our servers either — it is delivered back to your device only.

### **1.4 Usage Counters**
Per anonymous user, we store the following non-content metadata in our database (Firebase Firestore):

- Number of free roast generations consumed (lifetime)
- Total number of generations (lifetime)
- Timestamp of the last generation
- Rate-limit window state (server-only)
- Account creation and last-update timestamps

We do **not** store the contents of your screenshots, photos, descriptions, or generated roasts.

### **1.5 Information We Do NOT Collect**
The Application does **not** collect, request, or transmit:

- Your name, email address, phone number, postal address, or other contact details
- Your precise or approximate location
- Microphone audio, camera live feed, contacts, calendar, or health data
- Advertising identifiers (IDFA / GAID) — no App Tracking Transparency prompt is shown because no cross-app tracking is performed
- Push notification tokens — push notifications are not used in this version

---

## **2. AI Processing of Your Input**

The Application uses **OpenRouter** (https://openrouter.ai), a third-party AI routing service, to generate roasts from the input you provide. OpenRouter forwards your input to one of several large-language-model providers (such as Anthropic, OpenAI, or Google) selected at the time of your request.

### **2.1 How It Works**
- AI processing only occurs when you **explicitly tap "Roast it"**.
- Your image (resized and compressed on your device, with EXIF metadata stripped) or your text description is transmitted **securely over HTTPS** to our Cloud Functions backend, which then forwards it to OpenRouter.
- OpenRouter and the underlying model provider process the input solely to generate the 3 roast outputs returned to you.
- We do **not** store the input or output on our servers.

### **2.2 Third-Party AI Retention**
OpenRouter and the underlying model providers may briefly retain submitted inputs and outputs for service delivery, abuse monitoring, and safety evaluation, in accordance with their own published policies. Retention windows are managed by those providers and not by us. For details, please review:

- OpenRouter Privacy: https://openrouter.ai/privacy
- OpenRouter Terms: https://openrouter.ai/terms

### **2.3 No Facial Recognition**
The Application does **not** perform facial recognition, identity matching, or biometric extraction. The AI model is asked to generate humorous text based on the overall vibe, content, or context of the input — not to identify any individual.

### **2.4 Don't Upload Real-Person Identifiers You Don't Want Processed**
Because your input is sent to a third-party AI service, you should **avoid uploading content that contains personal information you do not want processed by an AI model** (e.g., other people's private messages, identification documents, or private photos of others without their consent). You are responsible for the content you submit.

---

## **3. Third-Party Services**

The Application integrates the following third-party services. Each has its own privacy policy governing how it handles data:

| Service | Purpose | Privacy Policy |
|---|---|---|
| **Firebase Authentication** (Google) | Anonymous user identifier | https://firebase.google.com/support/privacy |
| **Cloud Firestore** (Google) | Backend database for usage counters and remote configuration | https://firebase.google.com/support/privacy |
| **Cloud Functions for Firebase** (Google) | Server-side roast generation logic | https://firebase.google.com/support/privacy |
| **Firebase Crashlytics** (Google) | Crash diagnostics | https://firebase.google.com/support/privacy |
| **OpenRouter** | AI roast generation routing | https://openrouter.ai/privacy |
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

The Application offers optional auto-renewing subscriptions that unlock unlimited roast generations. Subscriptions are processed by **Apple via the App Store**, with subscription state mediated by **RevenueCat**.

We do **not** receive your full payment-card or App Store account credentials. We receive only the entitlement signal (whether your account currently has an active subscription) and a non-personal subscription identifier needed to verify your entitlement on this device.

For details on payment data handling, please review Apple's and RevenueCat's privacy policies linked in Section 3.

---

## **5. Analytics**

We use **Amplitude** to understand how users move through the Application (for example: how many people complete onboarding, how often roast generation succeeds, which intensity is most popular). Amplitude events are tied to your anonymous user identifier and contain **only metadata** — for example: input mode, intensity, language, latency, error code, and timestamps.

Amplitude events **never include**:

- The text of your descriptions
- The contents of your screenshots or photos
- The text of generated roasts

---

## **6. Children**

The Application is intended for users aged 13 and older and contains content that is not appropriate for younger children. We do not knowingly collect personal information from children under 13 years of age. If you are a parent or guardian and become aware that your child under 13 has used the Application, please contact us at [support@nextline.software](mailto:support@nextline.software) and we will take appropriate steps.

---

## **7. Data Retention and Deletion**

- **User-provided content (screenshots, photos, descriptions, generated roasts):** Not retained on our servers. Forwarded to the AI provider only for the duration of a single generation request.
- **Usage counters and anonymous account record:** Retained for as long as the Application is installed on your device and for a reasonable time thereafter.
- **Crash diagnostics:** Retained per Firebase Crashlytics defaults.
- **Analytics events:** Retained per Amplitude defaults.

If you would like us to delete the anonymous usage record associated with your device, please contact us at [support@nextline.software](mailto:support@nextline.software). Because the account is anonymous and not tied to an email, we may need additional information from you (such as your anonymous user ID, which can be found in the Application's settings if exposed there, or a recent device identifier) to locate the record.

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

**Last Updated**: 08/05/2026

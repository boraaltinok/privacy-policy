# **Privacy Policy**

This Privacy Policy applies to the **Swipeworthy** mobile application (the "Application") created by **NEXTLINE YAZILIM LİMİTED ŞİRKETİ** ("Service Provider"). The Application is offered as a Commercial service and is intended for use **"AS IS"** for entertainment and self-improvement purposes only.

By using the Application, you consent to our collection, use, and disclosure of information as described in this policy. This Privacy Policy may be updated from time to time, and we encourage you to review it periodically. Your continued use of the Application constitutes acceptance of any modifications to this policy.

---

## **1. Information Collection and Use**

### **1.1 Anonymous Account**
The Application creates an **anonymous account** for you automatically through Firebase Authentication on first launch. You are **not** required to provide an email address, name, phone number, or any other personally identifying information. The anonymous user identifier (UID) is used to:

- Track usage counters (free roast generations consumed, total audits, daily generation count)
- Enforce the lifetime free cap and the daily fair-use ceiling that protect the service from abuse
- Correlate anonymized product analytics events to a single device install

There is no sign-up flow, no profile, and no login screen.

### **1.2 Automatically Collected Information**
When you use the Application, the following diagnostic and product information may be automatically collected:

- **Device information**: device model, operating system version, app version, language/locale, time zone
- **Crash diagnostics**: stack traces, device state at time of crash, non-fatal error reports
- **Product analytics events**: which screens you viewed, which features you tapped, generation success/failure and latency, subscription state (premium / free), and timestamps

We use this information to monitor stability, debug issues, and improve the Application.

### **1.3 User-Provided Content (Your Profile Screenshots)**
The core feature of the Application is an AI audit of your dating-profile screenshots. When you actively confirm your lineup and start a roast, the 2–10 screenshots you selected for that single generation are sent to our backend to produce the audit:

- Screenshots are selected through the standard iOS photo picker — the Application never scans or accesses your photo library in the background.
- Before upload, each image is **resized and compressed on your device** (metadata such as EXIF/location tags is stripped during compression).
- The images are transmitted **securely over HTTPS** to our Cloud Functions backend, which forwards them to the AI provider (see Section 2), uses the response to compute your score and roast, and returns the result to your device.
- Your screenshots are **never written to our servers or to any cloud storage**. They exist server-side only in memory for the duration of your single request.

The Application also asks for your **explicit consent** on a dedicated consent screen before your first roast is ever generated.

### **1.4 Generated Results (24-Hour Text-Only Cache)**
To make sure a network retry or an interrupted app session never consumes a second free generation for the same lineup, the **text of your generated audit result** (score, roast lines, fix-plan text — **never your images**) is kept in a server-side processing cache for **up to 24 hours**, after which it is automatically deleted by a database time-to-live policy. Your full roast history is otherwise stored **only on your device**.

### **1.5 Usage Counters**
Per anonymous user, we store the following non-content metadata in our database (Firebase Firestore):

- Number of free roast generations consumed (lifetime)
- Total number of audits generated (lifetime)
- Current-day generation count and date (fair-use window)
- Account creation and last-update timestamps

We do **not** store the contents of your screenshots or your roast history on our servers (beyond the 24-hour text-only cache described in Section 1.4).

### **1.6 Local Device Data**
The following data is stored **only on your device** and never uploaded:

- Your roast history (past audit results and their thumbnails)
- Your fix-plan checklist progress
- App preferences and flags (onboarding completed, consent given, notification choice)

Deleting the Application deletes all of this local data.

### **1.7 Information We Do NOT Collect**
The Application does **not** collect, request, or transmit:

- Your name, email address, phone number, postal address, or other contact details
- Your precise or approximate location
- Microphone audio, camera live feed, contacts, calendar, or health data
- Advertising identifiers (IDFA / GAID) — no App Tracking Transparency prompt is shown because no cross-app tracking is performed
- Push notification tokens — the Application does not use push notifications (see Section 6)

---

## **2. AI Processing of Your Screenshots**

The Application uses **OpenRouter** (https://openrouter.ai), a third-party AI routing service, to analyze your profile screenshots with vision-capable large language models (such as models from Google or OpenAI) selected at the time of your request. Your numeric score is computed **deterministically on our own servers** from the model's structured critique — the AI model does not invent your score.

### **2.1 How It Works**
- AI processing only occurs when you **explicitly start a roast** after confirming your lineup and after having accepted the one-time AI consent screen.
- Your compressed screenshots are transmitted securely over HTTPS to our Cloud Functions backend, which forwards them to OpenRouter.
- OpenRouter and the underlying model provider process the images solely to generate the critique returned for your audit.
- We do **not** store your images on our servers.

### **2.2 Third-Party AI Retention**
OpenRouter and the underlying model providers may briefly retain submitted inputs and outputs for service delivery, abuse monitoring, and safety evaluation, in accordance with their own published policies. Retention windows are managed by those providers and not by us. For details, please review:

- OpenRouter Privacy: https://openrouter.ai/privacy
- OpenRouter Terms: https://openrouter.ai/terms

### **2.3 No Facial Recognition**
The Application does **not** perform facial recognition, identity matching, or biometric extraction. The AI model is asked to critique the presentation quality of a dating profile (photo variety, lighting, prompts, bio fields) — not to identify any individual.

### **2.4 Sensitive Information Within Screenshots**
Dating-profile screenshots can incidentally contain sensitive information — for example, text on the profile that reveals sexual orientation, religious views, or health details. Where such information appears in the screenshots you submit, it is processed **only on the basis of the explicit consent** you give on the in-app consent screen, solely to generate your requested audit, and is subject to the same no-storage rule as the rest of your screenshots (Sections 1.3 and 2.1). We do **not** extract, infer, categorize, profile, or retain any such characteristics.

### **2.5 AI Transparency — No Automated Decisions, No Training**
- All roasts, scores, and fix plans are **AI-generated content** produced for entertainment; they may be inaccurate and are not a factual assessment of any person.
- The Application makes **no automated decisions producing legal or similarly significant effects** about you (GDPR Art. 22). The output is entertainment feedback you can ignore or delete.
- We do **not** use your screenshots or results to train AI models. Submissions are forwarded solely to generate your requested audit; the AI routing provider and model providers process them under the retention terms in Section 2.2.

### **2.6 Be Careful What You Upload**
Because your screenshots are sent to a third-party AI service, you should **only upload screenshots of your own dating profile**. Avoid uploading content that contains personal information you do not want processed by an AI model — for example, other people's profiles, private chat messages, or images of other people without their consent. Crop or redact anything sensitive before uploading. You are responsible for the content you submit.

---

## **3. Third-Party Services**

The Application integrates the following third-party services. Each has its own privacy policy governing how it handles data:

| Service | Purpose | Privacy Policy |
|---|---|---|
| **Firebase Authentication** (Google) | Anonymous user identifier | https://firebase.google.com/support/privacy |
| **Cloud Firestore** (Google) | Backend database for usage counters and the 24-hour result cache | https://firebase.google.com/support/privacy |
| **Cloud Functions for Firebase** (Google) | Server-side audit generation and scoring logic | https://firebase.google.com/support/privacy |
| **Firebase Crashlytics** (Google) | Crash diagnostics | https://firebase.google.com/support/privacy |
| **Google Analytics for Firebase** | Aggregated app-usage statistics | https://firebase.google.com/support/privacy |
| **OpenRouter** | AI vision analysis routing | https://openrouter.ai/privacy |
| **Amplitude** | Anonymized product analytics | https://amplitude.com/privacy |
| **RevenueCat** | Subscription processing | https://www.revenuecat.com/privacy |
| **Apple App Store / In-App Purchase** | Payment processing for subscriptions | https://www.apple.com/legal/privacy/ |

We may also disclose information:

- as required by law, such as to comply with a subpoena or similar legal process;
- when we believe in good faith that disclosure is necessary to protect our rights, your safety, or the safety of others, investigate fraud, or respond to a government request;
- to trusted service providers who work on our behalf, do not have an independent right to use the information we disclose to them, and have agreed to adhere to the rules set forth in this policy.

---

## **4. Subscriptions and Payments**

The Application offers optional auto-renewing subscriptions that unlock the full roast text, fix plan, and re-roasts. Subscriptions are processed by **Apple via the App Store**, with subscription state mediated by **RevenueCat**.

We do **not** receive your full payment-card or App Store account credentials. We receive only the entitlement signal (whether your account currently has an active subscription) and a non-personal subscription identifier needed to verify your entitlement on this device.

For details on payment data handling, please review Apple's and RevenueCat's privacy policies linked in Section 3.

---

## **5. Analytics**

We use **Amplitude** and **Google Analytics for Firebase** to understand how users move through the Application (for example: how many people complete onboarding, how often roast generation succeeds, where users drop off). Analytics events are tied to your anonymous user identifier and contain **only metadata** — for example: screen names, feature taps, latency, error codes, subscription state, and timestamps.

Analytics events **never include**:

- The contents of your screenshots
- The text of your generated roasts, scores, or fix plans

---

## **6. Notifications**

The Application does **not** use push notifications and does not collect push tokens. If you choose to allow notifications, the Application schedules a single **local reminder on your device** (a re-roast reminder about 7 days after your roast). This reminder is created and delivered entirely on-device, can be declined at the permission prompt, and is cancelled automatically when you re-roast. You can disable notifications at any time in iOS Settings.

---

## **7. Photo Library Access**

- **Picking screenshots**: The Application uses the standard iOS photo picker, which lets you hand over only the images you select.
- **Saving share cards**: If you choose to save a score, roast, or glow-up share card, the Application asks for add-only photo library permission and writes just that image. Sharing via the share sheet is always user-initiated.

---

## **8. Children**

The Application is designed for adults who use dating apps and is intended for users aged **18 and older**. We do not knowingly collect personal information from children under 13 years of age. If you are a parent or guardian and become aware that your child has used the Application, please contact us at [support@nextline.software](mailto:support@nextline.software) and we will take appropriate steps.

---

## **9. Data Retention and Deletion**

- **Profile screenshots:** Not retained on our servers. Forwarded to the AI provider only for the duration of a single generation request.
- **Generated audit text:** Retained in a server-side processing cache for a maximum of 24 hours (Section 1.4), then deleted automatically. Retained on your device until you delete the audit or uninstall the Application.
- **Usage counters and anonymous account record:** Retained for as long as the Application is installed on your device and for a reasonable time thereafter.
- **Crash diagnostics:** Retained per Firebase Crashlytics defaults.
- **Analytics events:** Retained per Amplitude and Google Analytics defaults.

If you would like us to delete the anonymous usage record associated with your device, please contact us at [support@nextline.software](mailto:support@nextline.software). Because the account is anonymous and not tied to an email, we may need additional information from you (such as your device model and approximate first-launch date) to locate the record.

You can also stop all collection of information from this device immediately by **uninstalling the Application**.

---

## **10. Security**

We take reasonable physical, electronic, and procedural safeguards to protect the information we process. All transmissions to our backend and to third-party services occur over encrypted HTTPS / TLS connections. AI provider API credentials are held server-side only and are never embedded in the Application binary.

No method of transmission or storage is 100% secure, and we cannot guarantee absolute security.

---

## **11. International Data Transfers**

The third-party services listed in Section 3 operate globally. Your information may be processed in the United States or in other countries where these providers maintain infrastructure, including the country where the underlying AI model selected for your request is hosted.

Where personal data of users in the European Economic Area, the United Kingdom, or Switzerland is transferred to these providers, the transfer relies on recognized safeguards: an adequacy decision (including the **EU–U.S. Data Privacy Framework**, under which Google, Amplitude, and RevenueCat are certified) and/or **Standard Contractual Clauses** incorporated into the providers' data-processing terms.

---

## **12. Legal Bases for Processing (EEA / UK / Türkiye)**

Where the GDPR, UK GDPR, or Türkiye's KVKK applies, we process personal data on the following legal bases:

| Processing | Legal basis |
|---|---|
| AI analysis of the screenshots you submit (incl. any sensitive information they may incidentally contain) | **Explicit consent**, given on the in-app consent screen before your first roast (withdrawable at any time) |
| Anonymous account, usage counters, fair-use enforcement, 24-hour result cache | **Performance of a contract** (delivering the service you request) and **legitimate interests** (abuse prevention, service integrity) |
| Subscription entitlement processing | **Performance of a contract** |
| Crash diagnostics and product analytics | **Legitimate interests** (stability, security, and product improvement, using anonymous identifiers with no content) |
| Legal compliance disclosures | **Legal obligation** |

You may withdraw your AI-processing consent at any time by simply not starting further roasts, or entirely by uninstalling the Application; withdrawal does not affect the lawfulness of processing before withdrawal.

---

## **13. Your Privacy Rights**

**EEA / UK (GDPR):** You have the right to request access to, rectification of, or erasure of your personal data; restriction of or objection to processing; data portability; and the right to withdraw consent at any time. You also have the right to lodge a complaint with your local data-protection supervisory authority.

**Türkiye (KVKK Art. 11):** You have the corresponding rights to learn whether your data is processed, request information, correction, or deletion, and object to results produced exclusively by automated analysis.

**California (CCPA/CPRA):** We do not sell or share personal information as defined by the CCPA, and we collect no personal identifiers beyond the anonymous categories described above. You have the right to know, delete, and non-discrimination.

To exercise any of these rights, contact **support@nextline.software**. Because accounts are anonymous, we may need additional details (device model, approximate first-launch date) to locate your usage record; most of your content (roast history, photos) exists only on your device, where you can delete it directly (Settings → Delete my data, or uninstalling the Application).

---

## **14. Changes to This Privacy Policy**

This Privacy Policy may be updated from time to time. We will notify you of any changes by posting the new Privacy Policy on this page and updating the "Last Updated" date. Continued use of the Application after changes are posted constitutes your acceptance of those changes.

---

## **15. Transfer or Assignment**

We may share or transfer information in connection with any merger, sale of company assets, financing, or acquisition of all or a portion of our business to another company. In such an event, the acquiring company's use of information will be governed by the terms of this Privacy Policy unless otherwise notified.

---

## **16. Your Consent**

Consent for AI processing of your screenshots is collected **explicitly, in the Application, on a dedicated consent screen** before your first roast — not merely by your use of the Application. For the other processing described in this policy, the applicable legal bases are set out in Section 12.

---

## **17. Contact Us**

If you have any questions about this Privacy Policy or about our practices, please contact us:

- **Email**: [support@nextline.software](mailto:support@nextline.software)
- **Developer**: NEXTLINE YAZILIM LİMİTED ŞİRKETİ

**Last Updated**: 08/16/2026

# Privacy Policy

This Privacy Policy applies to the **Hantavirus Map & Alerts** mobile application (the "Application") created by **NEXTLINE YAZILIM LİMİTED ŞİRKETİ** ("Service Provider", "we", or "us"). The Application is offered as a Commercial service and is intended for use **"AS IS."**

By using the Application, you consent to our collection, use, and disclosure of information as described in this policy. This Privacy Policy may be updated from time to time, and we encourage you to review it periodically. Your continued use of the Application constitutes acceptance of any modifications to this policy.

---

## 1. Important Health Notice

The Application is a **public-health awareness utility**. It is **not** a medical device and does **not** diagnose disease, infection, or contamination.

- The Self-Check feature provides general awareness only — it is **not** a medical diagnosis.
- The Rodent-Sign Scanner identifies **visible environmental indicators** (such as droppings, nesting material, gnaw marks) only. It does **not** detect hantavirus, viral particles, or surface contamination.
- Outbreak data is reported third-party public-health data, displayed for informational purposes only.
- Always consult a qualified medical professional for diagnosis and treatment.

---

## 2. Information Collection and Use

### 2.1 Automatically Collected Information
When you download and use the Application, certain technical data may be automatically collected, such as:
- **IP address**
- **Device operating system and model**
- **Screens viewed, time spent on each screen, and timestamps of visits**
- **Crash diagnostics** (stack traces, non-personal device state)
- **Application locale and country code** (from device settings)

This data is used for analytics, troubleshooting, and improving the Application.

### 2.2 Anonymous Identifier (No User Account)
The Application does **not** require an email, password, or social login. It does **not** create a user account.

On first launch, an **anonymous identifier** is generated via Firebase Authentication. This identifier is local to your device and exists solely to:
- Associate your saved locations and alert preferences with your device.
- Verify your subscription entitlement when calling protected backend features.

We do **not** collect your name, email address, phone number, or any other personally identifiable contact information.

### 2.3 Location Data
The Application requests **"While Using"** location permission **once**, during post-purchase setup, **only** to suggest a first country or region for you to monitor.

- We request the **lowest precision** sufficient for country-level monitoring.
- We do **not** track your location continuously.
- We do **not** store your precise GPS coordinates.
- We do **not** request "Always" location access.
- You may decline location access and search for places manually instead.

When the permission is granted, your approximate coordinates are sent **once** to our backend reverse-geocoding function (which forwards the query to Mapbox) and discarded after a coarse place name is returned.

### 2.4 Saved Locations (User-Provided)
When you save a location to monitor, only **coarse identifiers** are stored:
- Country
- Region or state (when available)
- City (when available)
- Approximate centroid (latitude/longitude at country or region level, for map display)
- A label you choose (e.g., "Home", "Cabin")

We do **not** store street addresses. You may delete any saved location at any time from within the Application.

### 2.5 Scanner Image Processing
The Rodent-Sign Scanner allows you to capture a photo of an indoor or outdoor area to identify visible rodent signs.

When you submit a photo for analysis:
- The image is **compressed on your device** and transmitted over an encrypted connection (HTTPS) to our backend.
- Our backend forwards the image to **OpenRouter**, a third-party AI inference provider, which returns a structured description of any visible indicators.
- The image is **then discarded**.
- The image is **never persisted on our servers**. We do **not** use Firebase Storage for scanner photos.
- The image is **not** stored on your device unless you explicitly save the resulting text summary as a "Recent Scan Result." Even then, the **photo itself is not retained** — only a short text description of what the analysis returned.

You may delete locally stored Recent Scan Results at any time from within the Application.

### 2.6 Self-Check Responses
Your answers to the Exposure Risk Self-Check are processed locally on your device for a single session and are **not** persisted, transmitted, or stored anywhere.

### 2.7 Push Notification Token
If you grant notification permission, the Application stores a Firebase Cloud Messaging (FCM) token associated with your anonymous identifier so that we can deliver outbreak advisories for your saved locations. You may revoke notification permission at any time in your device settings.

### 2.8 Subscription State
Subscription purchases are processed by Apple and managed through **RevenueCat**. We receive subscription status (active / expired) so we can grant or revoke access to premium features. We do **not** receive your full payment information from Apple.

### 2.9 Outbreak Data
The Application displays public-health outbreak data licensed from **HantaCount** under the **Creative Commons Attribution 4.0 International (CC-BY-4.0)** license. This is data we display **to you** — it is not collected **from** you.

---

## 3. Premium Features & In-App Purchases

### Subscription Plans
Hantavirus Map & Alerts offers premium subscriptions that unlock the Application's features, including the outbreak map, saved-location monitoring, alerts, the rodent-sign scanner, exposure self-check, and safe cleanup guidance.

### Free Trial
The 6-month subscription includes a **7-day free trial**. If you do not cancel before the free trial ends, your payment method will be charged for the subscription. Trial eligibility is determined by Apple and may be limited to one trial per Apple ID.

### Billing & Renewal
- Subscriptions are billed through your Apple ID account at confirmation of purchase.
- Subscriptions automatically renew unless auto-renew is turned off at least 24 hours before the end of the current billing period.
- Your account will be charged for renewal within 24 hours prior to the end of the current period at the rate of the selected plan.
- You may manage or cancel your subscription by going to your Account Settings on the App Store after purchase.

### Refunds
Refund requests are handled by Apple in accordance with the App Store refund policy. We do not process refunds directly.

---

## 4. Third-Party Services

The Application uses third-party services that have their own privacy policies. We recommend reviewing their policies:

- [Google Firebase (Authentication, Firestore, Cloud Functions, Cloud Messaging, Crashlytics, Analytics)](https://firebase.google.com/support/privacy)
- [Amplitude](https://amplitude.com/privacy)
- [RevenueCat](https://www.revenuecat.com/privacy)
- [Mapbox](https://www.mapbox.com/legal/privacy) — used for map rendering and server-side geocoding
- [OpenRouter](https://openrouter.ai/privacy) — used to process scanner photos for visible rodent-sign analysis
- [Apple App Store](https://www.apple.com/legal/privacy) — used for subscription billing
- [HantaCount](https://hantacount.com) — public outbreak data source (CC-BY-4.0); data flows to your device, not from it

### Data Disclosure
We may disclose information:
- As required by law
- To protect our rights or user safety
- To investigate fraud or abuse
- To trusted service providers acting on our behalf
- To AI processors (such as OpenRouter) **solely** to generate scanner analysis results, with no retention after the request completes

All data transfers occur over encrypted connections (HTTPS).

---

## 5. Children

The Application is not directed to children under the age of 13. We do not knowingly collect personally identifiable information from children under 13. If you are a parent or guardian and believe your child has provided information through the Application, please contact us at **support@nextline.software** and we will take appropriate action.

---

## 6. Opt-Out Rights

You can stop all collection of information by the Application by **uninstalling it** through the standard process provided by your device or the App Store.

You may also:
- Disable location permission in your device settings.
- Disable notification permission in your device settings.
- Delete saved locations from within the Application.
- Delete Recent Scan Results from within the Application.
- Cancel your subscription through your Apple ID Account Settings.

---

## 7. Data Retention Policy

We retain the anonymous data described in this policy for as long as you use the Application and for a reasonable period afterward for backup, fraud prevention, and analytics integrity.

To request deletion of data associated with your anonymous identifier, email **support@nextline.software**. Because the Application does not require an account, please include reasonable identifying details so we can locate your record (for example, the country code of your saved location and the approximate date you began using the Application).

---

## 8. Security

We use physical, electronic, and procedural safeguards to protect your data. All transmissions to third-party services occur over encrypted connections (HTTPS). Sensitive backend operations require authentication and are protected by rate limits and abuse-detection logging.

No method of transmission or storage is completely secure. We cannot guarantee absolute security, but we work to follow industry-standard practices.

---

## 9. Changes to This Privacy Policy

This Privacy Policy may be updated periodically. We will notify you of material changes by updating this page. Your continued use of the Application after changes indicates acceptance of the updated policy.

---

## 10. Your Consent

By using the Application, you consent to the processing of your information as described in this Privacy Policy.

---

## 11. Contact Us

For privacy-related questions, requests, or concerns:

**Email:** support@nextline.software

**Last Updated:** May 13, 2026

---

*This Privacy Policy was prepared for NEXTLINE YAZILIM LİMİTED ŞİRKETİ and reflects the real behavior of the Hantavirus Map & Alerts application as of the date above.*

# Privacy Policy

This Privacy Policy applies to the **Object Remover from Image** mobile application (the "Application") created by **NEXTLINE YAZILIM LİMİTED ŞİRKETİ** ("Service Provider", "we", or "us"). The Application is offered as a Commercial service and is intended for use **"AS IS."**

By using the Application, you consent to our collection, use, and disclosure of information as described in this policy. This Privacy Policy may be updated from time to time, and we encourage you to review it periodically. Your continued use of the Application constitutes acceptance of any modifications to this policy.

---

## 1. Information Collection and Use

### 1.1 Automatically Collected Information
When you download and use the Application, certain data may be automatically collected, such as:
- **IP Address**
- **Device operating system**
- **Pages/screens visited**
- **Time spent on each page** and timestamps of visits

We may use this data for analytics, troubleshooting, and improving the Application.

### 1.2 Location Data
The Application does **not** collect GPS-based or precise location information. We collect only your device's timezone for the purpose of scheduling local notifications.

### 1.3 User-Provided Information
To improve your experience, we may collect:
- User ID (anonymous identifier generated via Firebase Authentication)
- Device ID (auto-generated anonymous identifier)

This information is used as described in this policy.

### 1.4 Image & Photo Processing Data
The Application allows users to select or capture photos for background removal and object removal.

**Background Removal:**
Background removal is performed **entirely on your device** using an on-device AI model (ONNX Runtime). Your photos are:
- **Never uploaded** to external servers or cloud services for background removal
- **Never transmitted** over the internet for background removal processing
- **Never stored** on our servers

**Object Removal:**
Object removal requires cloud-based AI processing. When you use the object removal feature:
- Your selected photo and the brush mask you create are **transmitted securely (via HTTPS)** to our cloud processing service powered by **Stability AI**
- The image is processed by Stability AI's inpainting technology and the result is returned to your device
- **Images are not permanently stored** on our servers or Stability AI's servers after processing is complete
- Processing is performed through our secure Firebase Cloud Function, which acts as a proxy and does not retain your images

Thumbnails of recent edits are stored locally on your device for convenience and are never transmitted externally.

### 1.5 Local Notifications
The Application may send local push notifications to your device (e.g., reminders or feature suggestions). These notifications are generated entirely on your device and do not involve any data transmission to external servers. You can disable notifications at any time through your device settings.

---

## 2. Analytics & Tracking

### 2.1 Analytics Data
We use **Amplitude** to collect anonymized usage analytics, including:
- Feature usage events (e.g., which editing tools are used)
- Session data (app opens, screen views)
- Conversion events (subscription interactions)
- Onboarding completion
- Processing duration metrics

Analytics data is associated with an anonymous user ID and does not include personally identifiable information such as your name, email address, or phone number.

### 2.2 Advertising Tracking
The Application may request access to your device's Identifier for Advertisers (IDFA) through Apple's App Tracking Transparency framework on iOS. This is used for analytics attribution purposes. You may decline this request, and the Application will continue to function normally without IDFA access.

---

## 3. Third-Party Services

The Application uses third-party services with their own Privacy Policies:

- [Firebase Authentication](https://firebase.google.com/support/privacy) — anonymous user authentication
- [Firebase Crashlytics](https://firebase.google.com/support/privacy) — crash reporting and error diagnostics
- [Firebase Cloud Functions](https://firebase.google.com/support/privacy) — secure cloud processing proxy for object removal
- [Stability AI](https://stability.ai/privacy-policy) — AI-powered object removal processing
- [Amplitude](https://amplitude.com/privacy) — anonymized usage analytics
- [RevenueCat](https://www.revenuecat.com/privacy) — subscription and purchase management

### Data Disclosure
We may disclose information:
- As required by law
- To protect our rights or user safety
- To investigate fraud
- To trusted service providers listed above

All data transfers to third-party services are encrypted (HTTPS).

---

## 4. Opt-Out Rights
You may stop all data collection by uninstalling the Application using your device's standard uninstall process.

---

## 5. Data Retention Policy
We retain analytics and crash reporting data as long as you use the Application and for a reasonable period afterward.

Images processed through the object removal feature are not permanently stored on our servers or third-party servers. Background removal processing occurs entirely on your device.

Thumbnails of recent edits are stored locally on your device and can be cleared by deleting the app or clearing app data.

You may request deletion of any data associated with your anonymous user ID at: **support@nextline.software**

---

## 6. Children's Privacy
The Application is not intended for use by children under the age of 13. We do not knowingly collect personal information from children under 13. If we discover that a child under 13 has provided us with personal information, we will promptly delete it.

---

## 7. Security
We use physical, electronic, and procedural safeguards to protect your data. All transmissions to third-party services occur via secure encrypted connections (HTTPS).

Background removal processing remains on your device and is never exposed to network-based security risks. Object removal transmissions are encrypted end-to-end between your device and our secure cloud processing service.

---

## 8. Changes to This Privacy Policy
We may update this policy periodically. Continued use of the Application indicates acceptance of any changes.

---

## 9. Your Consent
By using the Application, you consent to the processing of your information as described in this Privacy Policy.

---

## 10. Contact Us

Email: **support@nextline.software**

**Last Updated:** March 12, 2026

---

*This Privacy Policy was generated and adapted for NEXTLINE YAZILIM LİMİTED ŞİRKETİ.*

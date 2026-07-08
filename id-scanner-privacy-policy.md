# Privacy Policy

This Privacy Policy applies to the **ID Scanner: Age Check** mobile application (the "Application") created by **NEXTLINE YAZILIM LİMİTED ŞİRKETİ** ("Service Provider", "we", or "us"). The Application is offered as a Commercial service and is intended for use **"AS IS."**

By using the Application, you consent to our collection, use, and disclosure of information as described in this policy. This Privacy Policy may be updated from time to time, and we encourage you to review it periodically. Your continued use of the Application constitutes acceptance of any modifications to this policy.

---

## 1. Information Collection and Use

### 1.1 Automatically Collected Information
When you download and use the Application, certain data may be automatically collected, such as:
- **Device operating system and version**
- **Pages/screens visited within the Application**
- **Time spent on each page/screen and dates/times of visits**
- **App performance and crash data**
- **Anonymous usage events** (e.g., that a scan was completed and its verdict type — Pass, Review, or Deny — never the contents of the scanned ID)

We may use this automatically collected information for analytics, troubleshooting, and to improve the functionality of the Application.

### 1.2 Automatically Collected Identifiers
The Application's third-party SDKs may generate and collect pseudonymous identifiers, including:
- **Analytics identifiers** (e.g., Amplitude device/user IDs)
- **Subscription identifiers** (e.g., RevenueCat anonymous app user IDs)
- **Anonymous authentication tokens** (e.g., Firebase anonymous auth IDs)
- **Crash reporting identifiers** (e.g., Firebase Crashlytics installation IDs)
- **Apple advertising attribution tokens** (Apple's privacy-preserving AdServices token, used only to measure the effectiveness of our own App Store ads; it does not identify you or your device to third parties)

These identifiers are SDK-generated, pseudonymous, and not provided by you. They are used to associate usage data, manage subscriptions, and diagnose issues. Amplitude and RevenueCat may sync identifiers to link analytics data with subscription status. **These identifiers relate to you, the app user — never to the patrons whose IDs you scan.**

### 1.3 No User-Provided Information
The Application does not require you to create an account or submit any personal information. Authentication is handled anonymously via Firebase Auth — no email, password, or profile information is collected. If you contact our support team, we may receive information you voluntarily provide, such as your email address and message contents.

---

## 2. Camera Data

The Application uses your device's camera solely to read the PDF417 barcode printed on the back of US and Canadian identity documents. **All barcode reading and verdict processing is performed entirely on your device.** The Application does not take, store, or transmit photographs of IDs or people — the camera feed is used only for live barcode detection and is never saved or uploaded.

---

## 3. Scanned ID (Patron) Data

This is the most important section of this policy. When you scan the barcode on a patron's ID, the Application processes the barcode data **entirely on your device** to produce an age-verification verdict. No scanned ID data is ever sent to us or to any third party.

### 3.1 What is stored on your device
For each scan, the Application stores a local record containing:
- The verdict (Pass / Review / Deny) and the reason for it
- The patron's age and date of birth
- The document's expiration date, issuing state/province, and gender field (if present in the barcode)
- A cryptographic hash of the document number (see 3.2)
- Any note or tag you add manually

### 3.2 What is never stored
- **Patron names, addresses, and photographs are never stored.**
- **Raw document numbers are never stored or logged.** To power duplicate-scan (pass-back), banned, and VIP checks, the document number is immediately converted into a salted HMAC-SHA256 hash. The salt is generated on your device and kept in the device Keychain, so the hash is meaningless anywhere outside your device.

### 3.3 How it is protected
Scan history, banned-list, and VIP-list data are stored in **AES-encrypted local database files (Hive)**. The encryption key is generated on your device and stored in the secure Keychain. This data never leaves your device unless you explicitly export it (see Section 5).

### 3.4 What never reaches analytics
Analytics events carry the app funnel and the verdict **type** only. A patron's name, date of birth, address, document number, or document hash is **never** included in any analytics or crash-reporting event.

---

## 4. Locally Stored Data

In addition to scan records, the Application stores data on your device using local storage (Hive), including:
- **Daily visitor counters and statistics** (aggregate counts only)
- **App preferences** (age threshold, onboarding status, settings)
- **Premium status cache**

This data is stored on your device only and is not transmitted to our servers. You can delete scan history and counters from within the Application's Settings, or delete everything by clearing app data in your device settings or uninstalling the Application.

---

## 5. Exports You Create

The Application lets subscribers export their scan log as a CSV or PDF file through the device's native share sheet. Exports are **created only when you request them** and are handed directly to the destination you choose (email, file storage, etc.). Exported logs contain the scan details described in Section 3.1 (verdict, age, date of birth, expiry, issuing state, notes) — document hashes are never included in exports. Once you share an export, its handling is under your control and responsibility.

---

## 6. Location Data

The Application does **not** access your device's GPS and never requests location permissions. However, when analytics events are uploaded, our analytics provider (Amplitude) may estimate an approximate, city-level location from your IP address. This coarse location relates to you, the app user, is used only for aggregate usage statistics, and is never combined with any scanned ID data. Patron addresses read from scanned IDs are processed and stored only on your device (see Section 3).

---

## 7. Third-Party Services

The Application utilizes certain third-party services that have their own Privacy Policies regarding data handling. These services receive only the app-usage data described in Section 1 — never scanned ID data. Below are links to these third-party service providers' Privacy Policies:

- [Google Analytics for Firebase](https://firebase.google.com/support/privacy)
- [Firebase Crashlytics](https://firebase.google.com/support/privacy)
- [Amplitude](https://amplitude.com/privacy)
- [RevenueCat](https://www.revenuecat.com/privacy)

---

## 8. No Tracking

The Application does not track you. It does not access the Apple advertising identifier (IDFA), does not request App Tracking Transparency permission, and does not share your data with third parties for advertising or data-broker purposes. Analytics identifiers described in Section 1 are used only for our own product analytics and subscription management. Patron ID data is never used for tracking under any circumstances.

---

## 9. Data Disclosure

We may disclose automatically collected information:
- As required by law, such as to comply with a subpoena or similar legal process
- When we believe in good faith that disclosure is necessary to protect our rights, your safety or the safety of others, investigate fraud, or respond to a government request
- To trusted service providers who work on our behalf and agree to adhere to the rules set forth in this Privacy Policy

We cannot disclose scanned ID data because we never receive it — it exists only on your device.

---

## 10. Opt-Out Rights

You can stop all collection of information by the Application easily by uninstalling it. Use the standard uninstall processes available on your mobile device or via the mobile application marketplace.

---

## 11. Data Retention

- **Locally stored data** (scan history, banned/VIP lists, counters, preferences) is stored on your device and remains there until you clear it in the Application's Settings, clear the Application's data, or uninstall the Application. We do not have access to this data.
- **Third-party service data** (analytics events, crash reports, subscription records) is retained according to each provider's own data retention policies. Please refer to the privacy policies linked in Section 7 for details.

Some jurisdictions limit how long businesses may retain information obtained from scanning identity documents. As the operator of the device, you are responsible for clearing scan history in accordance with the laws that apply to your venue.

---

## 12. Children

The Application is a professional tool intended for venue staff and is not directed at children under 13. We do not knowingly collect personal information from children.

---

## 13. Security

We take reasonable measures (physical, electronic, and procedural safeguards) to protect information under our control from unauthorized access or disclosure. Scan history and banned/VIP lists are stored in AES-encrypted databases, with encryption keys and hashing salts held in the device's secure Keychain. Any transmissions to third-party services are encrypted via secure connections (HTTPS).

---

## 14. Changes to This Privacy Policy

This Privacy Policy may be updated from time to time for any reason. We will notify you of any changes by posting the new Privacy Policy on this page, and we will update the "Last Updated" date. Please review this Privacy Policy periodically for updates. Continued use of the Application after changes are posted constitutes your acceptance of those changes.

---

## 15. Your Consent

By using the Application, you consent to the processing of your information as described in this Privacy Policy, now and as amended by us.

---

## 16. Contact Us

If you have any questions regarding privacy while using the Application or have questions about our practices, please contact us via email:

- **Email**: [support@nextline.software](mailto:support@nextline.software)

**Last Updated**: *July 8, 2026*

---

*This privacy policy page was generated by [App Privacy MD Generator](https://github.com/nextline-yazilim/app-privacy-md-generator)*

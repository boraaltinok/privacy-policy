# Privacy Policy

This Privacy Policy applies to the **Menu Maker** mobile application (the "Application") created by **NEXTLINE YAZILIM LİMİTED ŞİRKETİ** ("Service Provider", "we", or "us"). The Application is offered as a Commercial service and is intended for use **"AS IS."**

By using the Application, you consent to our collection, use, and disclosure of information as described in this policy. This Privacy Policy may be updated from time to time, and we encourage you to review it periodically. Your continued use of the Application constitutes acceptance of any modifications to this policy.

---

## 1. Information Collection and Use

### 1.1 Automatically Collected Information
When you download and use the Application, certain data may be automatically collected, such as:
- **Device operating system and version**
- **Pages/screens visited within the Application**
- **Time spent on each page/screen and dates/times of visits**
- **App performance and crash data**

We may use this automatically collected information for analytics, troubleshooting, and to improve the functionality of the Application.

### 1.2 Automatically Collected Identifiers
The Application's third-party SDKs may generate and collect pseudonymous identifiers, including:
- **Analytics identifiers** (e.g., Amplitude and Google Analytics for Firebase device/instance IDs)
- **Subscription identifiers** (e.g., RevenueCat anonymous app user IDs)
- **Anonymous authentication tokens** (e.g., Firebase anonymous auth IDs)
- **Crash reporting identifiers** (e.g., Firebase Crashlytics installation IDs)

These identifiers are SDK-generated, pseudonymous, and not provided by you. They are used to associate usage data, manage subscriptions, and diagnose issues. Amplitude and RevenueCat may sync identifiers to link analytics data with subscription status.

### 1.3 Install Attribution
On iOS, the Application uses Apple's Ad Services framework to collect a short-lived attribution token. This token is used only to measure which advertising campaign led you to install the Application. It is a lightweight install-attribution signal — it is **not** an advertising identifier, it does **not** identify you personally, and it is **not** used to track you across other apps or websites.

### 1.4 No Account or User Profile
The Application does not require you to create an account, register, or log in, and it does not collect any name, email, password, or profile information for use of the app. Authentication is handled **anonymously** via Firebase Auth — an anonymous, SDK-generated identifier is created automatically so the Application can function. If you contact our support team, we may receive information you voluntarily provide, such as your email address and the contents of your message.

---

## 2. Menu Content You Create

The Application is a menu builder. You provide content such as dish names, descriptions, prices, venue name and details, and an optional venue logo or images. This content is entered manually or produced by the AI import feature described in Section 3.

- **Local storage.** By default, the menus you build are stored **locally on your device** (using Hive). Private drafts remain on your device and are **not** transmitted to our servers.
- **Publishing is your choice.** When — and only when — you choose to **publish** a menu, that menu (including its text, logo, and any images) is uploaded to and hosted on Google Firebase (Hosting/Storage) and served at a **public web address** (for example, `menu-maker-fb.web.app/...`). A published menu is **publicly accessible by design**: anyone who has the QR code or link can view it. Do not include information in a published menu that you do not want to be public.
- **You stay in control.** You decide whether to publish, what to publish, and when to update or unpublish a menu. Unpublishing or updating a menu changes what is served at the public address going forward.

---

## 3. Camera, Photos, and AI Import

### 3.1 Camera and Photo Library
With your permission, the Application can use your device's **camera** to scan a paper menu, and your **photo library** to select menu photos and a venue logo. A logo or image you select may be included in a menu you choose to publish.

### 3.2 AI Import and Translation (Remote Processing)
When you use **AI import**, the menu photo you capture or select is **uploaded to our backend** (Google Firebase Cloud Functions, region europe-west1), where an AI service extracts the text into a structured menu. Similarly, when you use the premium **translation** feature, your menu text is sent to our backend for AI processing. This processing is performed **remotely**, not on your device.

Menu photos transmitted for AI import are used only to return the extracted result to you and are **not retained beyond what is necessary** to perform that processing.

### 3.3 Accuracy Disclaimer
AI extraction and translation are automated and **may contain errors, omissions, or inaccuracies**. You are responsible for reviewing and correcting the results before using or publishing your menu.

---

## 4. Locally Stored Data

The Application stores data on your device using local storage (Hive), including:
- **Menus you build** (dishes, descriptions, prices, venue details)
- **Cached thumbnails and images**
- **App preferences** (theme, settings, onboarding status)
- **Premium status cache**

This data is stored on your device only and is not transmitted to our servers, except where you choose to publish a menu (see Section 2) or use AI import/translation (see Section 3). You can delete locally stored data at any time by clearing app data in your device settings or by uninstalling the Application.

---

## 5. Subscriptions and Payments

Premium features are offered through **auto-renewable subscriptions** managed via RevenueCat. RevenueCat generates an anonymous app-user ID to associate your subscription entitlements with your device. All purchases are processed by **Apple's App Store** — we never receive or store your payment card or billing details.

---

## 6. Notifications

The Application may use **local notifications** (on-device reminders) only. It does **not** send push notifications and does **not** use remote messaging services.

---

## 7. Location Data

The Application does **not** gather information about the location of your mobile device.

---

## 8. Third-Party Services

The Application utilizes certain third-party services that have their own Privacy Policies regarding data handling. Below are links to these third-party service providers' Privacy Policies:

- [Google Firebase](https://firebase.google.com/support/privacy) (Anonymous Authentication, Cloud Functions, Storage, Hosting, Crashlytics, Google Analytics for Firebase)
- [Amplitude](https://amplitude.com/privacy)
- [RevenueCat](https://www.revenuecat.com/privacy)
- [Apple](https://www.apple.com/legal/privacy/) (App Store subscriptions and Ad Services attribution)

---

## 9. Data Disclosure

We may disclose automatically collected information:
- As required by law, such as to comply with a subpoena or similar legal process
- When we believe in good faith that disclosure is necessary to protect our rights, your safety or the safety of others, investigate fraud, or respond to a government request
- To trusted service providers who work on our behalf and agree to adhere to the rules set forth in this Privacy Policy

---

## 10. Opt-Out Rights

You can stop all collection of information by the Application easily by uninstalling it. Use the standard uninstall processes available on your mobile device or via the mobile application marketplace. You may also choose not to grant camera or photo-library permissions, not to use AI import or translation, and not to publish any menu.

---

## 11. Data Retention

- **Locally stored data** (menus, preferences, cached images) is stored on your device and remains there until you clear the Application's data or uninstall it. We do not have access to this data.
- **Menu photos uploaded for AI import** are retained only as long as necessary to perform the extraction and return the result.
- **Published menus** remain hosted and publicly accessible until you unpublish them or request their removal.
- **Third-party service data** (analytics events, crash reports, subscription records) is retained according to each provider's own data retention policies. Please refer to the privacy policies linked in Section 8 for details.

---

## 12. Security

We take reasonable measures (physical, electronic, and procedural safeguards) to protect information under our control from unauthorized access or disclosure. Any transmissions to third-party services and to our backend are encrypted via secure connections (HTTPS). Locally stored data is protected by your device's built-in security mechanisms. Please note that content you choose to publish is intentionally made publicly accessible and is not protected by these access controls.

---

## 13. Changes to This Privacy Policy

This Privacy Policy may be updated from time to time for any reason. We will notify you of any changes by posting the new Privacy Policy on this page, and we will update the "Last Updated" date. Please review this Privacy Policy periodically for updates. Continued use of the Application after changes are posted constitutes your acceptance of those changes.

---

## 14. Your Consent

By using the Application, you consent to the processing of your information as described in this Privacy Policy, now and as amended by us.

---

## 15. Contact Us

If you have any questions regarding privacy while using the Application or have questions about our practices, please contact us via email:

- **Email**: [support@nextline.software](mailto:support@nextline.software)

**Last Updated**: *July 13, 2026*

---

*This privacy policy page was generated by [App Privacy MD Generator](https://github.com/nextline-yazilim/app-privacy-md-generator)*

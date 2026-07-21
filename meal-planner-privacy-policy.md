# Privacy Policy — Meal Planner

**Last updated: July 22, 2026**

This Privacy Policy explains how **NEXTLINE YAZILIM LİMİTED ŞİRKETİ** ("NEXTLINE", "we", "us", or "our") handles information in connection with the **Meal Planner** mobile application (the "App").

We built Meal Planner to be private by design. The App works **offline** and does **not require you to create an account or sign in**. The meal plans, preferences, grocery lists, and history you create are stored **only on your device**. This policy describes the limited data that the App processes and the third-party services we rely on for diagnostics, analytics, and subscriptions.

---

## 1. Summary

- **No account required.** You can use the App without registering, logging in, or providing your name, email, or password.
- **Your meal-planning data stays on your device.** Your diet, allergen, and household preferences, your weekly plans, grocery lists, favorites, and history are stored locally using on-device storage. We do not upload or store them on our servers.
- **We collect limited diagnostic and analytics data** to keep the App stable and understand how it is used, and we process subscription data to manage premium purchases.
- **We do not sell your personal data** and we do **not** use it for cross-app advertising or tracking. The App does not display ads.

---

## 2. Information Stored Only on Your Device

The following information is created and stored **locally on your device** and is **not transmitted to us**:

- Your profile preferences: diet, allergen selections, household size, cooking rhythm, and meal-slot settings.
- Your generated weekly meal plans and any edits you make.
- Your grocery lists and their checked/unchecked state.
- Favorites, blocked recipes, and plan history.
- App settings and flags (for example, whether you have completed onboarding).

Because this data lives only on your device, you remain in control of it. Removing this data is as simple as deleting the relevant items in the App or uninstalling the App, which erases the local data.

---

## 3. Information Collected Automatically

To operate, secure, and improve the App, we and our service providers process the following:

### a. Diagnostic / Crash Data
If the App crashes or encounters an error, crash reports and diagnostic information (such as the type of error, a stack trace, device model, operating-system version, and app version) are collected through **Firebase Crashlytics** to help us fix problems.

### b. Usage Analytics
We use **Amplitude** to understand how the App is used in aggregate — for example, app-open and session events, whether you are a new or returning user, the platform (iOS/Android), and event timestamps. This helps us prioritize improvements.

### c. Device / Anonymous Identifier
The App generates an **anonymous identifier** to associate diagnostic, analytics, and subscription information for a given installation. Depending on availability, this identifier is an anonymous Firebase authentication ID, a RevenueCat installation ID, or a locally generated random ID stored on your device. This identifier is **not** your name, email, or a persistent advertising identifier, and it is not used to track you across other apps or websites.

We do **not** collect your precise location, contacts, photos, microphone, or camera data. The App does not request those permissions.

---

## 4. Information You Choose to Submit

**Recipe issue reports.** If you choose to report a problem with a recipe, the App sends us the report so we can correct our content. A report contains the recipe identifier, the content-pack version, the reason you selected, an optional free-text note you type (up to 500 characters), your app language, and the app version, along with your anonymous identifier. These reports are stored using **Google Firebase (Cloud Firestore)**. Please do not include personal or sensitive information in the optional note.

---

## 5. AI Meal Arrangement (Optional Feature)

Meal Planner assembles your weekly plan using a **deterministic engine that runs entirely on your device** against a recipe pack bundled with the App. This on-device engine is the default and requires no network connection.

The App also includes an **optional AI-assisted arrangement** feature that, when enabled, can rearrange recipes that have **already been filtered on your device** to better match your preferences. When this optional feature is active and you have consented to it, the App sends the following to our secure cloud function (Google Firebase Cloud Functions), which relays it to our AI provider (**OpenRouter**) for processing:

- Preference values used for arrangement: household size, cooking rhythm, variety setting, selected meal "moods", budget target and currency, and enabled meal slots.
- An optional free-text note you type for the week (please avoid including personal or sensitive information).
- A list of pre-filtered candidate recipes (identifiers and recipe metadata from the bundled content pack).
- Non-identifying request metadata (app version, language, content-pack version, and whether the installation has premium access).

The AI service only **selects and orders recipes from the pre-filtered list**; it does not generate medical advice, and no result is used unless it passes the App's on-device allergen and safety re-check. If the feature is disabled, is unavailable, or fails for any reason, the App silently uses the on-device engine instead. This feature does not run without your consent.

> **Note:** This optional AI feature is disabled in the current release and may be enabled in a future update. Where it is active, the processing described above applies.

---

## 6. Subscriptions and Purchases

Premium features are offered through auto-renewable subscriptions processed by **Apple App Store** or **Google Play** and managed through **RevenueCat**. When you purchase or restore a subscription, RevenueCat processes purchase and entitlement information (such as product identifiers, purchase and expiration status, and the anonymous identifier described above) so we can unlock premium features and validate receipts. **We never receive or store your full payment-card details** — payment is handled entirely by the App Store or Google Play.

---

## 7. How We Use Information

We use the information described above to:

- Provide, operate, and maintain the App and its features.
- Diagnose crashes and fix bugs (Crashlytics).
- Understand aggregate usage and improve the product (Amplitude).
- Process and validate subscriptions and unlock premium features (RevenueCat / App Store / Google Play).
- Respond to and act on recipe issue reports you submit.
- Provide the optional AI meal-arrangement feature when you enable and consent to it.

---

## 8. Third-Party Services

The App relies on the following third-party providers, each of which processes data under its own privacy policy:

| Provider | Purpose | Data processed |
|----------|---------|----------------|
| Google Firebase Crashlytics | Crash & diagnostics | Crash reports, device/OS/app version, anonymous ID |
| Google Firebase (Authentication – anonymous, Cloud Firestore) | Anonymous identifier; storage of recipe issue reports; app version/config lookup | Anonymous ID; issue-report contents |
| Google Firebase Cloud Functions + OpenRouter | Optional AI meal arrangement (when enabled) | Preference values, optional note, pre-filtered recipe list, request metadata |
| Amplitude | Product analytics | Usage events, platform, timestamps, anonymous ID |
| RevenueCat | Subscription management | Purchase/entitlement status, anonymous ID |
| Apple App Store / Google Play | Payment processing | Handled by the platform; we do not receive card details |

We encourage you to review these providers' privacy policies for details on their processing.

---

## 9. Data Sharing

We do **not** sell your personal data. We share information only with the service providers listed above, strictly to provide the functions described in this policy, and where required by law.

---

## 10. Data Retention

- **On-device data** remains until you delete it in the App or uninstall the App.
- **Diagnostic and analytics data** is retained according to our service providers' standard retention periods and our operational needs.
- **Recipe issue reports** are retained as long as needed to improve our content.

---

## 11. Your Rights

Depending on where you live (for example, under the EU/UK GDPR, Turkey's KVKK, or the California CCPA/CPRA), you may have rights to access, correct, delete, or restrict processing of personal data, and to object to certain processing. Because most of your data is stored only on your device and we do not maintain user accounts, you can exercise many of these rights directly by editing or deleting data in the App or by uninstalling it. For requests concerning diagnostic, analytics, subscription, or issue-report data, contact us at **support@nextline.software**, and we will respond as required by applicable law.

---

## 12. Children's Privacy

The App is not directed to children under 13 (or the minimum age required in your jurisdiction), and we do not knowingly collect personal data from children. If you believe a child has provided us with personal data, please contact us and we will delete it.

---

## 13. Tracking and Advertising

The App does **not** display advertising and does **not** track you across other companies' apps or websites. We do not use the Apple Advertising Identifier (IDFA) for tracking, and the App does not present an App Tracking Transparency prompt because it collects no cross-app tracking data.

---

## 14. Data Security

We use reasonable technical and organizational measures, and rely on the security practices of our reputable service providers, to protect information. No method of transmission or storage is completely secure, and we cannot guarantee absolute security.

---

## 15. International Transfers

Our service providers may process data in countries other than your own. Where required, we rely on appropriate safeguards for such transfers.

---

## 16. Changes to This Policy

We may update this Privacy Policy from time to time. We will revise the "Last updated" date above and, where appropriate, provide additional notice. Your continued use of the App after changes take effect constitutes acceptance of the updated policy.

---

## 17. Contact Us

If you have questions about this Privacy Policy or our data practices, contact us at:

**NEXTLINE YAZILIM LİMİTED ŞİRKETİ**
Email: **support@nextline.software**

# Privacy Policy

_Last updated: 2026-07-21_

Thank you for using **Golf Handicap Tracker** ("Application"). This Privacy Policy explains how NEXTLINE YAZILIM LİMİTED ŞİRKETİ ("Service Provider", "we", or "us") handles information when you use our Application.

The Application is a personal golf handicap calculator and tracker based on the World Handicap System (WHS) formulas. **Your golf rounds are stored locally on your device.** We do not host user accounts, and we do not store your rounds on our servers. The optional iCloud sync feature (Premium) stores your data in **your own private iCloud container**, managed by Apple — not on servers we operate.

## 1. Information We Handle

### Stored Locally on Your Device (not transmitted to us)

Your golf data stays on your device. The Application uses local storage to keep:

- **Saved rounds**: course name, tee, course rating, slope rating, number of holes, your adjusted gross score, the computed score differential, and the date played.
- **Manually entered courses**: course names and rating/slope values you type in, saved for one-tap reuse.
- **Computed handicap data**: your Handicap Index history and trend, derived on your device from your rounds.
- **Preferences and flags**: settings such as the reminder toggle, iCloud sync toggle, onboarding status, and a randomly generated anonymous device identifier.
- **Bundled course catalog**: a read-only course list shipped inside the Application.

This data lives in the Application's local database. Uninstalling the Application removes it. On the free tier, entered rounds are kept only for the current session and are cleared when the Application restarts; Premium saves them persistently.

### iCloud Sync (Premium, optional)

If you are a Premium user and iCloud sync is enabled, the Application saves a snapshot of your rounds (`rounds.json`, including the anonymous device identifier) to **your private iCloud container** (`iCloud.com.nextline.golfhandicaptracker`). This data is:

- stored in your personal iCloud account and governed by Apple's privacy policies;
- **not** accessible to us — we operate no server and cannot read your iCloud data;
- removable by disabling iCloud sync in the Application's Settings, or by deleting the Application's iCloud data in your device's iCloud settings.

Separately, if iCloud Backup is enabled on your device, your local data may be included in your device backup according to your Apple settings.

### Information Automatically Collected by Third-Party SDKs

When you use the Application, certain technical information may be collected by integrated third-party SDKs to operate, secure, and improve the Application. **Your rounds, scores, course entries, and handicap values are never sent to any of these SDKs as content.**

- **Anonymous device identifier** generated for subscription tracking (RevenueCat). Purchases are processed by Apple; we never receive your payment card details.
- **Crash diagnostics** when the Application crashes, including device model, OS version, and stack trace (Firebase Crashlytics).
- **Anonymous usage events** describing in-app actions in metadata form — for example: screens viewed, save/paywall funnel steps, and plan types selected (Amplitude, Google Analytics for Firebase). The events do not include the content of your rounds.
- **Read-only application configuration**: on launch, the Application may fetch remote configuration values (Firebase Remote Config) used to enable or disable the paywall by region. This is an **inbound-only** read; we do not write any user data to Firebase.
- **Network-level data** such as IP address may be observed by these third-party SDKs as part of normal operation.

We do not collect:

- Your name, email, phone number, or any contact information.
- Your precise or approximate location.
- Photos, camera footage, microphone audio, contacts, calendar, health data, or files outside the Application's own storage.
- The IDFA / advertising identifier. The Application does not show the App Tracking Transparency prompt and does not track you across apps.
- Any biometric data.

The Application does not display third-party advertisements and does not include any ad SDK.

## 2. How We Use Information

We use the information described above only to:

- Provide the core handicap functionality (entering rounds, calculating your Handicap Index, showing history and trends) — entirely on your device.
- Sync your rounds between your own devices via your private iCloud container, if you enable Premium iCloud sync.
- Process subscription and lifetime purchases and restore prior purchases via RevenueCat.
- Diagnose crashes and improve stability via Firebase Crashlytics.
- Understand aggregate, anonymous usage patterns to improve the Application via Amplitude and Firebase Analytics.

We do not sell your information. We do not use your golf data for advertising. We do not build user profiles.

## 3. Third-Party Services

The Application integrates with the following third parties. Each has its own privacy policy that governs how it handles data on its side:

- [Firebase (Crashlytics, Analytics, Remote Config)](https://firebase.google.com/support/privacy)
- [Amplitude](https://amplitude.com/privacy)
- [RevenueCat](https://www.revenuecat.com/privacy)
- [Apple iCloud (governed by Apple's policies)](https://www.apple.com/legal/privacy/)

## 4. Data Retention

**Local data**: stays on your device until you delete a round, clear the Application's data, or uninstall the Application. Free-tier session rounds are cleared automatically when the Application restarts.

**iCloud data**: stays in your private iCloud container under your Apple ID, subject to your Apple settings.

**Third-party data**: retention is governed by each provider's policy linked above. To request deletion of analytics data tied to your anonymous device identifier, please contact us at [support@nextline.software](mailto:support@nextline.software).

## 5. Security

We take reasonable measures to protect data we handle:

- All round content stays on your device or in your private iCloud container — there is no server of ours to compromise.
- Subscription identifiers are anonymous (RevenueCat).
- Crash logs are scoped to crash data, not your golf content.

No security system is perfect, and we cannot guarantee absolute security.

## 6. Children's Privacy

The Application is not directed to children under 13 and we do not knowingly collect information from children under 13. If you believe a child has used the Application, please contact us at [support@nextline.software](mailto:support@nextline.software) and we will take appropriate action.

## 7. Purchases

The Application offers optional Premium plans (auto-renewing subscriptions and a one-time lifetime purchase) managed by Apple's App Store and tracked via RevenueCat using an anonymous device identifier. Apple handles your payment information; we do not receive your payment card details. See the Terms & Conditions for purchase terms.

## 8. Your Choices

- **Notifications**: the Application only schedules a single local "played a round lately?" reminder. You can disable it in the Application's Settings or revoke notification permission in iOS Settings.
- **iCloud sync**: Premium users can turn sync off at any time in the Application's Settings.
- **Analytics & Crash data**: you can stop all collection by uninstalling the Application.
- **Local data**: you can delete individual rounds inside the Application, or remove all data by uninstalling.

## 9. Not an Official Handicap Service

The Application computes an estimate of a WHS-style Handicap Index from the scores you enter. It is an independent tool: it is not affiliated with, or endorsed by, the USGA, The R&A, or any golf association, and the number it shows is **not an official Handicap Index** for competition purposes.

## 10. Changes to This Privacy Policy

We may update this Privacy Policy from time to time. The latest version will be posted at the same URL. Continued use of the Application after changes constitutes acceptance of the updated Privacy Policy.

## 11. Contact Us

If you have questions about this Privacy Policy, please contact us at [support@nextline.software](mailto:support@nextline.software).

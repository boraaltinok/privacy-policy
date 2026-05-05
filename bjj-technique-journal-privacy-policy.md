# Privacy Policy

_Last updated: 2026-05-05_

Thank you for using **BJJ Technique Journal** ("Application"). This Privacy Policy explains how NEXTLINE YAZILIM LİMİTED ŞİRKETİ ("Service Provider", "we", or "us") handles information when you use our Application.

The Application is a personal training journal for Brazilian Jiu-Jitsu practitioners. **Your saved notes are stored locally on your device and never leave it.** We do not host user accounts, and we do not store your notes on our servers. The Application does not include AI processing of your notes.

## 1. Information We Handle

### Stored Locally on Your Device (not transmitted to us)

Your training content stays on your device. The Application uses local storage to keep:

- **Saved notes**: titles, bodies, positions, attempt outcomes, reflections, source links, and voice transcripts you create.
- **Topics and reminders**: groupings you create to organize your notes, including any short personal reminders you save.
- **Counters and preferences**: free-tier usage counters, theme, reminder schedule, and recent searches.
- **Cached configuration**: a cached copy of the Application's feature toggles.

This data lives in the Application's local database. Uninstalling the Application removes it. If iCloud Backup is enabled on your iOS device, your local data may be included in your iCloud Backup according to your Apple settings; this is a backup managed by Apple, not a sync to our servers.

### Voice Notes

If you choose to record a voice note, the Application uses **Apple's on-device speech framework** (via the `speech_to_text` integration) to transcribe your voice to text. Apple's framework decides whether transcription happens on-device or via Apple's servers based on your device, locale, and iOS settings; this is governed by Apple's privacy policies.

The audio itself is **not** sent to our backend or any third party we control — it is handled by Apple's framework only. The resulting text transcript stays on your device. Recording a voice note requires the **Microphone** and **Speech Recognition** permissions, which iOS will prompt you to grant.

### Information Automatically Collected by Third-Party SDKs

When you use the Application, certain technical information is collected by integrated third-party SDKs to operate, secure, and improve the Application. **The content of your notes, voice transcripts, search queries, and topics is never sent to any of these SDKs.**

- **Anonymous device identifier** generated for subscription tracking (RevenueCat).
- **Crash diagnostics** when the Application crashes, including device model, OS version, and stack trace (Firebase Crashlytics).
- **Anonymous usage events** describing in-app actions in metadata form — for example: input type (text / voice / link), counts, latencies, paywall trigger types, plan types selected (Amplitude, Firebase Analytics). The raw text of notes, search queries, and voice transcripts is **never** included in these events. Where note IDs are referenced, they are hashed.
- **Read-only application configuration**: on launch, the Application fetches a single public configuration document from Firebase Cloud Firestore (`app_config/paywall_settings`) used to enable or disable the paywall by region. This is an **inbound-only** read; we do not write any user data to Firestore.
- **Network-level data** such as IP address may be observed by these third-party SDKs as part of normal operation.

We do not collect:

- Your name, email, phone number, or any contact information.
- Your precise or approximate location.
- Photos, camera footage, contacts, calendar, health data, or files outside the Application's own storage.
- The IDFA / advertising identifier.
- Any biometric data.

The Application does not display third-party advertisements and does not include any ad SDK.

## 2. How We Use Information

We use the information described above only to:

- Provide the core journal functionality (saving, searching, and reflecting on notes) — entirely on your device.
- Process subscription purchases and restore prior purchases via RevenueCat.
- Diagnose crashes and improve stability via Firebase Crashlytics.
- Understand aggregate, anonymous usage patterns to improve the Application via Amplitude.

We do not sell your information. We do not use your notes for advertising. We do not build user profiles. We do not use any AI service that processes your notes.

## 3. Third-Party Services

The Application integrates with the following third parties. Each has its own privacy policy that governs how it handles data on its side:

- [Firebase (Crashlytics, Analytics, Cloud Firestore)](https://firebase.google.com/support/privacy)
- [Amplitude](https://amplitude.com/privacy)
- [RevenueCat](https://www.revenuecat.com/privacy)
- [Apple Speech Recognition (governed by Apple's policies)](https://www.apple.com/legal/privacy/)

We do **not** integrate with OpenAI, OpenRouter, or any third-party AI provider. The Application does not call any AI API.

## 4. Data Retention

**Local data**: stays on your device until you delete a note, clear app storage, or uninstall the Application.

**Third-party data**: retention is governed by each provider's policy linked above. To request deletion of analytics data tied to your anonymous device identifier, please contact us at [support@nextline.software](mailto:support@nextline.software).

## 5. Security

We take reasonable measures to protect data we handle:

- All note content stays on your device — there is no server to compromise.
- Subscription identifiers are anonymous (RevenueCat).
- Crash logs are scoped to crash data, not user content.

No security system is perfect, and we cannot guarantee absolute security.

## 6. Children's Privacy

The Application is not directed to children under 13 and we do not knowingly collect information from children under 13. If you believe a child has used the Application, please contact us at [support@nextline.software](mailto:support@nextline.software) and we will take appropriate action.

## 7. Subscriptions

The Application offers optional Premium subscriptions managed by Apple's App Store and tracked via RevenueCat using an anonymous device identifier. Apple handles your payment information; we do not receive your payment card details. See Section 7 of the Terms & Conditions for subscription terms.

## 8. Your Choices

- **Microphone & Speech Recognition**: you can revoke these permissions any time in iOS Settings. Voice notes will then be unavailable.
- **Notifications**: local reminders can be enabled or disabled in iOS Settings or in the Application's Settings screen.
- **Analytics & Crash data**: you can stop all collection by uninstalling the Application.
- **Local data**: you can delete individual notes inside the Application, or remove all data by uninstalling.

## 9. Not Medical or Professional Advice

The Application is a personal note-keeping tool for training. It is not medical, fitness, or professional coaching advice. Train safely and consult qualified instructors and medical professionals for safety, injury, and health questions.

## 10. Changes to This Privacy Policy

We may update this Privacy Policy from time to time. The latest version will be posted at the same URL. Continued use of the Application after changes constitutes acceptance of the updated Privacy Policy.

## 11. Contact Us

If you have questions about this Privacy Policy, please contact us at [support@nextline.software](mailto:support@nextline.software).

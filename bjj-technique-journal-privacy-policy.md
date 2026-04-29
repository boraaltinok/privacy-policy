# Privacy Policy

_Last updated: 2026-04-29_

Thank you for using **BJJ Technique Journal** ("Application"). This Privacy Policy explains how NEXTLINE YAZILIM LİMİTED ŞİRKETİ ("Service Provider", "we", or "us") handles information when you use our Application.

The Application is a personal training journal for Brazilian Jiu-Jitsu practitioners. Your saved notes are stored locally on your device. We do not host user accounts, and we do not store your notes on our servers.

## 1. Information We Handle

### Stored Locally on Your Device (not transmitted to us)

Your training content stays on your device. The Application uses local storage to keep:

- **Saved notes**: titles, bodies, positions, attempt outcomes, reflections, source links, and voice transcripts you create.
- **Counters and preferences**: free-tier usage counters, theme, reminder schedule, and recent searches.
- **Cached configuration**: a cached copy of the Application's feature toggles.

This data lives in the Application's local database. Uninstalling the Application removes it. If iCloud Backup is enabled on your iOS device, your local data may be included in your iCloud Backup according to your Apple settings; this is a backup managed by Apple, not a sync to our servers.

### Sent to Our Backend Only When You Use AI Features

The Application includes two optional AI features: **AI note creation** (when you save a note from text, voice, or a link) and **Ask AI** (when you ask a question about your saved notes). Only when you actively use one of these features, the following is sent to our backend (Firebase Cloud Functions) for the purpose of generating a response:

- The text content of the note you are creating, OR
- Your AI question plus a small, automatically selected subset of your saved notes (up to 3 notes, capped at roughly 3,500 characters, plus a short same-session conversation history).

Our backend forwards this content to **OpenRouter**, a third-party AI gateway, which routes the request to an AI model provider. We send a `data_collection: deny` instruction with each request, asking that the receiving provider not retain inputs for training purposes. We do not use your notes to train any model of our own. We do not store your AI requests or responses on our backend; the backend acts as a stateless proxy.

If you do not use the AI features, no note content leaves your device through these channels.

### Voice Notes

If you choose to record a voice note, the Application uses **Apple's on-device speech framework** (via the `speech_to_text` integration) to transcribe your voice to text. Apple's framework decides whether transcription happens on-device or via Apple's servers based on your device, locale, and iOS settings; this is governed by Apple's privacy policies.

The audio itself is **not** sent to our backend. Only the resulting text transcript is used by the Application, and that transcript is only sent to our backend if you proceed to save the note with AI organization. Recording a voice note requires the **Microphone** and **Speech Recognition** permissions, which iOS will prompt you to grant.

### Information Automatically Collected by Third-Party SDKs

When you use the Application, certain technical information is collected by integrated third-party SDKs to operate, secure, and improve the Application. We do not send the **content** of your notes, your AI questions, or your voice transcripts to any of these SDKs.

- **Anonymous device identifier** generated for subscription tracking (RevenueCat).
- **Crash diagnostics** when the Application crashes, including device model, OS version, and stack trace (Firebase Crashlytics).
- **Anonymous usage events** describing in-app actions in metadata form — for example: input type (text / voice / link), counts, latencies, paywall trigger types, plan types selected (Amplitude). The raw text of notes, AI questions, search queries, and voice transcripts is **never** included in these events. Where note IDs are referenced, they are hashed.
- **Network-level data** such as IP address may be observed by these third-party SDKs and by our Cloud Functions hosting provider (Google / Firebase) as part of normal operation.

We do not collect:

- Your name, email, phone number, or any contact information.
- Your precise or approximate location.
- Photos, camera footage, contacts, calendar, health data, or files outside the Application's own storage.
- The IDFA / advertising identifier.
- Any biometric data.

The Application does not display third-party advertisements and does not include any ad SDK.

## 2. How We Use Information

We use the information described above only to:

- Provide the core journal functionality (saving, searching, and reflecting on notes).
- Generate AI responses when you actively invoke an AI feature.
- Process subscription purchases and restore prior purchases via RevenueCat.
- Diagnose crashes and improve stability via Firebase Crashlytics.
- Understand aggregate, anonymous usage patterns to improve the Application via Amplitude.
- Validate that requests to our backend originate from a legitimate copy of the Application via Firebase App Check.

We do not sell your information. We do not use your notes for advertising. We do not build user profiles.

## 3. Third-Party Services

The Application integrates with the following third parties. Each has its own privacy policy that governs how it handles data on its side:

- [Firebase (Cloud Functions, Firestore, Crashlytics, App Check, Analytics)](https://firebase.google.com/support/privacy)
- [Google Cloud (hosts our Cloud Functions)](https://cloud.google.com/terms/cloud-privacy-notice)
- [OpenRouter (AI gateway)](https://openrouter.ai/privacy)
- [Amplitude](https://amplitude.com/privacy)
- [RevenueCat](https://www.revenuecat.com/privacy)
- [Apple Speech Recognition (governed by Apple's policies)](https://www.apple.com/legal/privacy/)

When you use AI features, OpenRouter routes the request to an underlying AI model provider (for example, OpenAI). That provider's terms apply to its handling of the request. We pass a no-data-retention preference (`data_collection: deny`) on each request to ask that the provider not retain or train on your input.

## 4. Data Retention

**Local data**: stays on your device until you delete a note, clear app storage, or uninstall the Application.

**Backend data**: our Cloud Functions process AI requests in transit and do not persist your note content or questions. Operational logs (such as request counts, latencies, and error codes) are retained for a short period for reliability and abuse prevention.

**Third-party data**: retention is governed by each provider's policy linked above. To request deletion of analytics data tied to your anonymous device identifier, please contact us at [support@nextline.software](mailto:support@nextline.software).

## 5. Security

We take reasonable measures to protect data we handle:

- The OpenRouter API key is held only on our server side; it is never embedded in the Application.
- Cloud Functions require **Firebase App Check** (DeviceCheck on iOS) so that only legitimate copies of the Application can invoke them.
- Firestore configuration is exposed read-only and contains no user content.
- Per-device rate limits protect the AI features from abuse.

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

# Privacy Policy

_Last updated: 2026-07-16_

This Privacy Policy explains how **AI Song Maker** ("Application"), provided by NEXTLINE YAZILIM LİMİTED ŞİRKETİ ("Service Provider", "we", "us", or "our"), handles information in connection with your use of the Application. By using AI Song Maker, you agree to the practices described below.

AI Song Maker turns an idea or occasion you describe into personalized lyrics and, for paying users, a fully sung song. Some of this processing happens on our cloud servers and with trusted AI providers, as explained below.

## Summary

- We do **not** require you to create an account, and we do **not** ask for your name, email address, or password.
- We use **anonymous sign-in**, which assigns your device a random anonymous identifier. This is not an account with personal login credentials.
- The song ideas and details you type are sent to our servers and to AI providers so we can generate your lyrics and audio.
- We do **not** sell your personal data, and the Application does **not** display third-party advertising.
- The Application does **not** access your camera, microphone, photos, precise location, or contacts.

## Information We Collect

### 1. Information You Provide (Song Inputs)

To create a song, you provide text and selections such as:

- Your song idea or freeform prompt
- The occasion (for example, a birthday or anniversary)
- A recipient name or nickname you choose to include
- Additional details you optionally add
- Genre, language, and mood selections

This content is transmitted to our cloud backend (Firebase Cloud Functions) and to our AI generation providers so we can write lyrics and produce sung audio. Please only include names or details that you have the right to share. Do not submit sensitive personal information about yourself or others.

### 2. Anonymous Identifier

The Application uses **Firebase Anonymous Authentication** to assign a random, device-scoped anonymous ID. This identifier lets your generated songs appear in your in-app Library and lets us enforce fair-use limits. It is **not** a user account: we do not collect an email address, name, password, or profile, and there is no login.

### 3. Information Collected Automatically

When you use the Application, certain information is collected automatically by us and by third-party service providers, including:

- Device information (such as device model, operating system version, and language)
- Device and installation identifiers
- App usage and interaction events (such as screens viewed and features used)
- Approximate, coarse location derived from your IP address (we do **not** collect precise GPS location)
- IP address
- Crash logs and diagnostic data

### 4. Purchase Information

If you buy a subscription or one-time purchase, our payments partner **RevenueCat** processes purchase and subscription status, receipt data, and anonymized purchase identifiers together with your anonymous ID. Payment card details are handled by Apple or Google, not by us.

## How Your Songs Are Stored and Retained

- Generated songs (lyrics text and audio files) are stored in **Firebase** (Cloud Firestore and Cloud Storage), keyed to your anonymous ID, so they remain available in your Library.
- A copy of your Library is also cached locally on your device.
- Draft songs that are never converted into audio are automatically deleted after approximately 7 days.
- Songs you convert into audio are retained so they stay in your Library until deletion is requested or occurs through routine maintenance.
- You may request deletion of your data at any time by emailing us at [support@nextline.software](mailto:support@nextline.software).

## AI Processing Providers

To generate your song, your inputs and generated lyrics are sent over an encrypted connection to AI providers that perform the generation on their servers:

- **OpenRouter** (routing to a large language model) — used to write personalized lyrics from your prompt.
- **ElevenLabs** and/or **Mureka** — used to generate the sung audio from your lyrics, title, genre, language, and mood.

These providers process your inputs solely to deliver the requested generation output.

## Third-Party Services

The Application relies on the following third-party services, each governed by its own privacy policy:

- [Google Analytics for Firebase](https://firebase.google.com/support/privacy)
- [Firebase Crashlytics](https://firebase.google.com/support/privacy)
- [Firebase Authentication, Cloud Firestore, Cloud Functions, and Cloud Storage](https://firebase.google.com/support/privacy)
- [Amplitude](https://amplitude.com/privacy)
- [RevenueCat](https://www.revenuecat.com/privacy)
- [OpenRouter](https://openrouter.ai/privacy)
- [ElevenLabs](https://elevenlabs.io/privacy)
- [Mureka](https://www.mureka.ai/)

## App Tracking Transparency (iOS)

On iOS, the Application asks for your permission through Apple's App Tracking Transparency framework before using your device's advertising identifier for attribution (measuring which campaigns introduce new users to AI Song Maker). If you decline, we do not use tracking for that purpose. **We never sell your personal data.**

## Notifications

The Application may send you local notifications from your device (for example, reminders or updates about your song). These are scheduled on your device and do not require us to collect additional personal information.

## How We Use Information

We use the information described above to:

- Generate your lyrics and sung audio and display them in your Library
- Operate, maintain, and secure the Application, including enforcing fair-use limits
- Process subscriptions and purchases
- Measure performance, diagnose crashes, and improve the Application
- Measure marketing attribution (subject to your tracking choice on iOS)

## Data Sharing

We share information only with the third-party service providers listed above so they can perform services on our behalf, and only as needed to operate the Application. We do **not** sell your personal data, and we do **not** share it for third-party advertising.

## Security

We use industry-standard measures, including encryption in transit, to protect your information. However, no method of transmission or storage is completely secure, and we cannot guarantee absolute security.

## Children's Privacy

The Application is not intended for children under the age of 13, and we do not knowingly collect personal information from children under 13. If you believe a child has provided us with information, please contact us at [support@nextline.software](mailto:support@nextline.software) and we will delete it.

## Your Choices

- You can stop all further data collection by uninstalling the Application.
- You can request deletion of your stored songs and associated data by emailing [support@nextline.software](mailto:support@nextline.software).
- On iOS, you can change tracking permission at any time in your device settings.

## Changes to This Privacy Policy

We may update this Privacy Policy from time to time. The latest version will be posted at this location, and continued use of the Application after changes take effect constitutes acceptance of the updated policy.

## Contact Us

If you have any questions about this Privacy Policy, please contact us at [support@nextline.software](mailto:support@nextline.software).

# Privacy Policy

This Privacy Policy applies to the **Shared Calendar for Couples** mobile application (the "Application") created by **NEXTLINE YAZILIM LİMİTED ŞİRKETİ** ("Service Provider", "we", or "us"). The Application is offered as a Commercial service and is intended for use **"AS IS."**

By using the Application, you consent to our collection, use, and disclosure of information as described in this policy. This Privacy Policy may be updated from time to time, and we encourage you to review it periodically. Your continued use of the Application constitutes acceptance of any modifications to this policy.

---

## 1. Information Collection and Use

### 1.1 Automatically Collected Information
When you download and use the Application, certain data may be automatically collected, such as:
- **Device operating system and version**
- **Device model and language**
- **Application version**
- **Crash diagnostics and stack traces**
- **Usage events** (screens visited, features used, dates and times of activity)
- **Anonymous installation and analytics identifiers** assigned by our analytics and crash-reporting SDKs

The Application does **not** request access to the device's advertising identifier (IDFA on iOS) and does not display Apple's App Tracking Transparency prompt. We do not track you across other companies' apps or websites.

We use this automatically collected information for analytics, crash diagnostics, troubleshooting, and to improve the functionality of the Application.

### 1.2 Information You Provide During Sign-In
The Application requires you to sign in after the onboarding flow using **Google Sign-In** or **Sign in with Apple**. The following profile information is received from these providers and stored in our backend so the Application can function:
- **Email address**
- **Display name**
- **Profile photo URL** (if provided by the sign-in provider)
- **A unique user identifier** assigned by Firebase Authentication

### 1.3 Information You Provide Inside the Application
To deliver shared planning features, the Application stores information you enter, including:
- **Onboarding preferences** (date types you enjoy, your biggest relationship-planning challenge, your first name)
- **Partner-related profile fields** (such as the name you call your partner, relationship start date, time zone)
- **City and country** associated with your account. When you first sign in, the Application seeds a default city based on your device's **language and region settings** (for example, `en_US` seeds "New York"). This is **not** derived from GPS or any device-location service. You can edit or remove the city at any time in Settings.
- **Notification preferences**
- **Date and event details you create**: title, description, start time, end time, location, notes, checklist items, status, and post-date ratings or feedback
- **Photos you add to dates.** If you allow the Application to access your camera or photo library, photos you attach to a date are uploaded to our cloud storage and become visible to your connected partner.
- **Chat messages you send to Juno**, the Application's AI planning assistant. Your messages and Juno's responses are stored in our database under your account so your chat history persists across devices.
- **Partner invitation codes** that you generate or enter to connect with your partner

### 1.4 Subscription Information
When you start a free trial or purchase a subscription, **RevenueCat** processes your purchase and shares with us your subscription status, entitlement, and a RevenueCat user identifier. We do **not** receive your payment card or App Store / Play Store account credentials — these are handled exclusively by Apple or Google.

### 1.5 Camera and Photo Library
The Application can access your **camera** and **photo library** so you can attach photos to the dates you create. Access is requested only when you tap the add-photo button on a date; if you decline, the rest of the Application continues to work — you just cannot attach photos. Photos you select are uploaded to our cloud storage (see §5) and are visible to your connected partner. You can delete a photo from a date at any time.

### 1.6 Information We Do NOT Collect
- We do **not** access your microphone, contacts, calendars outside the Application, or other personal files on your device.
- We do **not** collect precise or approximate **location data from GPS or any device-location service**. The city and country on your profile are derived from your device's language and region settings (not a location lookup) and are editable in Settings.
- The Application does **not** send remote push notifications. Reminders are scheduled locally on your device.

---

## 2. Partner Sharing

The Application is designed for two connected partners to plan together. When you connect with a partner using a 6-digit invitation code, the following information becomes visible to that partner inside the Application:
- Date and event details you create or edit in the shared calendar (title, description, time, location, notes, checklist items, status, ratings)
- **Photos you attach to dates**
- Your display name and profile photo as provided by your sign-in provider
- Couple-level statistics (such as total dates planned and last date planned)

Your chat conversations with Juno (the AI assistant) are **private to you** and are **not** shared with your partner.

You may disconnect from a partner at any time through Settings. Disconnecting removes shared access going forward but does not retroactively delete events that were already created in the shared calendar.

---

## 3. AI Features (Juno chat and date suggestions)

The Application includes two AI-powered features provided through a Cloud Function we operate, which forwards requests to **OpenRouter**, a third-party AI inference service. OpenRouter routes the request to a large language model that generates a response.

### 3.1 Date suggestions
When you request a new batch of date ideas, we send your saved date-type preferences and an optional free-text request. Generated suggestions are stored in our database under your account so you can revisit them.

### 3.2 Juno chat
When you send a message to Juno, we send:
- Up to the last 15 messages of your recent chat history with Juno
- A compact **profile context**: your first name, your partner's name (if set), city and country, your selected date preferences, your chosen relationship-planning challenge, the number of dates you have completed, and a short reference to your most recent date (title and how many days ago it happened). This context lets Juno respond with relevant, personalized suggestions.

### 3.3 What we do NOT send to OpenRouter
- Your email address
- Your Firebase Authentication user ID
- Your RevenueCat or payment identifiers
- Your partner's email or account identifiers
- Any photos or event attachments

### 3.4 Retention of AI data
Chat messages and suggestions are stored in our database under your account for as long as your account exists. Deleting your account also deletes your chat history.

---

## 4. How We Use Your Information

We use the information described above to:
- **Provide core functionality**: authenticate you, sync the shared calendar between connected partners, deliver and store AI-generated date suggestions, and remember your preferences.
- **Improve the Application**: analyze aggregated usage patterns, fix bugs, and prioritize new features.
- **Manage subscriptions**: verify and refresh your subscription entitlement through RevenueCat.
- **Schedule local reminders**: trigger device-local notifications that you have opted into.
- **Diagnose crashes**: receive crash reports through Firebase Crashlytics.

---

## 5. Data Storage and Security

- Account, calendar, partner, chat, and suggestion data are stored in **Google Firebase (Cloud Firestore)** with encryption at rest and in transit.
- **Photos** you attach to dates are stored in **Google Firebase (Cloud Storage)** with encryption at rest and in transit. Each couple's photos live in an isolated storage path readable and writable only by the two connected partners.
- Partner pairing relies on per-couple access rules enforced by Firestore Security Rules so that only the two connected partners can read or write their shared events.
- App preferences and cached data are stored locally on your device using **Hive**.
- All network transmissions to our backend and third-party services use secure HTTPS connections.

We take reasonable physical, electronic, and procedural safeguards to protect information under our control from unauthorized access or disclosure. No method of transmission or storage, however, is completely secure.

---

## 6. Third-Party Access

### 6.1 Third-Party Services
The Application uses third-party services that have their own Privacy Policies governing how they handle data. Below are the providers we use and links to their policies:

- [Firebase Authentication, Cloud Firestore, Cloud Storage, Cloud Functions, and Crashlytics (Google)](https://firebase.google.com/support/privacy)
- [Google Analytics for Firebase](https://firebase.google.com/support/privacy)
- [Google Sign-In](https://policies.google.com/privacy)
- [Sign in with Apple](https://www.apple.com/legal/privacy/)
- [Amplitude](https://amplitude.com/privacy)
- [RevenueCat](https://www.revenuecat.com/privacy)
- [OpenRouter](https://openrouter.ai/privacy) (used for Juno chat and AI-generated date suggestions)

### 6.2 Data Disclosure
We may disclose information described in this policy:
- As required by law, such as to comply with a subpoena or similar legal process
- When we believe in good faith that disclosure is necessary to protect our rights, your safety or the safety of others, investigate fraud, or respond to a government request
- To trusted service providers who act on our behalf and have agreed to adhere to the practices set forth in this Privacy Policy

We do **not** sell your personal information.

---

## 7. Your Rights and Choices

You have the right to:
- **Access** the information stored in your account through the Application's Settings screen.
- **Delete** your account and associated personal data (including chat history and uploaded photos) using the **"Delete Account"** option in Settings. This action is permanent and cannot be undone.
- **Delete** individual photos from a date at any time from the date's details screen.
- **Disconnect** from your partner at any time through Settings.
- **Revoke camera or photo-library access** at any time through your device's Privacy settings. Existing photos already uploaded remain attached to their dates until you delete them.
- **Control** which local notifications you receive through your device's notification settings and the Application's notification preferences.
- **Stop all collection** by uninstalling the Application from your device.

If you would like assistance exercising any of these rights, contact us at the email address below.

---

## 8. Data Retention

- Account, profile, and shared calendar data are retained while your account remains active.
- When you delete your account through Settings, your personal data is removed from our active systems within a reasonable timeframe, generally not exceeding 30 days, except where retention is required for legal, accounting, or fraud-prevention purposes.
- Anonymized analytics and crash diagnostics data may be retained by our analytics providers in accordance with their own retention practices.

---

## 9. Children's Privacy

The Application is intended for adults in serious relationships and is not directed to children under 13. We do not knowingly collect personally identifiable information from children under 13. If you believe a child has provided us with personal information, please contact us at the address below and we will take appropriate action.

---

## 10. Changes to This Privacy Policy

This Privacy Policy may be updated from time to time. We will notify you of changes by updating this page and the "Last Updated" date below. Your continued use of the Application after changes are posted constitutes acceptance of the updated policy.

---

## 11. Your Consent

By using the Application, you consent to the processing of your information as described in this Privacy Policy, now and as amended by us.

---

## 12. Contact Us

If you have any questions about this Privacy Policy or our privacy practices, please contact us:

- **Email**: [support@nextline.software](mailto:support@nextline.software)

**Last Updated**: *April 23, 2026*

---

*This privacy policy was generated by [App Privacy MD Generator](https://github.com/nextline-yazilim/app-privacy-md-generator)*

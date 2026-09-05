# Privacy Policy

This Privacy Policy applies to the **BodyBird** mobile application (the "Application") created by **NEXTLINE YAZILIM LİMİTED ŞİRKETİ**, also known as Nextline Software ("Service Provider", "we", or "us"). The Application is offered as a Commercial service and is intended for use **"AS IS."**

By using the Application, you consent to the collection, use, and disclosure of information as described in this policy. This Privacy Policy may be updated from time to time. Your continued use of the Application constitutes acceptance of any changes.

---

## 1. What BodyBird Is

BodyBird is a camera game. You prop your phone on the floor, get into pushup position, and move up and down. The front camera watches your face, and the bird on screen follows your movement. Every run ends in a score. You can send that score to a friend as a challenge card.

There are no accounts. You do not sign up, log in, or give us an email address to play.

---

## 2. Camera Data

The Application uses your device's front camera to detect where your face is on screen. This is how the bird moves.

- **All camera processing happens on your device.** The Application uses Google ML Kit face detection, which runs locally on the phone.
- The Application does **not** record, save, or upload any photos, videos, or camera frames.
- Camera frames are never included in challenge cards, share images, or anything sent to our servers.
- The Application does not identify you. It only tracks the position and size of a face box to move the bird. It does not create or store a face template or any biometric identifier.
- The camera is only active on the play screen. It turns off when you leave that screen.

If you record your own screen while playing, that recording is created by your device and belongs to you. The Application does not capture it.

Camera permission can be changed at any time in your device settings. Without camera access the game cannot be played.

---

## 3. Information Collection and Use

### 3.1 Automatically Collected Information
When you use the Application, certain data may be collected automatically by the Application and its third-party SDKs, such as:
- **Device type, operating system, and version**
- **App version and language**
- **IP address** (received by third-party services when the Application connects to them; it may be used to derive an approximate region)
- **Screens visited and in-app events**, such as onboarding completed, run completed (with score, rep count, whether a continue was used, and run duration), new personal best, challenge created, shared, received, or attempted, rewarded ad watched, interstitial shown, purchase made, restore completed, skin equipped or unlocked, and whether camera or notification permission was granted
- **Session data** (when the Application was opened and closed)
- **Crash and performance data**

We use this information for analytics, troubleshooting, and to improve the Application.

### 3.2 Automatically Collected Identifiers
The Application and its SDKs generate pseudonymous identifiers. These are not provided by you and do not identify you by name:
- **Firebase anonymous user ID.** A random ID is created by Firebase Authentication the first time the Application runs. It is the key under which your scores, diamonds, skins, and challenges are stored. It is also used as your user ID in Amplitude and RevenueCat so those records can be matched. If Firebase is unavailable, a random ID is generated on the device instead.
- **Analytics identifiers** (Amplitude device ID, Firebase installation ID)
- **Crash reporting identifiers** (Firebase Crashlytics installation ID)
- **Purchase identifiers** (RevenueCat app user ID and App Store transaction identifiers)
- **Push notification token** (Firebase Cloud Messaging token, created only if you allow notifications)
- **Apple Search Ads attribution token.** The RevenueCat SDK may collect an anonymized AdServices token to measure whether the install came from an Apple Search Ads campaign. It does not identify you and does not involve cross-app tracking.

The Application does **not** ask for permission to track you across other apps and websites. It does not show the App Tracking Transparency prompt, and it does not use the advertising identifier (IDFA) for ad personalization.

### 3.3 Information You Provide
The Application asks for very little from you:
- **Challenge card name.** When you send a challenge, you can type a name (up to 20 characters) to show on the card. This is optional. If you leave it empty the card says "A FRIEND". The name you enter is saved on your device and in your user record on our servers, and it is included in the challenge record so the recipient can see who sent it.
- **Support messages.** If you email us, we receive your email address and whatever you write.

---

## 4. Game Data Stored on Our Servers

The Application uses Firebase (Google Cloud) to store game data so that challenges work and the global counter can be shared by everyone. All writes that matter go through our Cloud Functions. Data stored under your anonymous ID:
- **Your user record:** personal best score, total reps, diamond balance, owned and equipped skins, your challenge card name (if set), your push token (if you allowed notifications), and daily counters used for rate limiting and abuse prevention (runs per day, challenges created per day, rewarded ad diamonds per day).
- **Challenge records** you create: your anonymous ID, the name you chose, the score to beat, the bird skin shown on the card, creation and expiry dates, and, once someone plays it, the best attempt (their name if they set one, or "A friend", and their score).
- **Global counter:** the total number of reps counted by all players. Only the number is stored. It cannot be traced back to an individual.
- **Purchase credits:** when you buy a diamond pack, the product identifier and App Store transaction identifier are sent to our Cloud Functions so the diamonds can be credited once.
- **Short-lived request keys** that prevent the same run or purchase from being counted twice. These are kept for 48 hours.

Challenge records expire 30 days after they are created and are deleted by a scheduled cleanup.

Scores that are not plausible (for example above server limits) may be rejected or capped. This is an anti-abuse measure and does not use any personal data beyond your anonymous ID.

---

## 5. Challenge Cards and Sharing

- Sharing always goes through your device's system share sheet. You choose where the card goes.
- A challenge card contains: the score to beat, the name you typed (or "A FRIEND"), the bird skin you have equipped, and a link such as `bodybird.app/c/{id}`.
- Anyone who has the link can open the challenge and see the name, score, and skin on it. Treat the link like a public message.
- When someone plays your challenge, you can see their result in the Application: their card name (if they set one, otherwise "A friend") and their score.
- A run share card from the score screen contains your score, the mascot, and the app name. It never contains camera imagery.

---

## 6. Notifications

The Application can send **push notifications** to tell you when a friend takes your challenge. These are delivered through Firebase Cloud Messaging.

- The Application asks for notification permission only once, after you share your first challenge, and only if you tap "NOTIFY ME".
- If you allow notifications, a push token is stored in your user record so our Cloud Functions can send the result. The notification text contains the other player's card name (or "A friend") and the score.
- You can turn notifications off at any time in your device settings.

The Application does not schedule reminder or marketing notifications.

---

## 7. Advertising

The Application shows ads through Google AdMob:
- **Rewarded ads**, which you choose to watch to continue a run or earn diamonds.
- **Interstitial ads**, which may appear when you tap Play Again after the first session, at most about once every three runs.

All ad requests are made as **non-personalized ads**. The Application does not ask for tracking permission and does not provide an advertising identifier for personalization. Google may still receive device information, your IP address, and an approximate region from the IP address to serve ads, cap frequency, and prevent fraud. See Google's advertising policy linked in Section 11.

Buying **Remove Ads** removes interstitial ads permanently. Rewarded ads remain available because you choose when to watch them.

---

## 8. Purchases

The Application offers one-time in-app purchases: Remove Ads, diamond packs, and hero bird skins. There are **no subscriptions**.

Purchases are processed by Apple through the App Store, with the RevenueCat SDK managing entitlements. We do not receive or store your payment card details. We receive product and transaction identifiers so we can grant what you bought.

---

## 9. Locally Stored Data

The Application stores data on your device using local storage (Hive), including:
- Personal best, total reps, diamond balance, owned and equipped skins, and your card name
- Runs waiting to be sent to the server when you are offline
- A cache of challenges you sent and received
- Preferences and flags (onboarding done, haptics, language, session count, ad cadence counters)
- A cached copy of the global counter

This data stays on your device until you uninstall the Application. It is used to open the game instantly and to keep playing offline.

---

## 10. Location Data

The Application does **not** collect the location of your device. Third-party services may derive an approximate region from your IP address as described above.

---

## 11. Third-Party Services

The Application uses third-party services that have their own privacy policies:

- [Firebase](https://firebase.google.com/support/privacy) (Authentication, Firestore, Cloud Functions, Cloud Messaging, Crashlytics, Google Analytics for Firebase)
- [Google ML Kit](https://developers.google.com/ml-kit/terms) (on-device face detection; images never leave the device)
- [Google AdMob](https://policies.google.com/technologies/ads)
- [Amplitude](https://amplitude.com/privacy)
- [RevenueCat](https://www.revenuecat.com/privacy)
- [Apple App Store](https://www.apple.com/legal/privacy/)

The Application also downloads its two display fonts (Anton and Manrope) from Google Fonts the first time they are needed. This is a standard web request that includes your IP address. See [Google's privacy policy](https://policies.google.com/privacy).

---

## 12. Data Disclosure

We may disclose automatically collected information and game data:
- As required by law, such as to comply with a subpoena or similar legal process
- When we believe in good faith that disclosure is necessary to protect our rights, your safety or the safety of others, investigate fraud, or respond to a government request
- To trusted service providers who work on our behalf and agree to follow the rules in this Privacy Policy

We do not sell your information.

---

## 13. Your Choices and Rights

- **Camera:** grant or revoke camera access in your device settings.
- **Notifications:** turn push notifications on or off in your device settings.
- **Ads:** rewarded ads are optional. Interstitial ads can be removed with the Remove Ads purchase.
- **Uninstall:** uninstalling the Application stops all collection and deletes all locally stored data.
- **Deletion of server data:** because there are no accounts, your server data is tied to an anonymous ID that we cannot link to you by name. If you want it deleted, email us. Including a challenge link you created helps us find the record. Once the Application is uninstalled, a new install creates a new anonymous ID and the old data is not reachable from the new install.

If you are in the European Economic Area, the United Kingdom, Türkiye, or another region with data protection laws, you may have rights to access, correct, delete, or restrict the processing of your data. Contact us using the details in Section 18. Our legal basis for processing is our legitimate interest in running, securing, and improving the game, your consent where the law requires it (for example notifications), and the performance of a purchase you make.

---

## 14. Data Retention

- **Locally stored data** stays on your device until you uninstall the Application.
- **Challenge records** are deleted 30 days after creation.
- **Request keys** used to prevent double counting are deleted after 48 hours.
- **User records** (scores, diamonds, skins, card name, push token) are kept while they are needed to run the game. You can request deletion as described in Section 13.
- **Third-party data** (analytics, crash reports, ad logs, purchase records) is retained according to each provider's own policy.

---

## 15. Children

The Application is a general audience game. It is not directed at children under the age of 13, and we do not knowingly collect personal information from children under 13. There is no age gate, but the Application does not ask for a name, email, or any personal details to play, and all ads are served as non-personalized. If you believe a child has provided us with personal information, contact us so we can delete it.

---

## 16. Security

We take reasonable measures to protect information under our control. Server data is protected by Firebase security rules so that only you can read your own user record and only our Cloud Functions can write scores, diamonds, and challenges. Transmissions to our servers and to third-party services are encrypted (HTTPS). Locally stored data is protected by your device's built-in security.

---

## 17. Changes to This Privacy Policy

This Privacy Policy may be updated from time to time. We will post the new version on this page and update the "Last Updated" date. Continued use of the Application after changes are posted constitutes your acceptance of those changes.

---

## 18. Contact Us

If you have any questions about privacy while using the Application, contact us by email:

- **Email**: [support@nextline.software](mailto:support@nextline.software)

**Last Updated**: *September 5, 2026*

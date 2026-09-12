# Privacy Policy

This Privacy Policy applies to the **Speedometer: GPS Speed & HUD** mobile application (the "Application") created by **NEXTLINE YAZILIM LİMİTED ŞİRKETİ**, also known as Nextline Software ("Service Provider", "we", or "us"). The Application is offered as a Commercial service and is intended for use **"AS IS."**

By using the Application, you consent to the collection, use, and disclosure of information as described in this policy. This Privacy Policy may be updated from time to time. Your continued use of the Application constitutes acceptance of any changes.

---

## 1. What the Application Is

Speedometer is a GPS speedometer for iPhone and iPad. It shows your current speed from GPS in a large readout, with a HUD mirror mode for the windshield, vehicle modes, an optional speed alert, optional trip recording with a local history, and a Live Activity on the Lock Screen and in the Dynamic Island while a trip is being recorded.

The Application works on your device. **There are no accounts, no sign-up, and no server run by us.** Your speed, your location, and your trips are never sent to us.

---

## 2. Location Data

Location is the core of the Application. Without it there is no speed to show.

- **Permission.** The Application asks for location access **"While Using the App"**. It does not ask for "Always" access.
- **Precise Location.** Speed cannot be measured from an approximate position, so the Application asks for Precise Location. If Precise Location is off, the Application shows a screen explaining why it is needed and may ask iOS for temporary full accuracy for the current session.
- **What is read.** The Application reads position, speed, speed accuracy, horizontal accuracy, altitude, and course from the GPS. It also reads the compass heading and the accelerometer to show the heading and to tell whether the phone is moving when the GPS signal is weak.
- **Everything is processed on your device.** Speed is calculated on the phone. Location data is never uploaded, never sent to us, and never shared with any third party. It is not used for advertising.
- **Background location.** Location updates continue in the background **only while you are recording a trip** (a premium feature). This keeps the trip and the Live Activity updating when the screen is locked or another app is in front. iOS shows its blue location indicator during this time. When you stop the trip, background location updates stop. When you are not recording a trip, the Application does not use your location in the background.
- **What is stored.** When you record a trip, a simplified route outline (up to 600 points of latitude, longitude, speed, and time offset) is saved on your device together with the trip summary. See Section 7. Nothing else about your location is kept.

You can change location permission at any time in Settings > Speedometer > Location. Without location access the Application cannot measure speed.

---

## 3. Information Collection and Use

### 3.1 Automatically Collected Information
The Application does not have its own analytics or a server. The only third-party service the Application connects to is RevenueCat, which handles purchases and subscription status. When the Application connects to RevenueCat and to the Apple App Store, those services may receive:
- **Device type, operating system, and version**
- **App version and language**
- **IP address** (received by the service when the Application connects to it; it may be used to derive an approximate region)
- **Purchase and subscription status** (which plan you bought, trial status, renewal and expiry dates)

This information is used to load prices, process purchases, and keep your premium access in sync with the App Store.

### 3.2 Automatically Collected Identifiers
The Application and its SDKs generate pseudonymous identifiers. These are not provided by you and do not identify you by name:
- **RevenueCat anonymous app user ID.** A random ID created by the RevenueCat SDK on first launch. It is used to keep track of your premium entitlement.
- **App Store transaction identifiers** for purchases and subscriptions.
- **Apple Search Ads attribution token.** The RevenueCat SDK may collect an anonymized AdServices token to measure whether the install came from an Apple Search Ads campaign. It does not identify you and does not involve cross-app tracking.
- **A random installation ID** may be generated and stored on the device for internal use. It stays on the device.

The Application does **not** ask for permission to track you across other apps and websites. It does not show the App Tracking Transparency prompt, it does not use the advertising identifier (IDFA), and it shows no ads.

### 3.3 Analytics and Crash Reporting
This version of the Application does **not** send usage analytics or crash reports to any service. The Application contains analytics and crash reporting libraries (Amplitude and Firebase Crashlytics) as part of its build, but they are not configured in this version and do not run. If a future version enables them, this policy will be updated first.

### 3.4 Information You Provide
The Application does not ask you to enter any personal information. If you email us, or use the "Not really" feedback option after the accuracy question (which opens your own mail app with a message addressed to us), we receive your email address and whatever you write.

---

## 4. Purchases and the Free Readout

The Application is free to download. The live speed readout is free for a total of 30 seconds across all sessions. After that, continuing requires a premium plan. HUD mode, trip recording, the speed alert, the Live Activity, and dial styles are premium features from the start.

- **Plans.** A weekly subscription, a yearly subscription with a 3-day free trial, and a one-time lifetime purchase. Prices are shown in the Application in your local currency.
- **Processing.** Purchases are processed by Apple through the App Store. The RevenueCat SDK manages the entitlement. **We do not receive or store your payment card details.** We receive product and transaction identifiers so premium can be granted and restored.
- **The free counter.** The number of free seconds you have used (0 to 30) is stored on your device in the Application's local storage and also in the iOS Keychain. The Keychain copy is not synced to iCloud and does not leave the device. It can remain on the device after the Application is uninstalled, so reinstalling does not reset the free seconds. This value contains no personal information.

---

## 5. Notifications

The Application can schedule **one local notification**: a reminder on the second day of the yearly free trial that the trial is about to end and can be cancelled in Settings.

- The Application asks for notification permission only when you start the free trial, on the screen that offers the reminder. You can decline.
- The notification is scheduled on your device by the Application. There is no push notification service, and no notification token is created or sent anywhere.
- The reminder is cancelled automatically when your subscription status changes.
- The Application does not send marketing notifications.

You can turn notifications off at any time in Settings > Speedometer > Notifications.

---

## 6. Live Activity

While you record a trip, the Application can show a Live Activity on the Lock Screen and in the Dynamic Island with your current speed, distance, and elapsed time. It is updated by the Application on the device. No push updates are used, and no data is sent anywhere. The Stop button in the Live Activity opens the Application to end the trip. Live Activities require iOS 16.1 or later and can be turned off in Settings > Speedometer > Live Activities.

---

## 7. Locally Stored Data

The Application stores data on your device using local storage (Hive) and the iOS Keychain:
- **Trips** (premium): a unique trip ID, start and end times, vehicle mode, unit, distance, maximum speed, average speed, duration, moving time, and the simplified route outline described in Section 2.
- **Preferences:** speed unit, vehicle mode, dial style, appearance, keep-screen-awake, auto-dim, HUD brightness boost, speed alert threshold, alert feedback and sound.
- **Flags and counters:** onboarding completed, explainer shown, soft paywall shown, rating prompt count and date, last paywall time, trial reminder ID, free seconds used (also mirrored to the Keychain, see Section 4).
- **A cached copy of your premium status** kept by the RevenueCat SDK so premium works offline.

This data stays on your device. We cannot see it. You can delete any trip from the trip list (swipe) or from the trip summary screen. Uninstalling the Application deletes all locally stored data except the Keychain free-seconds counter described in Section 4.

---

## 8. Third-Party Services

The Application uses the following third-party services, which have their own privacy policies:

- [RevenueCat](https://www.revenuecat.com/privacy) (purchases and subscription status)
- [Apple App Store](https://www.apple.com/legal/privacy/) (payments, subscription management, the in-app rating prompt, and Apple Search Ads attribution)

The Application also contains links that open in your browser or in the App Store app: this Privacy Policy, the Terms, and the "Manage subscription" page. Opening a link is a normal web request to that site. The Application does not load web content, fonts, or images from the internet on its own.

---

## 9. Data Disclosure

We hold almost no data about you. The purchase records held by RevenueCat and Apple are the only data linked to your use of the Application that exist outside your device. We may disclose such information:
- As required by law, such as to comply with a subpoena or similar legal process
- When we believe in good faith that disclosure is necessary to protect our rights, your safety or the safety of others, investigate fraud, or respond to a government request
- To trusted service providers who work on our behalf and agree to follow the rules in this Privacy Policy

We do not sell your information.

---

## 10. Your Choices and Rights

- **Location:** grant, limit, or revoke location access and Precise Location in Settings > Speedometer > Location.
- **Background location:** only used while a trip is recording. Stop the trip to end it.
- **Notifications:** turn the trial reminder off in Settings > Speedometer > Notifications.
- **Live Activities:** turn them off in Settings > Speedometer > Live Activities.
- **Trips:** delete any trip inside the Application.
- **Subscriptions:** manage or cancel in your App Store account settings. Use Restore Purchases in the Application's Settings to bring premium to a new device.
- **Uninstall:** uninstalling the Application stops all processing and deletes the locally stored data described in Section 7 (except the Keychain counter, which contains no personal information).

If you are in the European Economic Area, the United Kingdom, Türkiye, or another region with data protection laws, you may have rights to access, correct, delete, or restrict the processing of your data. Because we do not run a server or hold your data, requests about purchase records are handled together with RevenueCat and Apple. Contact us using the details in Section 15. Our legal basis for processing is the performance of a purchase you make, our legitimate interest in running and securing the Application, and your consent where the law requires it (for example location and notifications).

---

## 11. Data Retention

- **Locally stored data** stays on your device until you delete it in the Application or uninstall the Application.
- **The Keychain free-seconds counter** may remain on the device after uninstall. It contains a number between 0 and 30 and nothing else.
- **Purchase and subscription records** are retained by RevenueCat and Apple according to their own policies.

---

## 12. Children

The Application is a general audience utility. It is not directed at children under the age of 13, and we do not knowingly collect personal information from children under 13. The Application does not ask for a name, email, or any personal details. If you believe a child has provided us with personal information, contact us so we can delete it.

---

## 13. Security

We take reasonable measures to protect information under our control. Communication with RevenueCat and the App Store is encrypted (HTTPS). Locally stored data is protected by your device's built-in security, and the free-seconds counter is stored in the iOS Keychain.

---

## 14. Changes to This Privacy Policy

This Privacy Policy may be updated from time to time. We will post the new version on this page and update the "Last Updated" date. Continued use of the Application after changes are posted constitutes your acceptance of those changes.

---

## 15. Contact Us

If you have any questions about privacy while using the Application, contact us by email:

- **Email**: [support@nextline.software](mailto:support@nextline.software)

**Last Updated**: *September 12, 2026*

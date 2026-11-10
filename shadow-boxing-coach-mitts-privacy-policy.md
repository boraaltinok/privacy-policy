# Privacy Policy

_Last updated: 2026-11-10_

Thank you for using **Mitts** (App Store name: "Shadow Boxing Coach: Mitts", the "Application"). This Privacy Policy explains how NEXTLINE YAZILIM LİMİTED ŞİRKETİ ("Service Provider", "we", or "us") handles information when you use the Application.

The Application is an audio-first shadow-boxing coach for training at home. A coach voice calls combos, defense, and footwork while pad sounds mark the tempo, and a board on screen shows the current combo. It also includes a free round timer, move sheets, a boxing cheat sheet, short programs, and reminders. **No account. Your workouts stay on your phone.** We do not run a server that stores your training data, and we never receive your round history or your custom workouts. The only information that leaves your phone is described below: optional usage events and crash reports (Firebase), and purchase records (RevenueCat).

## 1. Information We Handle

### Stored Locally on Your Device

Everything you enter or create while training is saved only in the Application's local storage (a local database) on your iPhone. These records are never uploaded; we never receive, see, or store them. (If **Share usage data** is on, a few of these values, namely your training goal, speed and difficulty level, coach language, and voice mode, can be attached to individual usage events as described under Usage Analytics below.) This includes:

- **Your training profile**: the answers you give during setup (your goal, how familiar you are with boxing, your stance, and your preferred session length), your voice mode (move names or numbers), coach language, and default speed and difficulty.
- **Round history**: for each round, the date and time, the type of round (coached or timer), the focus card or program day, the moves and combos it taught, the planned and actual duration, and whether it was completed or ended early.
- **Programs and custom workouts**: your progress through programs and any workouts you build yourself, including the name you give them.
- **Reminders and settings**: reminder days and time, sound and music mix, pad sounds, vibration, appearance, and your privacy choices (see Section 8).

This information lives only on your device. Deleting the Application deletes it. If you use iCloud Backup or back up your iPhone to a computer, this local data may be included in that device backup according to your Apple settings; that backup is managed by Apple, not by us, and is not a sync to our servers. There is no sync between devices. Restoring a purchase brings back your subscription, not your round history.

**Free-round counter.** The Application keeps a count of how many of your free coached rounds you have used (a number from 0 to 3) in the iOS Keychain on this device. It contains no personal information, is not synced to iCloud or other devices, and is never sent to us. iOS may keep Keychain items after the Application is deleted, so reinstalling the Application may not reset this count.

### Usage Analytics (Share usage data)

The Application uses Google Analytics for Firebase to understand, in aggregate, how it is used. It is controlled by the **Share usage data** switch in **Settings › About**:

- **Default:** the switch starts **off** if your device's region is set to a country in the European Economic Area, the United Kingdom, or Switzerland (or if the region cannot be determined), and **on** elsewhere. You can turn it on or off at any time.
- **What is sent when it is on:** product events from a fixed allowlist built into the Application, for example: which onboarding step was viewed, that a coached round or timer session started or was completed, which focus card or program day was used, the speed and difficulty level, the coach language and voice mode, that a round was paused or ended early, that a move sheet or the cheat sheet was opened, which paywall was shown and the training goal it was shown for, the plan type selected, whether a purchase or restore succeeded, and whether you allowed reminders. A plan status (free, trial, or Mitts Coach) may be attached as a user property. Google Analytics may also record App Store in-app purchase events (such as the product, price, and currency) automatically.
- **What is never sent:** your boxing familiarity, your stance, your session length, your reminder days and times, the names of your custom workouts, or your round history as a whole. Events that are not on the allowlist are dropped.
- **Identifier:** Firebase uses a random app-instance identifier stored on your device to group these events. It is not your name or email, but it is a persistent identifier, so this data is pseudonymous, not anonymous.
- **Advertising features are off:** ad storage, ad personalization, and ad user-data signals are disabled, the advertising identifier (IDFA) and the vendor identifier (IDFV) are not collected, and automatic screen reporting is disabled. As with any network service, Google may derive an approximate location (such as country or region) from your IP address.

When the switch is off, no usage events are sent.

### Crash Reports (Send crash reports)

If the Application crashes or hits an error, Firebase Crashlytics can send a crash report containing the stack trace, device model, iOS version, Application version, a Crashlytics installation identifier, a few technical state labels (for example, the current screen, the round state, and the coach language), and the names of the last in-app actions before the crash (action names only, with no values and no training data). Crash reports follow the **Send crash reports** switch in **Settings › About**, with the same region default as usage analytics (off in the EEA, UK, and Switzerland until you turn it on; on elsewhere). While it is off, crash reports are not sent.

### Purchases

Purchases are processed by Apple through the App Store and managed by RevenueCat. RevenueCat assigns a random **App User ID** to your installation (the Application never links it to your name or email and never calls a login) and receives your purchase and subscription history, along with technical information such as device model, iOS version, Application version, and IP address (from which RevenueCat may derive your country). We never receive your payment-card details.

If **Share usage data** is on when the Application starts, RevenueCat may also collect an attribution token through Apple's AdServices framework to measure whether an Apple Search Ads campaign led to the install. This token is not the advertising identifier (IDFA) and does not track you across other companies' apps or websites.

### Information You Send Us

If you contact us by email, we receive your email address and whatever you write. If you include your **Support ID** (see Section 8), we can use it to find your purchase records held by RevenueCat.

### What We Do Not Collect

- Your name, email address (unless you email us), phone number, or any account details. The Application has no account or login.
- Your precise location, contacts, photo library, camera, or microphone. The Application does not ask for location, contacts, camera, or microphone permission. (Saving the optional cheat-sheet image to Photos is add-only; the Application cannot read your photos.)
- Apple Health or other health data. The Application does not read from or write to Apple Health, does not measure your heart rate, and does not count your punches. Your round history never leaves your phone.
- The advertising identifier (IDFA). The Application shows no ads, does not track you across other companies' apps or websites, and therefore does not display an App Tracking Transparency prompt.

## 2. Device Features and Permissions

- **Audio while locked**: coach calls, pad sounds, and round bells are generated and played on your device and keep playing with the screen locked. They mix with your own music. Nothing is recorded; the Application does not use the microphone.
- **Phone calls and other audio**: if a call or another app interrupts audio, iOS tells the Application that audio was interrupted so it can pause the round. The Application does not read or store any call information.
- **Notifications**: reminders are **local notifications** scheduled on your device by iOS (training-day reminders, a reminder two days before a free trial ends, and a reminder after a quiet week). They are not push notifications and involve no server. The Application asks for notification permission only after a purchase, once after a completed round, or when you turn on reminders in **Settings › Reminders**; never at launch.
- **Vibration**: optional taps on each pad sound ("Vibrate with pads") run on your device only.
- **Rating prompt**: the Application may show Apple's standard rating prompt. Apple handles any rating you leave.
- **Sharing**: you can export the boxing cheat sheet as an image through the iOS share sheet. Nothing is shared unless you choose a destination, and the image contains the cheat sheet, not your training data. If you pick **Save Image** in the share sheet, iOS asks once for permission to add the image to your Photos; the Application can only add that image and cannot see your photo library.
- **Links**: Terms, Privacy, and subscription management open in Safari or Apple's own screens, which are governed by their own privacy policies.

## 3. Voice and Content

All coach audio, pad sounds, moves, programs, and the cheat sheet are bundled with the Application and work offline. This version of the Application does not download voice packs or any other content. If a future version adds downloadable language packs, we will update this Privacy Policy before it does.

## 4. How We Use Information

We use the information described above only to:

- provide the training features on your device (coached rounds, timer, programs, custom workouts, reminders);
- process, validate, and restore purchases (Apple, RevenueCat);
- find and fix crashes, if crash reports are on (Firebase Crashlytics);
- understand, in aggregate, how the Application is used so we can improve it, if usage data is on (Google Analytics for Firebase);
- measure our own App Store advertising, if usage data is on (AdServices attribution token);
- answer your support requests.

We do not sell your information, we do not use it for advertising profiles, and we do not share it with data brokers. Your training data is never used by us for any purpose, because we never receive it.

## 5. Legal Bases (EEA, UK, and similar laws)

Where data-protection laws such as the GDPR apply, we rely on: your **consent** for usage analytics, crash reports, and the AdServices attribution token (in the EEA, UK, and Switzerland these start off and are enabled only if you switch them on; you can withdraw consent at any time in Settings › About); and **performance of a contract** for processing and restoring your purchases.

## 6. Third-Party Services

The Application uses the following third parties. Each processes data under its own privacy policy:

- [Google Firebase (Analytics, Crashlytics)](https://firebase.google.com/support/privacy)
- [RevenueCat](https://www.revenuecat.com/privacy)
- [Apple (App Store purchases, AdServices attribution)](https://www.apple.com/legal/privacy/)

The Application does not use any advertising network and does not send your training data to any third party.

## 7. Data Retention

- **Local data** stays on your device until you delete the Application (or restore your device without its backup). The free-round counter in the Keychain may remain after deletion, as described in Section 1.
- **Third-party data** (analytics events, crash reports, purchase records) is kept according to each provider's retention policy linked above. To request deletion, email us your Support ID (see Section 8).

## 8. Your Choices and Rights

- **Usage analytics**: turn **Share usage data** on or off in **Settings › About**.
- **Crash reports**: turn **Send crash reports** on or off in **Settings › About**.
- **Reminders**: turn them on or off and change their days and time in **Settings › Reminders**, or change notification permission in iOS Settings.
- **Local data**: delete the Application to remove your training profile, round history, programs, custom workouts, and settings from your device.
- **Access or deletion of provider records**: because there is no account, we cannot look you up by name. Tap **Support ID** in **Settings › About** to copy it (it is your RevenueCat App User ID) and email it to [support@nextline.software](mailto:support@nextline.software). We will ask RevenueCat to access or delete the purchase records linked to it, as far as RevenueCat allows. Usage analytics and crash reports are keyed to separate Firebase identifiers that are not part of the Support ID, so we cannot pick them out individually; they expire under Google's retention settings, and you can stop any further collection with the switches above. Purchase records that Apple and RevenueCat must keep for accounting or legal reasons may be retained.

Depending on where you live, you may also have the right to object to or restrict processing, to data portability, and to complain to your local data-protection authority.

## 9. Security

Your training data never leaves your device, so there is no server copy of it to be breached. Connections to Firebase and RevenueCat are encrypted (HTTPS). No security measure is perfect, and we cannot guarantee absolute security; please keep your device protected with a passcode.

## 10. Children's Privacy

The Application is a general fitness app and is not directed to children under 13. We do not knowingly collect information from children under 13 (or the applicable age in your country). If you believe a child has used the Application and data was sent to our providers, contact us at [support@nextline.software](mailto:support@nextline.software) with the Support ID and we will take appropriate action.

## 11. Not Medical Advice

The Application is a fitness app for boxing training at home. It does not give medical advice and does not measure your health. See the health and safety section of our Terms & Conditions.

## 12. Changes to This Privacy Policy

We may update this Privacy Policy from time to time. The latest version will be posted at the same URL with a new "Last updated" date. Continued use of the Application after changes means you accept the updated Privacy Policy.

## 13. Contact Us

NEXTLINE YAZILIM LİMİTED ŞİRKETİ
Email: [support@nextline.software](mailto:support@nextline.software)

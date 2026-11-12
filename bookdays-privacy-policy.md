# Privacy Policy

This Privacy Policy applies to the **Bookdays** mobile application for iPhone and iPad (the "Application"), created by **NEXTLINE YAZILIM LİMİTED ŞİRKETİ** ("Service Provider", "we", or "us"). The Application is a personal reading diary and is offered as a Commercial service on an **"AS IS"** basis.

By using the Application, you consent to the collection, use, and disclosure of information as described in this policy. We may update this Privacy Policy from time to time, and we encourage you to review it periodically. Your continued use of the Application after changes are posted constitutes acceptance of the updated policy.

**The short version:**
- There is **no account**. You never sign up, log in, or give us your name or email to use the Application.
- **Your diary stays with you.** Your books, thoughts, quotes, photos and reading-room history are stored on your device and in **your own private iCloud**, which we cannot access or read.
- **Voice notes are the one exception.** When you hold to talk, the recording is sent through our server to **OpenAI**, which writes it down. We do not keep the recording.
- We use pseudonymous usage analytics and crash reports (Google Firebase) that **never contain your diary content**.
- **No ads, no tracking, no sale of data.** The Application does not use the advertising identifier (IDFA) and does not ask for tracking permission.

---

## 1. Information Collection and Use

### 1.1 Automatically Collected Information
When you use the Application, certain technical information is collected automatically by the third-party services listed in Section 6:

- **App-instance and installation identifiers** (Firebase app instance ID, Firebase installation ID used by Crashlytics and Remote Config). These are random identifiers created by the SDKs, not information you provide.
- **Usage events**: which screens and features are used (for example "a book was added", "a thought was saved", "the paywall was shown"). Every event and parameter comes from a fixed allowlist inside the Application and contains only categories, yes/no values or rounded buckets. **Book titles, authors, ISBNs, your thoughts, quotes, voice-note text, search words, file names and covers are never sent to analytics.**
- **A few user properties (no name, email or diary content)**: your plan status (free, trial, subscribed, lifetime), the reading goal you picked in onboarding (from a fixed list), and whether iCloud backup is on.
- **Device and app information**: device model, operating system version, app version, language and country/region settings.
- **Approximate location**: country or region derived from your IP address by Firebase. The Application does **not** request or collect your precise location.
- **Crash and diagnostic data**: crash reports and error codes (Firebase Crashlytics). Error reports are sanitized inside the Application so that diary text, book titles and similar content are removed before anything is sent. Crash reports are not linked to a user ID set by us.

We use this information to understand how the Application is used, fix problems, and improve features.

### 1.2 Location Data
The Application does **not** access your device's location services. Only an approximate country/region is inferred from your IP address by our analytics provider, as described above.

### 1.3 Information You Provide
- **Voice notes** (only if you choose to use Hold to talk): see Section 2.
- **Book lookups**: when you scan a barcode or search for a book, the ISBN or the search words are sent to our server to find the book (see Section 3).
- **Support emails**: if you contact us, we receive your email address, your message, and the **Support ID** and app version that the Application adds to the email so we can help you (see Section 8).

We do **not** collect your name, email address, phone number, contacts, or payment card details. Payments are handled entirely by Apple.

### 1.4 Information Stored Only on Your Device and in Your Own iCloud
The following stays on your device and, if iCloud is turned on for the Application, in the **private CloudKit database of your own Apple ID** (Apple iCloud). We cannot read it:

- Your books, statuses, ratings, finish dates and shelf layout
- Your typed thoughts and saved quotes
- The text of your voice notes once written down, and the audio of voice notes that are still waiting to be written down
- Photos you take of a book cover ("Snap your copy"), photo frames and cut-out objects for your shelf
- Reading-room session lines (for example "42 min · Rainy window")
- Small usage counters for the free tier (number of books added, page-photo quotes and voice notes used), kept in the device Keychain and in iCloud key-value storage so they survive a reinstall

Device preferences (theme, sounds, reminder times, recent searches, an unsaved typed draft) are stored only on the device.

### 1.5 On-Device Processing
- **Barcode scanning**, **page text recognition** (turning a page photo into a quote) and **subject lift** (cutting an object out of a photo) run entirely on your device using Apple frameworks. **Page photos are read on the device and discarded immediately**; only the lines you choose to keep are saved.
- **Importing** a reading list from another app (Goodreads, StoryGraph, Bookmory or a CSV/ZIP file) is parsed on your device. Only ISBNs are then looked up, as described in Section 3.
- **Exporting** your diary (CSV, ZIP or Markdown) is created on your device and handed to the iOS share sheet; we never receive it.

---

## 2. Voice Notes (Hold to Talk)

Hold to talk is optional, and the Application asks for your permission before the first recording. Typing never depends on it.

- When you release the button, the recording (up to 3 minutes) is sent over an encrypted connection to our server (Google Cloud Functions for Firebase, United States). The server forwards it to **OpenAI** (speech-to-text API), which returns the written text. The server then returns the text to your device.
- **We do not keep the recording.** On our server the audio exists in memory only for the duration of that single request. It is never written to disk, to storage, or to logs.
- **OpenAI** processes the audio as our service provider. According to OpenAI's API data-usage policy, API data is not used to train its models by default, and it may be retained by OpenAI for up to 30 days for abuse monitoring. See [OpenAI's privacy policy](https://openai.com/policies/privacy-policy/).
- **Short-term copy of the text:** our server keeps the written text of each voice note for up to **24 hours**, together with a random note ID and pseudonymous identifiers, so that a retry after a lost connection does not send your audio twice. It is then deleted automatically.
- **Fair-use counters:** to protect the service from abuse, our server keeps the number of seconds transcribed per day, keyed by pseudonymous identifiers (see Section 4). Daily entries older than 31 days are deleted automatically.
- Each voice request carries pseudonymous identifiers (the anonymous Firebase user ID and the Application's stable ID described in Section 4) so that the fair-use limit can be applied. It does not carry your name, Apple ID or email.
- While a voice note waits to be written down (for example when you are offline), its audio stays on your device and in your own iCloud. Once the text is saved, the audio file is deleted.
- You can turn voice notes off at any time in **Settings › Voice notes**.

---

## 3. Book Lookups and Covers

- When you scan a barcode, search for a book, browse editions, or import a list, the **ISBN or search words** are sent to our server, which asks public book catalogues to identify the book: **Open Library** (Internet Archive), the **Deutsche Nationalbibliothek**, the **Bibliothèque nationale de France**, and the **National Diet Library** (Japan). A commercial catalogue (ISBNdb) may be added later; if it is, it will be listed in the Application under **Settings › Help › Book sources**.
- Search words are used only to answer the search and are not stored by our server. Book facts found for an ISBN are cached on our server **by ISBN only**, without any link to you, so the next lookup of the same book is faster. Your photos and the titles you type are never written to this shared cache.
- Book **cover images** are downloaded by the Application directly from the cover servers (for example covers.openlibrary.org). As with any web request, your IP address is visible to that server. No diary content is sent.

---

## 4. Identifiers

The Application has no user accounts. To make some features work it uses the following pseudonymous identifiers:

- **Firebase anonymous user ID**: created only the first time the Application needs our server (a book lookup or a voice note). It lets our server reject unauthenticated requests and apply rate limits.
- **Stable ID**: a one-way hash (SHA-256) of your iCloud user record identifier for this Application, or of a random device identifier if iCloud is off. It is used to share your purchase status between your own devices (through RevenueCat) and to apply the voice fair-use limit. It cannot be reversed into your Apple ID, name or email.
- **Support ID**: the first 12 characters of the stable ID. The Application adds it to support emails so we can find the server-side records that belong to you if you ask us to delete them.
- **RevenueCat app user ID**: equal to the stable ID when iCloud is available, otherwise an anonymous RevenueCat ID.
- **Hashed IP address**: to limit abuse, our server stores a salted, one-way hash of your IP address together with the date and a daily request count. These records expire after 2 days. Your IP address itself is not stored by us.

---

## 5. Purchases and Subscriptions

Purchases of **Bookdays Plus** are processed by **Apple** through your App Store account. We never receive your payment details.

We use **RevenueCat** to validate purchases and check whether Bookdays Plus is active. RevenueCat receives your purchase history, the RevenueCat app user ID described above, and basic device information. The Application also enables Apple's **AdServices attribution token** collection through RevenueCat, which tells us whether an install came from an Apple Search Ads campaign. This is used only to measure our own campaigns. It does not use the advertising identifier (IDFA) and is not used to track you across other companies' apps or websites.

---

## 6. Third-Party Access

### Third-Party Services
The Application uses the following third-party services, which have their own privacy policies:

| Service | What it does | Data it receives |
|---|---|---|
| [Google Analytics for Firebase](https://firebase.google.com/support/privacy) | Pseudonymous usage analytics | Allowlisted usage events, app-instance ID, device info, approximate location from IP |
| [Firebase Crashlytics](https://firebase.google.com/support/privacy) | Crash reports | Sanitized crash and diagnostic data, installation ID |
| [Firebase Authentication](https://firebase.google.com/support/privacy) (anonymous) | Protects our server from abuse | Anonymous user ID |
| [Firebase Remote Config](https://firebase.google.com/support/privacy) | Remote settings (free-tier limits, supported voice languages) | Installation ID, app version, device language |
| [Google Cloud Functions for Firebase / Cloud Firestore](https://cloud.google.com/terms/cloud-privacy-notice) | Our server for book lookups and voice notes | ISBNs, search words, voice audio (in transit), pseudonymous IDs |
| [OpenAI](https://openai.com/policies/privacy-policy/) | Writes down voice notes | Voice recordings and the language setting |
| [RevenueCat](https://www.revenuecat.com/privacy) | Purchase validation | Purchase history, RevenueCat app user ID, AdServices token |
| [Apple iCloud](https://www.apple.com/legal/privacy/) | Stores and syncs your diary in your own iCloud account | Your diary, under your Apple ID; we cannot read it |
| Book catalogues: [Open Library](https://archive.org/about/terms.php), Deutsche Nationalbibliothek, Bibliothèque nationale de France, National Diet Library | Book information and covers | ISBNs and search words (from our server); your IP address when the Application downloads a cover |

The Application does **not** include any advertising SDKs, does not show ads, and does not sell or rent your information to anyone.

### Data Disclosure
We may disclose information that we hold:
- As required by law, such as to comply with a subpoena or similar legal process
- When we believe in good faith that disclosure is necessary to protect our rights, your safety or the safety of others, investigate fraud, or respond to a government request
- To the trusted service providers listed above, who process it on our behalf

---

## 7. Permissions

The Application asks for the following permissions only when you first use the related feature:

- **Camera**: to scan a book's barcode, snap its cover, photograph a page to save a quote, or photograph an object for your shelf. Photos are processed on your device.
- **Microphone**: for Hold to talk voice notes (see Section 2).
- **Notifications** (optional): for reading reminders and, if you start a free trial, a reminder before it ends. All notifications are scheduled locally on your device. By default they never show a book title on the lock screen.

When you add a photo frame to your shelf, you choose a single photo with Apple's system photo picker; the Application does not get access to your photo library. If you choose "Save Image" when sharing your year card or a quote card, iOS asks once whether the Application may add photos to your library; it can only add, never read.

The Application does **not** request location, contacts, Bluetooth or tracking permission.

---

## 8. Opt-Out Rights and Your Choices

- You can turn off voice notes in **Settings › Voice notes**; typing works without them.
- You can turn iCloud backup off for the Application in **iOS Settings › your name › iCloud**.
- You can deny or revoke camera, microphone, photo and notification permissions in **iOS Settings › Bookdays**.
- You can stop all collection of information by the Application by uninstalling it.

---

## 9. Data Retention and Deletion

| Data | Where | How long |
|---|---|---|
| Your diary (books, thoughts, quotes, photos) | Your device and your own iCloud | Until you delete it. Deleting the app deletes the copy on the device. To delete the iCloud copy: **iOS Settings › your name › iCloud › Manage Storage › Bookdays** |
| Voice recording | Our server | Not stored (in memory for one request only) |
| Voice recording | OpenAI | Up to 30 days, under OpenAI's API policy |
| Voice-note text | Our server | Up to 24 hours |
| Voice fair-use counters (seconds per day) | Our server | Daily entries deleted after 31 days |
| Hashed IP daily counters | Our server | 2 days |
| Book lookup cache (book facts by ISBN, not linked to you) | Our server | Kept as a shared catalogue; refreshed after 180 days ("not found" results after 14 days) |
| Usage analytics | Google Analytics for Firebase | 14 months |
| Crash reports | Firebase Crashlytics | 90 days |
| Purchase records | Apple and RevenueCat | As long as needed to provide your purchases and meet legal obligations |

The Application has no "delete my account" button because there is no account. If you would like us to delete the pseudonymous data held by us or by RevenueCat, email [support@nextline.software](mailto:support@nextline.software) from **Settings › Help › Contact**, which includes your Support ID, and we will respond within a reasonable timeframe (and within the time required by applicable law).

---

## 10. Your Rights

Depending on where you live (for example under the EU/UK GDPR or the Turkish Personal Data Protection Law No. 6698, "KVKK"), you may have the right to access, correct, delete, or restrict the processing of your personal data, to object to processing, and to data portability. Because your diary is stored on your device and in your own iCloud, you already control it directly, and you can export it at any time from **Settings › Backup & export**. For data held by us or our service providers, contact us with your Support ID. You may also lodge a complaint with your local data protection authority.

Our server and several of our service providers are located in the United States. Where your information is transferred outside your country, we rely on the safeguards offered by those providers (such as standard contractual clauses).

---

## 11. Children

The Application is not directed at children under the age of 13, and we do not knowingly collect personal information from children. If you believe a child has provided us with personal information, please contact us at [support@nextline.software](mailto:support@nextline.software) so we can take the necessary action.

---

## 12. Security

We take reasonable measures to protect information under our control. All communication between the Application, our server and our service providers uses encrypted connections (HTTPS/TLS). Our server's database cannot be read or written by the Application directly. Your diary in iCloud is stored in your private CloudKit database and protected by your Apple ID.

---

## 13. Changes to This Privacy Policy

This Privacy Policy may be updated from time to time for any reason. We will post the new Privacy Policy on this page and update the "Last Updated" date. If we change who receives your voice notes, the Application will ask for your consent again before the next recording is sent. Continued use of the Application after changes are posted constitutes your acceptance of those changes.

---

## 14. Your Consent

By using the Application, you consent to the processing of your information as described in this Privacy Policy, now and as amended by us.

---

## 15. Contact Us

If you have any questions about privacy while using the Application, or about our practices, please contact us:

- **Email**: [support@nextline.software](mailto:support@nextline.software)
- **Developer**: NEXTLINE YAZILIM LİMİTED ŞİRKETİ

**Last Updated**: *November 12, 2026*

---

*This privacy policy page was generated by [App Privacy MD Generator](https://github.com/nextline-yazilim/app-privacy-md-generator)*

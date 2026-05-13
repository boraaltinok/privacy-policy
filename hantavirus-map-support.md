# Hantavirus Map & Alerts — Support

Welcome to the Hantavirus Map & Alerts support page. We're here to help you get the most out of the Application.

## What This App Does

Hantavirus Map & Alerts is a public-health awareness utility that helps you:
- Check reported hantavirus outbreak data on a country-level map.
- Save the places that matter to you (home, family, cabin, travel destinations) and receive alerts when reported risk changes.
- Run a 5-question exposure risk **Self-Check** for general awareness.
- Identify **visible rodent signs** (droppings, nesting material, gnaw marks, entry gaps) with the Rodent-Sign Scanner.
- Follow CDC- and WHO-aligned **safe cleanup** guidance after possible rodent exposure.

The Application is for **awareness and information only**. It is **not** a medical device, does **not** diagnose disease, and does **not** detect viruses or contamination.

---

## Key Features

- **Outbreak Map** with country-level pins, total reported cases, and last-updated timestamp from [HantaCount](https://hantacount.com) (CC-BY-4.0).
- **Saved Locations** with five alert preference switches (risk-level changes, new reported cases, official guidance updates, daily summary, weekly digest).
- **Exposure Self-Check** — five questions, three concern tiers (Low / Possible / Higher), framed as *"your answers suggest..."*, never *"your risk is..."*.
- **Rodent-Sign Scanner** — capture a photo, get a text summary of visible rodent indicators. Photos are analyzed transiently and **never stored** on our servers.
- **Safe Cleanup Checklist** — aligned with CDC and WHO guidance for handling areas with rodent activity.
- **Outbreak Source Cards** with source attribution and link-outs to official public-health resources.
- **Locale-aware emergency CTAs** that read from local emergency-number mappings (no hardcoded numbers).

---

## Frequently Asked Questions

### General

**Q: Can this app diagnose hantavirus?**
A: **No.** The Application is an awareness utility, not a medical device. It does not diagnose disease, infection, or contamination. The Self-Check provides general awareness only. If you have symptoms or concerns, contact a qualified medical professional or your local public-health authority.

**Q: Does the scanner detect the virus?**
A: **No.** The Scanner identifies **visible rodent signs** (droppings, nesting material, gnaw marks, entry gaps, urine or smear marks) using AI image analysis. It does not detect viruses, surface contamination, or pathogen presence. Always follow official public-health guidance before disturbing any area suspected of rodent activity.

**Q: Where does the outbreak data come from?**
A: Outbreak data is sourced from [HantaCount](https://hantacount.com) under the Creative Commons Attribution 4.0 license. We display attribution and a last-updated timestamp on every data screen. The Application also links out to official sources such as WHO, CDC, ECDC, and PAHO.

**Q: How often is the data updated?**
A: We sync from HantaCount every 30–60 minutes during active outbreak periods. The map will show the last-cached update if the source is briefly unavailable.

---

### Permissions

**Q: Why does the app ask for camera permission?**
A: The camera is used **only** by the Rodent-Sign Scanner to capture a photo of an area you want analyzed. Photos are sent to our backend for one-time analysis and are **not stored** on our servers. The camera is not used for any other purpose.

**Q: Why does the app ask for location permission?**
A: Location is requested **once**, during post-purchase setup, **only** to suggest a first country or region for you to monitor. We request "While Using" permission only — never "Always." If you decline, you can search for places manually instead. We do not track your location continuously.

**Q: Why does the app ask for notification permission?**
A: To deliver outbreak advisories for the locations you save. You can change this at any time in your device settings.

---

### Privacy & Data

**Q: Do you store my scanner photos?**
A: **No.** Photos are sent over an encrypted connection (HTTPS) for one-time analysis, the result is returned, and the image is discarded. The Application does not retain scanner photos on our servers, in Firebase Storage, or in Firestore.

**Q: Do I need an account?**
A: **No.** The Application does not require an email, password, or social login. An anonymous identifier is generated on your device at first launch to associate your saved locations and subscription state with your installation.

**Q: How do I request deletion of my data?**
A: Because the Application does not require an account, email **support@nextline.software** with reasonable identifying details (for example, the country code of your saved location and the approximate date you began using the Application) so we can locate and delete your record.

**Q: Is my data secure?**
A: All transmissions to our backend and to third-party services use encrypted connections (HTTPS). Sensitive backend operations require authentication and are protected by rate limits.

---

### Technical Support

**Q: The app isn't working properly. What should I try?**
A: Standard troubleshooting:
1. Close and reopen the Application.
2. Restart your device.
3. Confirm you are on the latest version from the App Store.
4. Check your internet connection.
5. Verify that you have granted the necessary permissions (camera for Scanner, location for first-time setup, notifications for alerts).

**Q: The map isn't loading.**
A: The map needs an internet connection. If you are offline, the Application will show the last cached snapshot with a stale-data banner. Once connectivity is restored, the map will refresh.

**Q: The scanner won't analyze my photo.**
A: Common causes:
- Blurry photo — retake in better lighting.
- No internet connection — Scanner requires connectivity.
- Hourly rate limit reached — wait a short while and try again.
- Server-side issue — try again later; if it persists, contact support.

**Q: I'm not receiving alerts.**
A: Check the following:
- Notification permission is enabled in your device settings.
- You have at least one saved location with the relevant alert switches turned on.
- Your subscription is active.
- Alerts are rate-limited (maximum 1 per saved location per 12 hours, 2 per user per day) to avoid fatigue.

**Q: How do I update the app?**
A: App updates are typically automatic. You can also manually check for updates in the App Store.

---

### Subscription

**Q: Is there a free trial?**
A: The 6-month plan includes a **7-day free trial**. If you do not cancel before the trial ends, your Apple ID will be charged for the subscription. Trial eligibility is determined by Apple and may be limited to one trial per Apple ID.

**Q: How do I restore my purchase on a new device?**
A: Open the Application and tap **Restore Purchases** on the paywall or in **Settings**. You must be signed into the same Apple ID that made the original purchase.

**Q: How do I cancel my subscription?**
A: Subscriptions are managed by Apple. Go to your iPhone **Settings → [Your Name] → Subscriptions** and cancel from there. You can also tap **Manage Subscription** in the Application's Settings to open the App Store subscription page.

**Q: I was charged but the app says I don't have access.**
A: Tap **Restore Purchases** in the Application. If the issue persists, contact us at **support@nextline.software** with your Apple ID receipt details.

**Q: Can I get a refund?**
A: Refunds are processed by Apple in accordance with App Store policy. Request a refund at [reportaproblem.apple.com](https://reportaproblem.apple.com).

---

### Outbreak Data & Sources

**Q: Why doesn't the map show my exact city?**
A: The Application is intentionally **country-level**. The data source (HantaCount) provides country-granularity figures. Inventing precision the source does not support would mislead users. Saved-location monitoring is also country/region-level.

**Q: Is this app affiliated with the CDC, WHO, or ECDC?**
A: **No.** The Application links out to those public-health authorities as informational sources but is not affiliated with, endorsed by, or operated by any of them.

---

## Account and Data Management

**Q: How do I delete my data?**
A: Email **support@nextline.software** with reasonable identifying details. Note that the Application does not require an account — there is no separate "delete account" action because no account exists.

**Q: Can I export my data?**
A: For data export inquiries, contact **support@nextline.software**.

---

## Contact Support

If you need further assistance:

**Email:** [support@nextline.software](mailto:support@nextline.software)

### When contacting support, please provide:
- Your device model and operating system version
- App version number (visible at the bottom of the Settings screen)
- A detailed description of the issue
- Steps you have already tried

---

## Privacy and Legal

- [Privacy Policy](./hantavirus-map-privacy-policy.md)
- [Terms & Conditions](./hantavirus-map-terms-conditions.md)

For privacy-related concerns, contact **support@nextline.software**.

---

**App Version:** Latest
**Last Updated:** May 13, 2026
**Developer:** NEXTLINE YAZILIM LİMİTED ŞİRKETİ

---

*Prepared for the Hantavirus Map & Alerts application. Content reflects the actual behavior of the Application as of the date above.*

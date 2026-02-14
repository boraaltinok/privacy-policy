# Privacy Policy for Lottery Ticket Scanner App for Mega Millions

**Effective Date:** February 14, 2026

**Last Updated:** February 14, 2026

## Important Disclaimer

**Disclaimer:** Lottery Ticket Scanner App for Mega Millions is an independent third-party utility and is not affiliated with, endorsed by, or sponsored by Mega Millions®, Powerball®, or any official state lottery organization. Mega Millions® and Powerball® are registered trademarks of their respective owners. This app is not produced, supported, endorsed, nor associated with any state or national lottery commission.

---

## 1. Information Collection

When you use Lottery Ticket Scanner App for Mega Millions ("the App"), operated by NEXTLINE YAZILIM LİMİTED ŞİRKETİ ("Service Provider," "we," "our"), we may collect and process the following types of information:

### 1.1 Ticket Image Data
- **Ticket Images**: When you use our ticket scanning features, the app processes photos you take with your camera or select from your photo library. These images are compressed, converted to base64 format, and transmitted securely via HTTPS to our Firebase Cloud Functions for AI-powered number extraction using OpenRouter LLM services.
- **What Images May Contain**: Lottery ticket images may include printed information such as ticket serial numbers, retailer information, purchase dates, and lottery numbers.
- **Processing**: Images are processed to extract Mega Millions lottery numbers, draw dates, and Megaplier selections from your ticket.
- **Retention**: Ticket images are processed in real-time and are not permanently stored on our servers. Images may be temporarily retained in memory during the extraction process and are deleted after processing completion. OpenRouter, our AI processing service, may temporarily retain request data for service delivery and abuse monitoring purposes, after which it is deleted.

### 1.2 Device and Usage Information
- **Device Identifiers**: We collect anonymous device identifiers for analytics and crash reporting purposes.
- **App Usage Data**: Information about how you interact with the app, including features used, session duration, and navigation patterns.
- **Camera Permissions**: The app requires camera access to capture ticket images for scanning purposes.
- **Approximate Location**: We may collect approximate location data (e.g., based on IP address) for analytics, personalized content, and service improvement. We do not collect precise GPS-level location data.

### 1.3 Lottery Number Data
- **Scanned Numbers**: Lottery numbers extracted from your scanned tickets are sent to our Cloud Functions to check against winning numbers.
- **Manually Entered Numbers**: Numbers you enter or generate in the Create Ticket feature are processed similarly.
- **Local Storage**: Ticket data may be stored locally on your device using an encrypted local database for your convenience.

### 1.4 Authentication
- **Anonymous Authentication**: The app uses Firebase Anonymous Authentication to create a unique, anonymous user identifier. This identifier does not require you to provide any personal information such as name, email, or phone number. It is used to manage your subscription status and provide personalized app functionality.

## 2. Third-Party Access

### 2.1 Firebase Services (Google)
We utilize several Firebase services provided by Google:
- **Firebase Anonymous Authentication**: For creating anonymous user sessions without collecting personal information
- **Firebase Analytics**: For understanding app usage patterns and improving user experience
- **Firebase Crashlytics**: For monitoring app stability and fixing crashes
- **Cloud Firestore**: For retrieving winning lottery numbers and managing user data
- **Firebase Cloud Functions**: For processing ticket scanning and winning number verification requests

Firebase may collect additional data as described in Google's Privacy Policy: https://policies.google.com/privacy

### 2.2 OpenRouter AI Services
- **Purpose**: Ticket number extraction through AI/ML-powered optical character recognition (OCR)
- **Data Transmitted**: Compressed ticket images (base64 format) sent via our Firebase Cloud Functions
- **Processing**: Images are analyzed by a large language model to extract lottery numbers, draw dates, and game details
- **Retention**: OpenRouter processes images for the purpose of fulfilling the request. Data may be temporarily retained for service delivery and abuse monitoring, after which it is deleted
- **Security**: All data transmission occurs over encrypted HTTPS connections

### 2.3 RevenueCat
- **Purpose**: Subscription management and in-app purchase processing
- **Data Collected**: Anonymous user identifiers, subscription status, purchase receipts
- **Processing**: Handles premium subscription verification and management
- **Privacy Policy**: https://www.revenuecat.com/privacy

### 2.4 Amplitude Analytics
- **Purpose**: Advanced analytics for app improvement and user experience optimization
- **Data Collected**: App usage events, feature interactions, session data, and anonymized user behavior patterns
- **Privacy Policy**: https://amplitude.com/privacy

### 2.5 Apple App Store / Google Play Store
- **Purpose**: App distribution, in-app purchase processing, and subscription billing
- **Data Collected**: Purchase and subscription information is processed through the respective platform

The Service Provider may disclose user-provided or automatically collected information:
- As required by law (e.g., to comply with legal processes such as a subpoena)
- When necessary to protect rights, safety, or investigate fraud
- With trusted service providers working on our behalf, bound by confidentiality agreements consistent with this privacy policy

## 3. How We Use Information

### 3.1 Core App Functionality
- **Ticket Scanning**: Processing uploaded images to accurately extract Mega Millions lottery numbers
- **Winning Verification**: Checking scanned or entered numbers against official winning numbers
- **Drawing Results**: Displaying latest and historical Mega Millions drawing results
- **Service Improvement**: Analyzing usage patterns to enhance accuracy and user experience

### 3.2 Analytics and Performance
- **App Performance**: Monitoring crashes and technical issues to improve app stability
- **Feature Usage**: Understanding which features are most valuable to optimize development
- **User Experience**: Analyzing navigation and interaction patterns to improve app design

### 3.3 Notifications
- **Local Notifications**: The app may send local device notifications as reminders about drawing dates or to re-engage users. These notifications are scheduled locally on your device and do not require transmitting data to external servers.

### 3.4 Advertising Attribution
- **App Tracking Transparency (iOS)**: On iOS devices, the app may request permission to track your activity across other companies' apps and websites for the purpose of measuring advertising effectiveness. You can deny this request with no impact on app functionality.
- **AdServices Attribution**: If tracking is permitted, anonymous attribution tokens may be collected to measure advertising campaign performance.

## 4. Data Security and Storage

### 4.1 Security Measures
- **Encryption**: All data transmission between the app and external services uses HTTPS/TLS encryption
- **Local Storage**: App data is stored on your device using a local database (Hive)
- **Anonymous Processing**: Ticket scanning is performed without associating images with personal identifiers
- **Image Compression**: Ticket images are compressed before transmission to minimize data exposure

### 4.2 Data Retention
- **Ticket Images**: Processed in real-time and not permanently stored on our servers
- **Analytics Data**: Aggregated usage data may be retained for service improvement purposes
- **Local Data**: App data remains on your device until you delete the app or manually clear the data
- **Authentication**: Your anonymous user identifier persists until the app is uninstalled or data is cleared

### 4.3 Third-Party Security
We work with reputable third-party services that maintain their own security standards:
- Firebase/Google Cloud Platform security standards
- OpenRouter AI service security protocols
- RevenueCat payment security compliance

## 5. Your Rights and Choices

### 5.1 Data Access and Deletion
- **Local Data**: You can delete your local app data by uninstalling the app
- **Server Data**: Contact support@nextline.software to request deletion of any server-side data associated with your anonymous identifier
- **Analytics Opt-Out**: You can request to opt out of analytics tracking by contacting support

### 5.2 Permissions Management
- **Camera Access**: You can revoke camera permissions in your device settings, though this will limit core scanning functionality
- **Notification Permissions**: You can disable notifications in your device settings
- **Tracking (iOS)**: You can change your App Tracking Transparency preference in iOS Settings > Privacy > Tracking

### 5.3 Subscription Management
- **Premium Features**: Manage your subscription through the App Store (iOS) or Google Play (Android)

Contact support@nextline.software to exercise these rights.

## 6. Opt-Out Rights

You can stop all collection of information by uninstalling the Application. You may also use the standard uninstall processes available on your mobile device or via the mobile application marketplace or network.

## 7. Children

The Application is not intended for use by children under 13. We do not knowingly collect personal information from children under 13. If we discover that a child under 13 has provided us with personal information, we will delete it immediately. If you are a parent or guardian and you are aware that your child has provided us with personal information, please contact us at support@nextline.software so that we can take necessary action.

## 8. Changes to This Privacy Policy

We may update this Privacy Policy from time to time. We will notify you of any changes by posting the new Privacy Policy on this page and updating the "Last Updated" date. Changes become effective when posted.

For significant changes affecting data processing, we may provide additional notice through the app.

## 9. Your Consent

By using Lottery Ticket Scanner App for Mega Millions, you consent to the collection and use of information as outlined in this Privacy Policy. If you do not agree with this policy, please do not use the app.

You can withdraw consent by uninstalling the app, which will stop all data collection. Locally stored data will be removed upon uninstallation.

## 10. Contact Information

If you have any questions about this Privacy Policy or our data practices, please contact us:

**NEXTLINE YAZILIM LİMİTED ŞİRKETİ**
- **Email**: support@nextline.software
- **Subject Line**: Privacy Policy - Lottery Ticket Scanner App for Mega Millions

---

**Service Notice**: Lottery Ticket Scanner App for Mega Millions is provided "AS IS" without warranties. We strive for accuracy in ticket scanning and number extraction, but cannot guarantee 100% accuracy for all tickets or conditions. Always verify results against your physical ticket and official lottery sources.

**Trademark Notice**: Lottery Ticket Scanner App for Mega Millions is an independent third-party utility. Mega Millions® and Powerball® are registered trademarks of their respective owners. This app is not affiliated with, endorsed by, or sponsored by any official lottery organization.

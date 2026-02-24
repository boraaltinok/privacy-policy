# Privacy Policy for Whiskey Scanner

**Effective Date:** February 24, 2026

**Last Updated:** February 24, 2026

---

## 1. Information Collection

When you use Whiskey Scanner ("the App"), operated by NEXTLINE YAZILIM LİMİTED ŞİRKETİ ("Service Provider," "we," "our"), we may collect and process the following types of information:

### 1.1 Image Data
- **Bottle Images**: When you use our bottle scanning features, the app processes photos you take with your camera or select from your photo library. These images are compressed, converted to base64 format, and transmitted securely via HTTPS to Firebase Cloud Functions for AI-powered whiskey identification.
- **Processed Images**: Images are processed to identify whiskey bottles, including brand, category, flavor profile, tasting notes, and pricing information.
- **Image Storage**: Scan images are stored securely in Firebase Storage (at the path `scans/{userId}/{scanId}`) and are associated with your anonymous user account. These images are retained to allow you to view your previously scanned bottles within the app.
- **Image Deletion**: You can delete your stored images by removing bottles from your collection or by uninstalling the app and requesting data deletion via email.

### 1.2 Device and Usage Information
- **Device Identifiers**: We collect anonymous device identifiers for analytics and crash reporting purposes.
- **App Usage Data**: Information about how you interact with the app, including features used, session duration, and navigation patterns.
- **Camera Permissions**: The app requires camera access to capture bottle images for identification purposes.
- **Approximate Location**: We may collect approximate location data (e.g., based on IP address) for analytics and service improvement. We do not collect precise GPS-level location data.

### 1.3 Collection Data
- **Whiskey Collection**: Your whiskey collection data (bottle details, flavor profiles, tasting notes, status) is stored in Cloud Firestore under your anonymous user account. This data is synced across sessions.
- **Local Data**: Certain app data, including chat history and cached information, is stored locally on your device using a Hive database.
- **User Notes**: Any personal tasting notes or preferences you add to bottles are stored in Cloud Firestore associated with your anonymous account.

### 1.4 Authentication
- **Anonymous Authentication**: The app uses Firebase Anonymous Authentication to create a unique, anonymous user identifier. This identifier does not require you to provide any personal information such as name, email, or phone number. It is used to manage your subscription status, scan history, and collection data.

## 2. Third-Party Access

### 2.1 Firebase Services (Google)
We utilize several Firebase services provided by Google:
- **Firebase Anonymous Authentication**: For creating anonymous user sessions without collecting personal information
- **Firebase Analytics**: For understanding app usage patterns and improving user experience
- **Firebase Crashlytics**: For monitoring app stability and fixing crashes
- **Cloud Firestore**: For storing user profiles and whiskey collection data
- **Firebase Cloud Functions**: For processing bottle scanning and AI-powered identification requests
- **Firebase Storage**: For storing scan images associated with your account

Firebase may collect additional data as described in Google's Privacy Policy: https://policies.google.com/privacy

### 2.2 AI Processing Services
- **Purpose**: Whiskey bottle identification and analysis through AI/ML models
- **Data Transmitted**: Compressed bottle images (base64 format) sent via our Firebase Cloud Functions
- **Processing**: Images are analyzed by AI models to identify whiskey details including brand, flavor profile, tasting notes, and pricing
- **Server-Side Processing**: All AI processing is handled entirely server-side through our Cloud Functions. No AI API keys or direct AI service connections exist on the client app.
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
- **Bottle Identification**: Processing uploaded images to accurately identify whiskey bottles, including brand, category, flavor profile, and pricing
- **Collection Management**: Enabling storage and organization of your whiskey collection in Cloud Firestore
- **AI Whiskey Advisor**: Providing an AI-powered chat assistant (the "Professor") for whiskey recommendations and education based on your collection
- **Service Improvement**: Analyzing usage patterns to enhance accuracy and user experience

### 3.2 Analytics and Performance
- **App Performance**: Monitoring crashes and technical issues to improve app stability
- **Feature Usage**: Understanding which features are most valuable to optimize development
- **User Experience**: Analyzing navigation and interaction patterns to improve app design

### 3.3 Notifications
- **Local Notifications**: The app may send local device notifications as reminders or to re-engage users. These notifications are scheduled locally on your device and do not require transmitting data to external servers.

### 3.4 Advertising Attribution
- **App Tracking Transparency (iOS)**: On iOS devices, the app may request permission to track your activity across other companies' apps and websites for the purpose of measuring advertising effectiveness. You can deny this request with no impact on app functionality.
- **AdServices Attribution**: If tracking is permitted, anonymous attribution tokens may be collected to measure advertising campaign performance.

## 4. Data Security and Storage

### 4.1 Security Measures
- **Encryption**: All data transmission between the app and external services uses HTTPS/TLS encryption
- **Cloud Storage**: Scan images and collection data are stored securely in Firebase services with Google Cloud Platform security standards
- **Local Storage**: Cached app data is stored on your device using a Hive database
- **Anonymous Processing**: All data is associated with anonymous identifiers, not personal information

### 4.2 Data Retention
- **Scan Images**: Stored in Firebase Storage and retained while your account is active. Images can be deleted by removing bottles from your collection or by contacting support.
- **Collection Data**: Retained in Cloud Firestore while your account is active
- **Analytics Data**: Aggregated usage data may be retained for service improvement purposes
- **Local Data**: App data remains on your device until you delete the app or manually clear the data
- **Authentication**: Your anonymous user identifier persists until the app is uninstalled or data is cleared

### 4.3 Third-Party Security
We work with reputable third-party services that maintain their own security standards:
- Firebase/Google Cloud Platform security standards
- RevenueCat payment security compliance
- Amplitude analytics security protocols

## 5. Your Rights and Choices

### 5.1 Data Access and Deletion
- **Local Data**: You can delete your local app data by uninstalling the app
- **Server Data**: Contact support@nextline.software to request deletion of any server-side data associated with your anonymous identifier
- **Collection Data**: You can delete individual bottles from your collection within the app
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

By using Whiskey Scanner, you consent to the collection and use of information as outlined in this Privacy Policy. If you do not agree with this policy, please do not use the app.

You can withdraw consent by uninstalling the app, which will stop all data collection. Locally stored data will be removed upon uninstallation. To request deletion of server-side data, contact support@nextline.software.

## 10. Contact Information

If you have any questions about this Privacy Policy or our data practices, please contact us:

**NEXTLINE YAZILIM LİMİTED ŞİRKETİ**
- **Email**: support@nextline.software
- **Subject Line**: Privacy Policy - Whiskey Scanner

For data protection inquiries specifically related to GDPR compliance, please include "GDPR Request" in your subject line.

---

**Service Notice**: Whiskey Scanner is provided "AS IS" without warranties. We strive for accuracy in bottle identification and whiskey information, but cannot guarantee 100% accuracy for all bottles or market conditions.

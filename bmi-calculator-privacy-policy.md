**Privacy Policy**

This privacy policy applies to the BMI Calculator: Weight Plan app (hereby referred to as "Application") for mobile devices that was created by NEXTLINE YAZILIM LİMİTED ŞİRKETİ (hereby referred to as "Service Provider") as a Commercial service. This service is intended for use "AS IS".

**Information Collection and Use**

The Application collects information when you download and use it. This information may include information such as

*   Your device's Internet Protocol address (e.g. IP address)
*   The operating system you use on your mobile device
*   Crash diagnostic data when the Application encounters an error
*   Product analytics events (such as which screens you view and which features you interact with)
*   An anonymous user identifier assigned by Firebase Authentication, device identifiers used by analytics and crash-reporting services, and purchase entitlement information provided by RevenueCat and the Apple App Store
*   In-app purchase entitlement status needed to determine whether premium features are available

The Application does not request access to the iOS or Android location APIs and does not use GPS, Wi-Fi-based, or cellular-tower-based location services. Some third-party services listed under "Third Party Access" below (notably Amplitude) may derive an approximate (city / region level) location from the IP address attached to network requests for analytics purposes; the Service Provider does not receive precise geographical coordinates from your device.

The Application does not access the microphone, camera, photo library, contacts, calendar, motion sensors, or any health data store on your device (such as Apple Health or Google Fit).

For a better experience, while using the Application, the Service Provider requires you to provide the following information that you enter into the Application directly:

*   Age, selected sex option (Female / Male / Prefer not to say), height, and weight — used on-device to calculate your Body Mass Index (BMI) and, for premium users, to generate a personalized Action Plan.
*   Optional weight check-in entries — recorded to display your weight history inside the Application.
*   Optional answers to a short multiple-choice interview (goal direction, daily routine, coaching style preference) — used to personalize the AI-generated Action Plan.
*   Optional messages you send to the in-app AI Coach — transmitted to the AI processing service described below to generate a reply.

Some of this information is stored on your device. Some information may also be synced to the Service Provider's cloud database under an anonymous identifier — primarily to power premium features (plan setup, plan history, weight check-ins, and AI Coach). Interview answers entered before purchase may be stored temporarily under the same anonymous identifier so that your plan setup can be resumed if you leave the Application before unlocking the plan.

The Service Provider does not collect your email address, phone number, real name, postal address, payment card information, or any other directly identifying personal contact information. Payments are processed entirely by the Apple App Store and the Service Provider receives no payment card or billing details.

**Anonymous Authentication**

The Application uses Firebase Authentication in anonymous mode to assign each installation an anonymous user identifier (UID). This identifier:

*   Is generated automatically when you open the Application — you are NOT asked to register, sign up, choose a username, or enter a password.
*   Is not linked to your name, email address, or any external account.
*   Is used to associate your BMI history, plan, weight check-ins, and AI Coach conversations with your installation so that they persist across sessions on the same device.
*   May be reset by the Service Provider's "Delete my data" feature inside the Application, after which a new anonymous UID is assigned to the same installation.

**AI Processing**

For premium users, the Application offers an AI-generated Action Plan and an AI Coach conversation feature. To provide these features, the following data is transmitted from your device to the Service Provider's cloud backend, and from there to a third-party AI provider:

*   Your BMI inputs (age, sex, height, weight, BMI category)
*   Your answers to the in-app interview (goal direction, struggles, daily routine, coaching style)
*   The messages you type into the AI Coach
*   A short rolling window of the recent AI Coach conversation, for context

The third-party AI provider used to generate plan content and coach replies is **OpenRouter** (see Third Party Access below). The Application may also send your selected app language / locale so that AI-generated content can be returned in the correct language. Generated responses are returned to your device for display and stored in the Service Provider's cloud database under your anonymous UID for as long as you continue to use the Application.

**Local Device Storage**

The Application stores the following information locally on your device so that the Application can function offline and across sessions:

*   Your most recent BMI inputs and the calculated BMI value
*   Your BMI calculation history
*   Your weight check-in entries
*   Your unit-system preference (metric or imperial)
*   Your selected language and country (for localized content)
*   A cached copy of the Action Plan and AI Coach chat for premium users

This local data is not transmitted off your device except as described in the AI Processing and Third Party Access sections.

**Third Party Access**

Only the data described in the sections above is transmitted to external services to provide the features described to you. The Service Provider may share your information with third parties in the ways described in this privacy statement.

The Application uses the following third-party services, each of which has its own privacy policy regarding the handling of data:

*   [Firebase Authentication](https://firebase.google.com/support/privacy) — anonymous user identification
*   [Firebase Cloud Firestore](https://firebase.google.com/support/privacy) — cloud database for plan setup, plan history, weight check-ins, and AI Coach conversations
*   [Firebase Cloud Functions](https://firebase.google.com/support/privacy) — backend processing for plan generation and AI Coach
*   [Firebase Crashlytics](https://firebase.google.com/support/privacy/) — crash diagnostic reporting
*   [Amplitude](https://amplitude.com/privacy) — product analytics, such as screen views, feature interactions, subscription funnel events, and approximate location derived from IP address
*   [RevenueCat](https://www.revenuecat.com/privacy) — in-app subscription management and entitlement state
*   [OpenRouter](https://openrouter.ai/privacy) — AI text generation for premium Plan and Coach features
*   [Apple App Store](https://www.apple.com/legal/privacy/) — payment processing and subscription billing

The Service Provider may disclose User Provided and Automatically Collected Information:

*   as required by law, such as to comply with a subpoena, or similar legal process;
*   when they believe in good faith that disclosure is necessary to protect their rights, protect your safety or the safety of others, investigate fraud, or respond to a government request;
*   with their trusted services providers who work on their behalf, do not have an independent use of the information we disclose to them, and have agreed to adhere to the rules set forth in this privacy statement.

**No Cross-App Tracking and No Advertising**

The Application does **not** display advertisements, does **not** integrate any advertising or ad-attribution SDK, and does **not** participate in cross-app tracking under Apple's App Tracking Transparency framework. No data collected by the Application is shared with third-party advertising networks for targeting, measurement, or attribution.

**Opt-Out Rights**

You can stop all collection of information by the Application easily by uninstalling it. You may use the standard uninstall processes as may be available as part of your mobile device or via the mobile application marketplace or network.

You can also request deletion of the cloud-stored data associated with your installation at any time by using the **"Delete my data"** option in the Application's profile/settings screen. This operation removes your anonymous-UID data (plan, history, AI Coach messages, weight log) from the Service Provider's cloud database.

**Data Retention Policy**

The Service Provider will retain User Provided data for as long as you use the Application and for a reasonable time thereafter. If you'd like them to delete User Provided Data that you have provided via the Application, please contact them at support@nextline.software and they will respond in a reasonable time. You may also use the in-app "Delete my data" option described under Opt-Out Rights.

**Children**

The Application includes BMI calculation inputs for a wide age range, including children and teens, but it is not directed to children under 13 as a standalone child-targeted service. The Service Provider does not market the Application to children under 13. Children under 13 should use the Application only with the involvement and consent of a parent or guardian.

For children and teens, BMI should be interpreted with the help of a parent, guardian, or qualified healthcare professional. The age-appropriate result and content shown in the Application is informational only and is not a substitute for pediatric medical guidance.

The Service Provider does not knowingly collect personally identifiable information from children under 13 years of age beyond the anonymous BMI inputs described in the Information Collection and Use section. If you are a parent or guardian and you are aware that your child has provided us with personal information that should be removed, please contact the Service Provider at support@nextline.software so that they can take the necessary actions.

**Security**

The Service Provider is concerned about safeguarding the confidentiality of your information. The Service Provider provides physical, electronic, and procedural safeguards to protect information the Service Provider processes and maintains. Data transmitted between the Application and the Service Provider's cloud backend is encrypted in transit using industry-standard HTTPS/TLS.

**Changes**

This Privacy Policy may be updated from time to time for any reason. The Service Provider will notify you of any changes to the Privacy Policy by updating this page with the new Privacy Policy. You are advised to consult this Privacy Policy regularly for any changes, as continued use is deemed approval of all changes.

This privacy policy is effective as of 2026-05-16

**Your Consent**

By using the Application, you are consenting to the processing of your information as set forth in this Privacy Policy now and as amended by us.

**Contact Us**

If you have any questions regarding privacy while using the Application, or have questions about the practices, please contact the Service Provider via email at support@nextline.software.

* * *

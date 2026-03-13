# Privacy Policy

_Last updated: 2026-03-13_

Thank you for using **Back in Stock ‑ Notify Me** ("Application", "App"). This Privacy Policy explains how NEXTLINE YAZILIM LİMİTED ŞİRKETİ ("Service Provider", "we", or "us") collects, uses, and protects your information when you use our Application.

This policy applies to both **merchants** who install the App through the Shopify App Store and **customers** (end users of merchant stores) who interact with the App's storefront widgets.

## 1. Information We Collect

### Information Collected from Merchants
When a merchant installs and uses the App, we collect:
- **Shop domain** and store information provided by Shopify during app installation.
- **App settings** configured by the merchant, including email sender name, email subject line, low stock threshold, and notification preferences.
- **Resend API key** (optional) — if the merchant chooses to send emails from their own domain.

### Information Collected from Customers
When a customer subscribes to a back-in-stock notification on a merchant's store, we collect:
- **Email address** — provided voluntarily by the customer through the storefront notification widget.
- **Product interest** — the specific product and variant the customer wants to be notified about (product title, variant title, product handle, and product image URL).

### Automatically Collected Information
- **IP address** — used solely for rate limiting on the subscription API endpoint. IP addresses are held in temporary memory only and are not stored in our database.

### Information We Do NOT Collect
- We do not use cookies or tracking scripts on merchant storefronts.
- We do not collect payment information, physical addresses, phone numbers, or demographic data from customers.
- We do not collect analytics or behavioral data from customers.

## 2. How We Use Information

We use the collected information exclusively to provide the App's core functionality:
- **Customer email addresses** — to send back-in-stock notification emails when a product they subscribed to is restocked.
- **Product interest data** — to match inventory updates with the correct subscribers.
- **Merchant settings** — to customize notification emails (sender name, subject line) and control app behavior (thresholds, active/inactive status).
- **IP addresses** — for rate limiting to prevent abuse of the subscription endpoint. Not persisted.

We do not use any collected data for advertising, profiling, or marketing purposes unrelated to the App's core functionality.

## 3. Shopify API Data

Our App accesses the following Shopify API scopes:

| Scope | Purpose |
|-------|---------|
| `read_products` | To look up product and variant information when processing inventory webhooks |
| `write_products` | Required by the Shopify app framework for product-related operations |
| `read_inventory` | To detect inventory level changes that trigger back-in-stock notifications |
| `write_inventory` | Required by the Shopify app framework for inventory-related operations |

Shopify API data is processed only to match inventory updates with subscriber records. We do not store raw Shopify API responses beyond what is needed for notification matching.

## 4. Third-Party Services

Our Application uses the following third-party services:

### Resend (Email Delivery)
- **Data shared:** Customer email addresses, product titles, product image URLs, and merchant shop domain.
- **Purpose:** To deliver back-in-stock notification emails to customers.
- **Privacy policy:** [https://resend.com/legal/privacy-policy](https://resend.com/legal/privacy-policy)

### Shopify
- **Data shared:** App operates as an embedded Shopify app and communicates with the Shopify Admin API.
- **Purpose:** To access product and inventory data for notification matching.
- **Privacy policy:** [https://www.shopify.com/legal/privacy](https://www.shopify.com/legal/privacy)

### Fly.io (Hosting)
- **Data shared:** All application data is processed on Fly.io infrastructure.
- **Purpose:** Application hosting and database hosting.
- **Privacy policy:** [https://fly.io/legal/privacy-policy/](https://fly.io/legal/privacy-policy/)

We do not sell, rent, or share personal data with any other third parties.

## 5. Data Storage & Security

- All data is stored in a PostgreSQL database hosted on Fly.io.
- Data is encrypted in transit via TLS/HTTPS.
- Resend API keys provided by merchants are stored in the database. We recommend merchants use API keys with minimal required permissions.
- Access to production systems is restricted to authorized personnel only.

## 6. Data Retention & Deletion

### During App Usage
- **Subscription records** are retained as long as the merchant has the App installed.
- **Notification logs** (delivery status records) are retained for operational monitoring.
- Customers who have been notified are marked as "notified" but their records are retained so the merchant can review notification history.

### On App Uninstall
When a merchant uninstalls the App, we **automatically and permanently delete** all data associated with their store:
- All customer subscription records
- All notification logs
- All merchant settings (including any stored API keys)
- All session data

### GDPR Compliance Webhooks
Our App implements all mandatory Shopify GDPR/privacy webhooks:

- **`customers/data_request`** — We acknowledge the request. The data we store (email and product interest) is available for export upon request.
- **`customers/redact`** — We permanently delete all subscription records associated with the specified customer's email address for the requesting store.
- **`shop/redact`** — We permanently delete all data (subscriptions, notification logs, settings) associated with the store.

## 7. Your Rights

### For Customers (GDPR/CCPA)
As a customer who has subscribed to a back-in-stock notification, you have the right to:
- **Access** — Request a copy of the data we hold about you.
- **Correction** — Request correction of inaccurate data.
- **Deletion** — Request deletion of your subscription and notification data.
- **Portability** — Request your data in a portable format.

To exercise any of these rights, contact us at [support@nextline.software](mailto:support@nextline.software) with the email address used for the subscription and the store domain.

### For Merchants
Merchants can view all subscriber data in the App dashboard. To request complete data deletion, uninstall the App (which triggers automatic deletion) or contact us at [support@nextline.software](mailto:support@nextline.software).

### California Residents (CCPA)
California residents have additional rights under the CCPA, including the right to know what personal information is collected and the right to opt out of the sale of personal information. **We do not sell personal information.**

## 8. Children's Privacy

Our Application is not directed at children under the age of 13 (or 16 in the European Economic Area). We do not knowingly collect personal information from children. If you believe we have inadvertently collected information from a child, please contact us immediately at [support@nextline.software](mailto:support@nextline.software) so we can promptly delete the data.

## 9. Changes to This Privacy Policy

We may update this Privacy Policy from time to time. Any changes will be reflected by updating the "Last updated" date at the top of this page. For material changes, we will notify merchants through the App interface. Continued use of the Application after modifications constitutes acceptance of the updated terms.

## 10. Contact Us

If you have any questions about this Privacy Policy, our data practices, or wish to exercise your data rights, please contact us:

- **Company:** NEXTLINE YAZILIM LİMİTED ŞİRKETİ
- **Email:** [support@nextline.software](mailto:support@nextline.software)

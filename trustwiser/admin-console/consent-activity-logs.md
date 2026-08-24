---
layout:
  width: default
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: false
  pagination:
    visible: true
  metadata:
    visible: false
  tags:
    visible: true
---

# Consent Activity Logs

The **Consent Activity Logs** provides a complete audit trail of all consent-related actions and updates. The dashboard gives a quick summary of consent activity:

* **Total Records** – Total number of consent-related entries across all categories
* **Customer Activity Logs** – Actions performed by or on behalf of customers
* **Admin Activity Logs** – Configuration or consent changes made by administrators
* **API Activity Logs** – Consent updates triggered through API integrations

Example: If a customer updates his/her communication preference by disabling Email notifications, the system records the change instantly, the log captures both **old value (Enabled)** and **new value (Disabled)**, and the **source** reflects whether the action was performed via portal or API.

This ensures full traceability of every consent change.

**Consent Activity Logs:** Displays detailed records of consent changes made by or for customers. It ensures compliance and audit readiness, provides full visibility into customer consent changes, and enable data export for reporting and governance

Each activity logs includes:

* **Timestamp** – Date and time when the action occurred
* **Customer ID** – Unique identifier of the customer
* **Consent Type** – Category of consent (e.g., Channel, Product, External App)
* **Field Name** – Specific consent item (e.g., SMS, In-App Messages)
* **Action** – Type of update (Granted or Revoked)
* **Old Value** – Previous consent status
* **New Value** – Updated consent status
* **Source** – Origin of the change (e.g., CMS website)
* **IP Address** – IP address from which the action was performed
* **Consent Proof** – Proof of change in consent preference

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (33).png" alt=""><figcaption></figcaption></figure></div>

Switch between the Customer/Admin/API Activity tabs to view the respective activity logs.

Use Search or Filter to locate the required activity logs.

You can export logs in PDF or as a CSV file for reporting and governance.

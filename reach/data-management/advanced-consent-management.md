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
  actions:
    visible: true
---

# Advanced Consent Management

**Advanced Consent Management** extends standard consent management by allowing businesses to define and enforce consent at a more granular level. Instead of managing consent only at the communication channel level (such as SMS, Email, or WhatsApp), businesses can capture and manage customer preferences across specific products, services, communication purposes, data categories, and business use cases. This enables organizations to align customer communications and data usage more closely with individual preferences and regulatory requirements.

Unlike standard Consent Management, which primarily identifies customers based on opt-in or opt-out preferences for communication channels, **Advanced Consent Management** supports purpose-based consent, category-level preferences, consent history tracking, privacy request handling, consent enforcement across integrated systems, and real-time consent updates through the Consent Management Platform (CMP). This helps ensure that every communication and data-processing activity respects the customer's latest consent preferences while supporting DPDPA-aligned consent governance.

<div align="left"><figure><img src="../../.gitbook/assets/image (126).png" alt=""><figcaption></figcaption></figure></div>

[Click here](https://help.uniservenxt.com/~/revisions/Ni2mChuLCH97NWtSyg1s/consent-management-platform-cmp/admin-console/consent-management) to know how to collect consent from users using our consent management portal.

When a customer updates their communication preferences through the consent management experience, Reach automatically updates the corresponding consent record.

Consent status is stored against each channel in the Consent Data table as:

* **1** – Opted In
* **0** – Opted Out

Reach uses the latest consent status during communication execution to ensure messages are sent according to customer preferences.

<div align="left"><figure><img src="../../.gitbook/assets/image (125).png" alt=""><figcaption></figcaption></figure></div>

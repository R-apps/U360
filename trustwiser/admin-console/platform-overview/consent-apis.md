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
  anchors:
    visible: false
---

# Consent APIs

This provides the API documentation for integrating external systems to manage consent updates, status, and details programmatically.

There are separate APIs to manage customers' consent preferences.&#x20;

**Update consent API**: This let external systems grant or revoke customers' consent through API call without using the dashboard.

**Validate Consent API:** Lets external systems retrieve a customer's current consent status across communication channels, consent categories, and data-sharing partners in a single API call.

**Privacy Center Details API:** Lets external systems retrieve a customer's consent categories, communication channels, data-sharing partners, or complete consent records for administrative and debugging purposes.

**Webhook Event Subscribers:** Lets administrators manage webhook subscribers that receive real-time notifications about consent events.

**Event Receivers (Webhooks):** Lets external systems receive real-time consent event notifications through configured webhook endpoints to synchronize consent data and trigger business processes.

**Notice Message Details API:** Lets external systems retrieve published consent notice messages for grant, revoke, display, and acknowledgement actions using a notice ID or name.

**Customer Complaints API:** Lets authenticated customers submit and track privacy complaints, reply to cases, reopen resolved complaints, and view complaint history.

**Widget Integration:** Lets developers embed published consent widgets in web pages by configuring runtime settings, URLs, and authentication.

**Mobile Widget SDK:** Lets developers integrate published consent widgets into mobile applications using the CMS widget SDK and its supported properties, callbacks, and methods.

**Update Consent API:** Lets external systems grant or revoke a customer's consent through an API call without using the dashboard.

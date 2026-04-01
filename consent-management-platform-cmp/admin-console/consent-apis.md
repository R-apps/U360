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

# Consent APIs

This provides the API documentation for integrating external systems to manage consent updates, status, and details programmatically.

There are separate APIs to manage customers' consent preferences.&#x20;

**Update consent API**: This let external systems grant or revoke customers' consent through API call without using the dashboard.

**Consent Status API**: This enable external systems can read a customer's current consent preference with a single API call.

**Consent Details API**: This API provides read-only access for all customer consents. This fetches records from the database. when API is called.

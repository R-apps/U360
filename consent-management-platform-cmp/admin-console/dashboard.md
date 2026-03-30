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

# Dashboard

The **Admin Console's Interactive Dashboard** provides a consolidated view of consent activity, system status, and compliance metrics. It helps administrators monitor how consent is captured, enforced, and updated across the platform.

Let's understand each section in this dashboard.

**Summary metrics** - display high-level indicators such as Total customers, number of active consents, revoked consents, and consent coverage. This helps you quickly access the current consent landscape.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (56).png" alt=""><figcaption></figcaption></figure></div>

{% tabs %}
{% tab title="Consent Trends" %}
**Consent Trends -** a graphical representation on how the consent status (Granted/Revoked/Updated) changes over time for different categories. This helps you identify patterns and shifts in user preferences.&#x20;

**Distribution** - displays which categories have higher or lower consent adoption.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (58).png" alt=""><figcaption></figcaption></figure></div>
{% endtab %}

{% tab title="Enforcement" %}
**Enforcement -** helps you understand how many messages were allowed or restricted based on user consent.

* _Messages Allowed_**:** Number of communications successfully sent where valid consent exists.
* _Messages Blocked_**:** Number of messages prevented from delivery due to missing consent.
* _Suppressed After Revocation_**:** Messages stopped immediately after a user revoked consent.
* _API Calls_**:** Total number of API requests processed for consent updates.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (60).png" alt=""><figcaption></figcaption></figure></div>


{% endtab %}

{% tab title="Systems" %}
**Systems -** provides visibility into privacy requests efficiency and integration performance.&#x20;

* **Privacy Requests** displays a breakdown of data-related requests (Total, Completed, Pending) along with the completion rate. This helps track how efficiently privacy requests are handled.
* **Downstream Systems** helps you monitor the status and health of all the integrated systems (external and internal) such as communication platforms, banking systems, or CRM tools. It&#x20;
  * displays the connected systems and its status (Connected or Degraded)
  * Shows sync status to indicate data alignment
  * Provides response time and last sync details for quick health checks

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (61).png" alt=""><figcaption></figcaption></figure></div>
{% endtab %}

{% tab title="Consent Types" %}
**Consent Types -** provides a summary of consent status based on user actions.

* _Total consents_ - Total number of consent records available in the system.
* _Granted -_ Number of consents where users have allowed communication.
* _Revoked -_ Number of consents withdrawn by users.
* _Updated -_ Number of consents that have been modified after initial capture.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (54).png" alt=""><figcaption></figcaption></figure></div>
{% endtab %}
{% endtabs %}

**Recent Activity** - a live feed of consent-related actions.&#x20;

* Shows actions such as grant, revoke, and update
* Includes details like customer reference, consent type, source, date, and time
* Indicates the status of each action

It helps you quickly review recent changes and track user interactions as they happen.&#x20;

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (59).png" alt=""><figcaption></figcaption></figure></div>

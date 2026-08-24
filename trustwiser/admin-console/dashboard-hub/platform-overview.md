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
    visible: false
---

# Platform Overview

Select **Open Platform Overview** to view the platform's overall activity and operational status.

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Privacy Governance Platform.png" alt=""><figcaption></figcaption></figure></div>

Let's understand each section in this dashboard.

**Summary metrics** - display high-level indicators such as, Total customers, number of active consents, revoked consents, and consent coverage. This helps you quickly access the current consent landscape.

{% tabs %}
{% tab title="Consent Trends" %}
**Consent Trends—**&#x61; graphical representation of how the consent status (Granted/Revoked/Updated) changes over time for different categories. This helps you identify patterns and shifts in user preferences.&#x20;

**Distribution** - displays which categories have higher or lower consent adoption.

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Consent Trends.png" alt=""><figcaption></figcaption></figure></div>
{% endtab %}

{% tab title="Enforcement" %}
**Enforcement -** helps you understand how many messages were allowed or restricted based on user consent.

* _Messages Allowed_**:** Number of communications successfully sent where valid consent exists.
* _Messages Blocked_**:** Number of messages prevented from delivery due to missing consent.
* _Suppressed After Revocation_**:** Messages stopped immediately after a user revoked consent.
* _API Calls_**:** Total number of API requests processed for consent updates.

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Dashboard - Enforcement.png" alt=""><figcaption></figcaption></figure></div>
{% endtab %}

{% tab title="Systems" %}
**Systems** provides a real-time overview of your privacy workflows, downstream integrations, and core technical metrics.&#x20;

Use this dashboard to track compliance performance and troubleshoot system bottlenecks.&#x20;

* **Privacy Requests** displays a breakdown of data-related requests (Total, Completed, Pending) along with the completion rate.&#x20;
  * _Total_: _The total number of privacy requests received this month._
  * _Completed_: _The number of requests successfully processed and resolved_.
  * _Pending_: _The number of requests currently in progress or awaiting action_.
  * _Completion Rate_: _The percentage of overall privacy requests completed this month._

This helps track how efficiently privacy requests are handled.

* **Downstream Systems** helps you monitor the status and health of all the integrated systems (external and internal) such as communication platforms, banking systems, or CRM tools. It&#x20;
  * displays the connected systems and its status (Connected or Degraded),
  * Shows sync status (%) - rate of data synchronized between the platform and integrated system.
  * Provides response time in milliseconds (ms), and
  * the timestamp of the last recorded sync
* **System Health Metrics** displays real-time performance indicators for the underlying infrastructure. Metrics turn <mark style="color:orange;">orange</mark> if they cross their defined operational thresholds.
  * _Consent API Latency_: The average time it takes for the API to respond to consent queries. _(Threshold: < 100ms)_
  * _Cache Hit Rate_: The percentage of requests served directly from the cache. Higher rates improve performance. _(Threshold: > 95%)_
  * _Database Connections_: The percentage of available database connections currently in use. _(Threshold: < 85%)_
  * _Webhook Success Rate_: The percentage of automated notifications successfully delivered to external systems. _(Threshold: > 99.9%)_
  * _API Error Rate_: The percentage of API requests that resulted in an error. \
    _(Threshold: < 0.1%)_

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Dashboard - Systems.png" alt=""><figcaption></figcaption></figure></div>
{% endtab %}

{% tab title="Consent Types" %}
**Consent Types**—provides a summary of consent status based on customer actions and data preferences.

Use this dashboard to track consent metrics across different categories.

* _Total consents_ - Total number of consent records available in the system.
* _Granted -_ Number of consents granted and allowed communication, along with the percentage increase or decrease compared to the previous period.
* _Revoked -_ Number of consents withdrawn by users, along with the percentage change.
* _Updated -_ Number of consent records that customers modified after initial capture.

**Consent Type Breakdown** - This section categorizes consent into specific operational areas (e.g., Channel, External App, Personal Info, Product). Click any category row to expand it and view comprehensive statistics.

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Dashboard - Consent Types (1).png" alt=""><figcaption></figcaption></figure></div>
{% endtab %}
{% endtabs %}

**Recent Activity** - a live feed of consent-related actions.&#x20;

* Shows actions such as grant, revoke, and update
* Includes details like customer reference, consent type, source, date, and time
* Indicates the status of each action

It helps you quickly review recent changes and track user interactions as they happen.&#x20;

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Dashboard - Recent Activity.png" alt=""><figcaption></figcaption></figure></div>

To export the dashboard data, select **Options** > **Export**.

To check the auto-refresh setting, select **Options**. If **Auto-refresh** is turned OFF, select **Refresh** to load the latest dashboard data. Alternatively, turn ON **Auto-refresh** to keep the dashboard data updated automatically.

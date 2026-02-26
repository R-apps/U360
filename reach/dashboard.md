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

Reach offers two different dashboard views - **Transactional (CPaaS)** and **Communication**.

One presenting the detailed reports and performance summaries of channels and aggregators, and the other is omnichannel dashboard that helps you discover instantly how your campaigns are performing.

Considering the customer analytical needs, we, Reach team, customize these dashboards with required metrics. This helps restrict users accessing detailed analytics and quick-access links based on team hierarchy and activity within the application. The Administrator selects the appropriate dashboard when assigning user permissions.&#x20;

&#x20;Here is a quick walk through of these dashboards.

**1. Transactional Dashboard**

This helps you monitor the real-time performance of CPaaS communications.

The channel summary gives you the following channel-wise metrics, enabling you to identify which channel is under performing.

**Messages Communicated**: Total number of messages received by CHUB and that submitted by aggregator. Clicking the count gives you a breakdown of requests (OTP/Transactional/Promotional).

**Top Source System**: This information is plotted in a pie-chart displaying the top-performing applications generating message traffic.

**Channel-wise Data**: This displays the channels'(SMS, Email, WhatsApp, and others) volumes over the selected time period (daily/weekly/monthly/yearly).

**Aggregator Distribution**: This Displays channel-wise communication distribution across configured aggregators. This Aggregator Health enables you monitor gateway performance and validate routing paths.

**Delivery Latency**: These charts show the time taken to deliver messages (grouped in 0–2s, 2–5s, etc.) for each channel. This helps you identify delays in delivering communications.&#x20;

**Detailed Request Report**: Filter and view specific communications based on channel, gateway, status, message id. This information is ideal for in-depth troubleshooting.

**Request Performance summary**: Tracks every stage of the communication request lifecycle from API hits and validation to DND filters, queue handling, and message delivery. This helps you identify any delays in communication deliveries.

<div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/CHUB Dashboard - Channel summary.png" alt=""><figcaption></figcaption></figure></div>

**2. Communication Dashboard**

This Dashboard simplifies campaign operations by bringing creation, monitoring, and management into one place. It gives quick access to campaigns, templates, data, calendars, and system actions without switching screens.

This dashboard lets you:

* Create campaigns instantly using any channel (SMS, Email, WhatsApp, RCS, Voice, Web Push, App Push, In App). Each option takes you directly to the campaign creation flow for that channel.
* Track recent communications along with delivery metrics including sent, delivered, opened, clicked, failed, and bounced.
* Create templates instantly&#x20;
* Upload audience or campaign data files for targeting and personalization.
* Manage Opt-In / Opt-Out effortlessly - control customer communication preferences to ensure messages are sent only to eligible users.
* Validate audience list for accuracy and readiness before launching campaigns, reducing delivery failures.
* View communication calendar that displays scheduled and executed campaigns in a calendar format. This helps you plan future communications effectively and track campaign timelines easily.
* Access other actions such as geo-fencing contacts, creating A/B experiments, surveys, download reports, and more.

<div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/Communication Dashboard (1).png" alt=""><figcaption></figcaption></figure></div>

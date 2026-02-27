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

# Live Performance Report

The "Live Performance Report" gives you real-time insights into how your gateways, load distribution, campaigns, and system are performing in real-time without having to wait for end-of-day reports.

This report helps users (marketers)

* quickly spot under-performing gateways or campaigns
* debug failed messages
* efficiently reroute traffic

Reach delivers this live analytics for each individual communication channel (SMS, WhatsApp, Email, and more), so you can make smarter decisions, instantly.

To view a channel's live performance:

* Navigate to **Analytics** > **Live Performance Report**
* Select the communication channel (SMS, Email, WhatsApp, Voice, etc.).&#x20;

The platform generates and displays the selected channel's performance report.

Let's see the live performance report for the SMS channel.

### Live Analytics

This report includes the following:

* **Gateway Delivery Summary** - helps monitor delivery success and responsiveness of a specific gateway or all the gateways.
* **Load Distribution** - displays how traffic is being distributed across different gateways. This helps in detecting overload or underutilized gateways.
* **System Performance Summary** - provides metrics like API requests, validation results, total DND counts, and others. This helps in spotting system errors or bottlenecks.
* **Gateway Performance Summary** - Visualizes message processing time ranges across gateways— critical for latency analysis and optimization.
* **Detailed Logs** - displays message ID, gateway, status, time stamps, error message, and other information that helps in debugging failed deliveries or delays in real time. Use search filters to look up a specific log.

\<IMAGE>

### Channel Performance

This gives you a real-time and historical view of how the selected channel communications are performing across different gateways and system components.

This report helps you monitor, troubleshoot, and identify gateway delays instantly at every stage. For example, a spike in > 20sec indicates latency issues.

Let's select **SMS** channel and understand the metrics in this report.

This report includes the following:

* **Gateway Performance Summary** - this data helps you track delivery latencies for your SMS campaigns across selected gateways.
* **System Performance Summary** - this data tells how your system is handling SMS communication workflows for a selected time period. This helps you spot where messages are getting stuck—whether due to DND issues, validation errors, or queue delays.
* **Gateway Delivery Summary** - This gives a day-wise breakdown of delivery metrics. Use this to compare daily performance to detect any unusual drops or spikes in delivery. To focus on the performance of a specific provider, use the Gateway dropdown to select it.

\<IMAGE>

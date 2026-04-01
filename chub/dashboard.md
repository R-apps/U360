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

The **CHUB Dashboard** provides a unified view of communication performance across channels, aggregators, and [source systems](#user-content-fn-1)[^1] - **single source of truth** for all communication activity.

This dashboard shows:

* **End-to-end message journey**\
  From request received → processed → submitted → delivered
* **Channel performance**\
  Success, failure, rejection, and response rates for each channel
* **Aggregator performance**\
  How different providers handle your traffic and their delivery health
* **Delivery speed**\
  Delivery speed using latency insights
* **Detailed logs**\
  Record-level data for tracking and troubleshooting

This real-time interactive dashboard gives you clear visibility into what is happening with every message. View, track, and improve every message you send, ensuring your communications reach users reliably and on time.

### How this Dashboard Helps?

When you send large volumes of messages across multiple channels and aggregators, it becomes hard to track message status manually. This dashboard removes that complexity by giving a single, unified view of all communication activity. Assess overall communication health in real time.

This dashboard is enabled for enterprises using Reach CPaaS services. To view, select **Dashboard** menu in Reach platform.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (79).png" alt=""><figcaption></figcaption></figure></div>

Let's explore this dashboard.

{% tabs %}
{% tab title="Channel Summary" %}
You can view these analytics for required period. Select the period and the dashboard will load the data instantly.&#x20;

**Messages Communicated**: Total number of messages received by CHUB and that submitted by aggregator. Clicking the count for each channel gives you a breakdown of requests - total number of requests received, and that of submitted, along with CHUB success rate.

View and compare the CHUB and Aggregator success rates for the requests recived for each channel.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (66).png" alt=""><figcaption></figcaption></figure></div>

Use this section to quickly identify which channels are performing well and which are underperforming.&#x20;

**Top Source System**: This information is plotted in a pie-chart displaying the top-performing applications generating message traffic for the selected channel.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (68).png" alt="" width="452"><figcaption></figcaption></figure></div>

Use this to track contribution by each system.

**Channel-wise Data**: This displays the channels (SMS, Email, WhatsApp) volumes over the selected time period (daily/weekly/monthly/yearly).

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (69).png" alt="" width="444"><figcaption></figcaption></figure></div>

Use this to analyze patterns for better planning and optimization

**Aggregator Distribution**: This Displays channel-wise communication distribution across configured aggregators. This Aggregator Health enables you monitor gateway performance and validate routing paths.&#x20;

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (72).png" alt=""><figcaption></figcaption></figure></div>

Use this to check load balancing and reliability across providers.

**Delivery Latency**: These charts shows how quickly the messages are delivered (grouped in 0–2s, 2–5s, etc.) for each channel.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (71).png" alt=""><figcaption></figcaption></figure></div>

Use this to monitor speed and identify delays in delivering communications.&#x20;

**Detailed Request Report**: This displays request-level data for deeper analysis. Filter and view specific communications based on channel, gateway, status, message id. This information is ideal for in-depth troubleshooting.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (73).png" alt=""><figcaption></figcaption></figure></div>

**Request Performance summary**: Tracks every stage of the communication request lifecycle from API hits and validation to DND filters, queue handling, and message delivery, for the selected channel.&#x20;

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (74).png" alt=""><figcaption></figcaption></figure></div>

Use it to understand system throughput and validation efficiency.
{% endtab %}

{% tab title="Source System" %}
This displays how your messages are processed and delivered across channels like SMS, Email, and WhatsApp for all or the selected source system and for selected time period.

The source system data presents the delivery latency at CHUB and Aggregators, along with the total delivery time for each communication.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (75).png" alt=""><figcaption></figcaption></figure></div>
{% endtab %}

{% tab title="Aggregator Summary" %}
This provides the performance of each aggregator configured for SMS, Email, and WhatsApp channels for the selected period.

**Aggregator Summary**

It shows the total requests came to it from CHUB, along with delivered, success, failure rates, and average latency.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (76).png" alt=""><figcaption></figcaption></figure></div>

**Aggregator Performance Summary**

This displays a graphical view of how each aggregator is performing for the selected channel based on the delivery latency.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (77).png" alt=""><figcaption></figcaption></figure></div>

**Aggregator Data**

This displays the number of requests submitted by each aggregator, along with the success and failure rates based on the latency at CHUB and Aggregator.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (78).png" alt=""><figcaption></figcaption></figure></div>
{% endtab %}
{% endtabs %}



[^1]: 

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

# SMS Profile

To set up SMS profiles, go to **Settings** > **SMS Profile.** Alternatively, press <kbd>Alt+S</kbd>&#x20;

Follow this four-step process to set up a new SMS profile, and ensure you save the configuration after each step.

{% stepper %}
{% step %}
#### Creating a new profile

* In the **SMS Settings** dialog, select **New** and give the profile unique name and select **Ok**. Then, select it from the **Profile Name**.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/Create SMS profile.png" alt="" width="563"><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
#### Configure SMS server details

In the **SMS Server Details** section:

* Select the **Protocol**
  * SMPP (Short Message Peer-to-Peer) - select this for handling speed and high volume messages, along with a technical team to set up server and analyze real-time reports. &#x20;
  * Web URL - select this for quick and lower volume messages
* Enter the **System Type** provided by your SMS aggregator.
* Enable **Global Configuration** to use it globally.
* Choose the **Bind Mode**:
  * Transmitter - for one-way, outbound messaging
  * Transceiver - for two-way communication (outgoing and incoming messages within a single connection).
* Choose the **Processing** **Mode**:
  * Synchronous – waits for delivery acknowledgment before sending the next message.
  * Asynchronous – sends messages continuously without waiting for acknowledgment.
* Enter the **IP address** and **Port number** of the SMS server.
* Enter the **User name** and **Password** to authenticate with the SMS gateway.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/SMS Profile setup.png" alt="" width="479"><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
### Define the message content

* Switch to the **Message** tab.
* Enter the **Sender Mobile Number**.

{% hint style="info" %}
If the sender number is already defined at the document level and indexed as a data object, you don’t need to enter it again for each customer.
{% endhint %}

* Type the SMS content in the **Message** area. To insert dynamic data for personalized messages, use **Meta Data**, select the required data object, and click **Insert**.
* Select **Multilingual** to localize the content.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/SMS profile name selection - Message content.png" alt="" width="449"><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
### Advanced Settings

<<mark style="color:orange;">Need sufficient info</mark>>
{% endstep %}
{% endstepper %}

Save your SMS profile configuration. The profile now appears in the **Profile Name** list.

### Applying SMS Profile

Open the **SMS Settings** dialog and select the SMS profile in the **Select Profile** fiel&#x64;**.**

Then, select **Ok** to apply.<br>


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

# Voice

Voice communications typically involve voice broadcasting. Voice campaigns use the power of spoken communication to connect with your audience in a more personalized and engaging manner. Voice technology caters to users, including those with visual impairments or limited access to written content, making it an inclusive communication channel. These campaigns can be personalized and scheduled to be sent at specific times. The platform often provides analytics to track delivery rates, CTR, and engagement, allowing you to optimize your campaigns for better results.

### Prerequisites

1. Voice message template
2. Customer data

### Steps to Create a Voice Communication

Follow these steps to create a voice campaign:

{% stepper %}
{% step %}
### Step 1: Create Communication

1. Navigate to **Communication Management** > **Voice** > **Create Communication**
2. Give the voice campaign a name and select the communication type (Schedule /Recurring/ Event/ Transaction)
3. Enter a brief description of the communication, and click **Create Communication**. The communication is created with a communication ID and directs you to the audience selection page.
{% endstep %}

{% step %}
### Step 2: Select Audience

[Click here](audience-selection.md) to understand the audience selection.

After selecting the audience, click **Save & Continue**.
{% endstep %}

{% step %}
### Step 3: Compose Message

Next, select the message type (Template/File).

For the "Template" message type:

* Click **Browse Template** to select a template. When you select a template, the application automatically populates the template type and communication message.
* Select the voice language and the available voice actor (Person voice)

However, you can personalize the message as needed. Additionally, the application provides a mobile preview of your communication message, as illustrated below.

\<IMAGE>

> The templates you see in the template repository were created by your admin. If you do not find a template closest to your needs, you can create one if you have the necessary permissions.&#x20;

To change or insert variables in a message, point to the message body and \
click **Personalize**. Select the variable to insert, as illustrated below.

\<IMAGE>

For the "File" message type:

Add a voice file in MP3 format from your local storage and select if it is a transactional message or for a contact.

Then, you can test your communication using the **Send Text** option. Enter the mobile number and run the campaign.

\<IMAGE>

After you finish configuring your campaign, click **Save & Continue**. The application saves your communication and directs you to proceed with further steps.

Based on your communication type,

* Select the communication frequency (Schedule / Frequency of occurrence / Transactional info).
* Select the SMS Mode (By default, it is set to “Single Mode”).
{% endstep %}

{% step %}
### Step 4: Communication Settings

* Select the communication settings, as shown in the illustration below:
  * **Override DND Setting** – Select this option to send SMS to customers’ contacts overriding their DND settings.
  * **Override Throttling Setting** – Select this option to set a limit on the number of SMS to send per minute.
  * **Send To Unique Contact** - Select this to send SMS to each contact individually.
  * **Override Queue Setting** – Select this option to set to ‘0’ to send your communication overriding the queue. Set the Override Queue Setting to '0' to bypass the queue and send your communication directly.
  * **Apply STO** – Select STO (Send Time Optimization) to send communications when recipients are most responsive.

\<IMAGE>

* Then, click Broadcast to send SMS to your audience and provide your confirmation in the displayed pop-up as the communication will be in draft mode. This sends communication to the selected audience.


{% endstep %}
{% endstepper %}

For “Transaction” type communications, you can schedule them and run the campaigns when required.

\<IMAGE>

### Managing Communications

To view your voice communications, navigate to **Communication Management** > **Voice** > **View**\*\* Communication\*\*. The application displays schedules and event-based communications separately. Switch between the tabs to see the corresponding communications. Furthermore, you can look for a communication by name, status, or date.

* To edit a communication, click ![](<../../.gitbook/assets/Edit icon.png>), and update it.
* To execute a communication, click ![](<../../.gitbook/assets/Play or Execute icon.png>).
* To cancel a communication, click **X**.
* To delete a communication, click ![](<../../.gitbook/assets/Delete CSV Data.png>).

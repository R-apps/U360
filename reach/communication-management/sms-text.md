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

# SMS Text

The SMS text campaign (communication) module helps you create, test, and send transactional, personalized, and targeted text messages to target audience. You can even schedule to send promotional messages at specific times.

Channel level analytics help you track delivery rates, CTR, and engagement, allowing you to optimize your campaigns for better results.

## Prerequisites

1. An approved SMS Text communication template
2. DLT (Distributed Ledger Technology) registration - a mandate step for businesses to send SMS - requiring entity, Header (Sender ID), and content template registration on telecom operator portals (like Airtel, Jio, Vodafone Idea) to prevent spam and ensure verified communication
3. Target customer data - could be either from DB, or a CSV file, or a segment of audience for marketing messages

## Steps to Create an SMS Text Communication

{% stepper %}
{% step %}
### Step 1: Create Communication

* Navigate to **Communication Management** > **SMS Text** > **Create Communication**.
* Give the campaign a name and select the communication type (Schedule /Recurring / Transaction)
* Enter a brief description of the communication, and click **Create Communication**. The communication is created with a communication ID and directs you to the audience selection page.

\<IMAGE>
{% endstep %}

{% step %}
### Select Audience

[Click here](audience-selection.md) to understand the audience selection.

After selecting the audience, click **Save & Continue**.
{% endstep %}

{% step %}
### Compose Message

* Next, select the template type (single variant or test with multiple variants using \
  [A/B testing](ab-testing.md).
* Click **Browse Template** to select a template. When you select a template, the application automatically populates the template type, header, and communication message. However, you can personalize the message as needed. Additionally, the application provides a mobile preview of your communication message, as illustrated below.\
  \<IMAGE>
* To change or insert variables in a message, point to your message body and click **Personalize**. Select the variable to insert, as illustrated below.\
  \<IMAGE>
* Further, you can add a survey, a form, or both.
* You can even test your communication using the **Send Text** option. Enter the mobile number and run the campaign.

After you configure your campaign, click **Save & Continue**. The application saves your communication and directs you to proceed with further steps.
{% endstep %}

{% step %}
### Communication Settings

Based on your communication type:

* Select the communication frequency (Schedule / Frequency of occurrence / Transactional info).
* Select the SMS Mode (By default, it is set to “Single Mode”).
*   Select the communication settings, as shown in the illustration below:

    * **Override DND Setting** – Select this option to send SMS to customers’ contacts overriding their DND settings.
    * **Override Throttling Setting** – Select this option to set a limit on the number of SMS to send per minute
    * **Send To Unique Contact** - Select this to send SMS to each contact individually.
    * **Override Queue Setting** – Select this to set to ‘0’ to send your communication overriding the queue. Set the Override Queue Setting to '0' to bypass the queue and send your communication directly.
    * **Apply STO** – Select STO (Send Time Optimization) to send communications when recipients are most responsive.

    \<IMAGE>
* Then, click Broadcast to send SMS to your audience and provide your confirmation in the displayed pop-up as the communication will be in draft mode. This sends communication to the selected audience.

For "Transaction" type communications, you can schedule them and run the campaigns when required.
{% endstep %}
{% endstepper %}

## Managing SMS Communications

To view your SMS communications, navigate to **Communication Management** > **SMS Text** > **View Communication.** The application displays schedules and event-based communications separately. Switch between the tabs to see the corresponding communications. Furthermore, you can look for a communication by name, status, or date.

\<IMAGE>

* To edit a communication, click ![](<../../.gitbook/assets/Edit icon.png>), and update it.
* To execute a communication, click ![](<../../.gitbook/assets/Play or Execute icon.png>), and to cancel, click '**x**'.
* To delete a communication, click ![](<../../.gitbook/assets/Delete CSV Data.png>).

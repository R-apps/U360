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

# WhatsApp

WhatsApp campaigns offer a direct line to users, facilitating real-time interactions. They're particularly effective for promotions, event reminders, customer support, and exclusive offers. With features like multimedia content and group messaging, WhatsApp campaigns stand out for their versatility and ability to deliver rich, engaging content seamlessly. WhatsApp campaigns excel in reaching audiences quickly and effectively, making them a valuable addition to any marketing strategy.

## Prerequisites

1. A registered WhatsApp Business Account (WABA)
2. WhatsApp template
3. Customer data

## Steps to Create a WhatsApp Communication

Follow these steps to create a WhatsApp campaign:

{% stepper %}
{% step %}
### Create Communication

1. Navigate to **Communication Management** > **WhatsApp** > **Create Communication**
2. Give the voice campaign a name and select the communication type (Schedule / Recurring / Transaction)
3. Enter a brief description of the communication, and click **Create Communication**. The communication is created with a communication ID and directs you to the audience selection page.

\<IMAGE>
{% endstep %}

{% step %}
### Select Audience

[Click here](audience-selection.md) to understand the audience selection.

After selecting the audience, click **Save & Continue**.
{% endstep %}

{% step %}
### Compose Message

Next, select the message template.

* Click **Browse Template** to select a template that suits your needs. When you select a template, the application automatically populates the template type and the communication message.
* Personalize the template as needed. Additionally, the application provides a mobile preview of your communication message, as illustrated below.

\<IMAGE>

> The templates you see in the template repository were created either by you or your admin. If you do not find a template closest to your needs, you can create one if you have the necessary permissions.

* Further, you can test your communication using the **Send Text** option. Enter the WhatsApp mobile number and run the campaign.\
  \<IMAGE>
* After you finish configuring your campaign, click **Save & Continue**. The application saves your communication and directs you to proceed with further steps.
* Next, choose whether the template needs to be reviewed. If you choose "Yes", specify the number of reviews to be done and the reviewers. Then, click **Save & Continue**.\
  \<IMAGE>
* Then, based on your communication type selection, select the event, or the transaction, or a schedule, to run the campaign.
{% endstep %}

{% step %}
### Communication Settings

* **Override DND Setting** – Select this option to send communication to customers’ contacts overriding their DND settings.
* **Override Throttling Setting** – Select this option to set a limit on the number of communications to send per minute.
* **Send To Unique Contact** - Select this to send communication to each contact individually.
* **Override Queue Setting** – Select this to set to ‘0’ to send your communication overriding the queue. Set the Override Queue Setting to '0' to bypass the queue and send your communication directly.
* **Apply STO** – Select STO (Send Time Optimization) to send communications when recipients are most responsive.

\<IMAGE>

Then, click **Broadcast** to send communication to your audience and provide your confirmation in the displayed pop-up as the communication will be in draft mode. This sends the communication to the selected audience.

\<IMAGE>
{% endstep %}
{% endstepper %}

## Manage Communications

To view your WhatsApp communications, navigate to **Communication Management** > **WhatsApp** > **View Communication**. The application displays the communications created by you to date along with their status. Expand the communication to view its stats.

Furthermore, you can choose to edit or delete these communications as required.

* To view a communication, click !\[]\(../../images/View Communication.png).
* To edit a communication, click , and update it.
* To execute a communication, click !\[]\(../../images/Run campaign.png).
* To delete a communication, click .

Executed campaigns cannot be edited.

## Analytics

To access your WhatsApp campaign reports, navigate to:

**Menu** > **Analytics** > **Communication Analytics** > **WhatsApp** > **Reports**

The application displays a summary of reports for all the WhatsApp communications made to date, as illustrated here.

\<IMAGE>

* Click ‘+’ to view the quick summary detailing requests and delivery summaries
* Click the Communication ID to view the count of requests made and a detailed summary of each request. Furthermore, you can download this report to your local storage.

To access your WhatsApp campaign reports, navigate to:

**Menu** > **Analytics** > **Communication Analytics** > **WhatsApp** > **Reports**

The application displays a summary of reports for all the WhatsApp communications made to date.

* Click ‘+’ to view its quick summary detailing requests and delivery summaries.
* Click the Communication ID to view the count of requests made and a detailed summary of each request. Furthermore, you can download this report to your local storage.

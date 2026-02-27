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

# Mail PrintPDF

Mail Print PDF communication involves generating personalized PDF documents that can be mailed to recipients as part of a campaign. These PDFs include campaign content, such as newsletters, promotional offers, or personalized letters, which are then printed and mailed to recipients.

This method is ideal for sending detailed information, invoices, contracts, or personalized offers. It is effective for official documents, legal notices, and high-impact marketing campaigns that require a professional appearance.

## Prerequisites

1. A valid and registered Email ID.
2. Message template
3. Customer data

## Steps to Create a Mail Print PDF Communication

Follow these steps to create a WhatsApp campaign:

{% stepper %}
{% step %}
### Create Communication

1. Navigate to **Communication Management** > **Mail** > **Create Print PDF**
2. Give the campaign a name and select the communication type (Schedule/Event/Recurring/Transaction)
3. Enter a brief description of it, and click **Create Communication**. The communication is created with a communication ID and directs you to the audience selection page.

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
* Personalize the template as needed. The application provides a mobile preview of your communication message, as illustrated below.\
  \<IMAGE>

> The templates you see in the template repository were created either by you or your admin. If you do not find a template closest to your needs, you can create one if you have the necessary permissions.&#x20;

* Further, you can test your communication using the **Send Text** option. Enter the email ID and trial run the campaign.\
  \<IMAGE>
* After you finish configuring your campaign, click **Save & Continue**. The application saves your communication and directs you to proceed with further steps.
* Next, choose whether the template needs to be reviewed. If you choose "Yes", specify the number of reviews to be done and the reviewers. Then, click **Save & Continue**, as illustrated below:

\<IMAGE>

Then, based on your communication type selection, select the event, or, the transaction, or a schedule, to run the campaign. Before broadcasting, select the communication settings.
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

## Managing Mail Communications

To view your mail print PDF communications, navigate to **Communication Management** > **Voice** > **View Print PDF**. The application displays the communications created by you to date along with their status. Expand the communication to view its stats.

Furthermore, you can choose to edit or delete these communications as required.

* To view a communication, click **View.**
* To edit a communication, click ![](<../../.gitbook/assets/Edit icon.png>), and update it.
* To execute a communication, click ![](<../../.gitbook/assets/Play or Execute icon.png>).
* To delete a communication, click ![](<../../.gitbook/assets/Delete CSV Data.png>).

Executed campaigns cannot be edited.

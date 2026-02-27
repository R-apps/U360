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

# RCS

RCS (Rich Communication Services) is an advanced form of mobile messaging that works inside the user’s default messaging app. Unlike traditional SMS, RCS supports **rich content** such as images, buttons, carousels, quick replies, and branded messages. It combines the reach of SMS with the experience of a mobile app.

RCS transforms messages into conversations. Customers can take action directly from the message, such as clicking a button, confirming details, or navigating to a page.

RCS channel is useful for alerts, reminders, service updates, and more.

**Example**: Credit card payment reminder - instead of plain text, it helps you show the outstanding amount, due date, include action buttons like "Pay Now", "View Statement". This helps customers act directly from the message.

### Prerequisites

1. RCS communication template
2. Target customer data - could be either from DB or a CSV file or a segment of audience for marketing messages

### Steps to Create an RCS Communication

Follow these steps to create an RCS campaign:

{% stepper %}
{% step %}
### Creating a Communication

To create a RCS communication:

* Navigate to **Communication Management** > **RCS** > **Create Communication**
* Give the new RCS communication a name, select the communication type (Scheduled/Recurring), and a brief description.

\<IMAGE>

Then, click **Create Communication**.
{% endstep %}

{% step %}
### Audience Selection

[Click here](audience-selection.md) to understand the audience selection.

After selecting the audience, click **Save & Continue**.
{% endstep %}

{% step %}
### Compose Message Content

Select the format that best fits your message:

* **Standard Template** – For simple text-based messages with actions
* **Rich Card Template** – For messages with a single image, title, and description
* **Carousel Template** – For showcasing multiple cards, such as offers or services

Choose the template based on how much visual detail your message requires.

To select the required template, use **Browse Template**. As you select, the template content is placed in the message body. The mobile preview on the right shows how the RCS message will look on a customer’s phone. This preview changes as you personalize your communication.&#x20;

\<IMAGE>

However, you can personalize it as needed.

Add Title and draft your communication message. You can personalize it by:

* inserting dynamic placeholders,
* add payment links,
* forms (allow customers to collect specific information from a customer to take an action. Use when you need customers to submit information),
* surveys (to collect opinions, preferences, or feedback, not to perform an action. Use when you want customers to share their experience), and
* interactive actions (to guide customers toward the next best step and remove confusion or effort. Customers can simply tap a button to proceed)

Here is how you can add these:

* **Dynamic data** - Place your cursor at the required position in the message and use "Personalize" option. Then, choose the variable to insert. Add as many dynamic variables as needed.\
  \<IMAGE>
* **Payment link** - To add, click Payment Link. Specify the Link URL and the parameters to be passed, so that the respective API is called when the user clicks the payment link. Once done, save it.\
  \<IMAGE>
* **Forms** - To add a form, point to your message body and click **Add Form.** Select the one to add it in your message. A form URL link gets inserted.\
  \<IMAGE>
* **Surveys** - To add a survey form, point to your message body to tell where the survey form is to be inserted and click **Add Survey**. Select a survey form from the available list. A survey form is inserted.\
  \<IMAGE>
* **Interactive actions** - Suggested Actions turn RCS messages into interactive experiences rather than static notifications. To add, click **Add Button** located beneath the message body. Specify the following for each button:
  * **Action Type** (URL/Phone/Reply)
  * **Button Text** (what the user sees)
  * **URL to open** (link or response)
  * **Suggestion Postback** (sends a predefined response back to the system, to help system understand the next follow up action)\
    \<IMAGE>

Once the message is ready, you may test using the **Test Send** option. Enter the mobile number and run the campaign.

\<IMAGE>

Post testing, revise the communication if required. Then, click **Save & Continue**. The platform saves your communication and directs you to proceed with further steps.

If your campaign needs approval, select YES and follow the approval process, else, select NO and click **Save & Continue**.
{% endstep %}

{% step %}
### Approval Process (Optional)

<mark style="color:yellow;">(Approval process step — follow your approval workflow if required.)</mark>
{% endstep %}

{% step %}
### Communication Settings

Before publishing the communication, set its preferences. To set, expand the **Advance Setting** and set the following preferences:

* **Override DND Setting** – Select this option to send communication to customers’ contacts overriding their DND settings.
* **Override Throttling Setting** – Select this option to set a limit on the number of RCS messages to send per minute.
* **Send To Unique Contact** - Select this to send this communication to each contact individually.
* **Override Queue Setting** – Set the Override Queue Setting to '0' to bypass the queue and send your communication directly, or specify the number of hours it should wait in queue (the system checks for DND and waits in queue as per IST time).
* **Apply STO** – Select STO (Send Time Optimization) to send communications when recipients are most responsive.\
  \<IMAGE>
* Then, click **Publish** to send it to the selected audience.

For "Scheduled” communications, the communication gets saved and lists under "View Communication" with the status "SCHEDULED".

To execute, click ![](<../../.gitbook/assets/Play or Execute icon.png>) to run the campaign. The platform sends the communication to the selected set of audience and marks the status as "EXECUTED".
{% endstep %}
{% endstepper %}

### Managing RCS Communications

To view your SMS communications, navigate to **Communication Management** > **RCS** > \
**View Communication.**

The application displays the communication created to date categorizing them into scheduled, event-based, recurring, and transaction. Switch between the tabs to see the respective communications.

\<IMAGE>

Further, you can look for a communication by name, status, or date.

* To edit a communication, click ![](<../../.gitbook/assets/Edit icon.png>), and update it.
* To execute a communication, click ![](<../../.gitbook/assets/Play or Execute icon.png>), and to cancel, click '**X'** .
* To delete a communication, click ![](<../../.gitbook/assets/Delete CSV Data.png>).

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

# App Notification

App notifications, also known as push notifications, are messages sent to the users mobile applications. App notifications are commonly used to notify users about new messages, updates, events, or other app-related information. As these notifications are sent even when the app is not in use or running in the background, they help to re-engage users and keep them informed.

App push notifications in REACH allow enterprises to send timely messages directly to users’ mobile applications. REACH supports both **Standard** and **Custom** push notifications, depending on the level of flexibility required.

## Prerequisites

* Client's FCM details
* SDK (Software Development Kit) should be integrated with the Client code/project
* Message template
* Customer data - for specific audience

## Steps to Create a App Push Notification

{% stepper %}
{% step %}
### Create Communication

* Navigate to **Communication Management** > **App Notification** > **Create Communication**.
* Give the communication a name and select the communication type as "Schedule".
* Select the application for which you want to send push notifications to users, and select the application type (standard/custom push notification).
  * **Standard push notification** - are pre-defined alerts sent from the app to deliver common updates such as transaction confirmations, reminders, or status changes, using a fixed format.
  * **Custom push notification** - are fully configurable messages tailored to specific user segments, events, or campaigns, allowing businesses to personalize content, timing, and actions for higher engagement.
* Enter a brief description of the communication, and click **Create Communication**.
{% endstep %}

{% step %}
### Select Audience

[Click here](audience-selection.md) to understand the audience selection.

After selecting the audience, click **Save & Continue**.
{% endstep %}

{% step %}
### Compose Content

* Next, select the communication template. For more templates, click **Browse Templates**.
* Display setting - Personalize value
* Give a title and compose your message. In the case you wish to help users access your app directly from the message, include an icon or link by selecting a resource from the available assets.

You will see a preview of your message as you begin to compose it. You can further zoom in and out of the preview as needed, and switch between collapsed and expanded views.

To conduct A/B testing, create multiple template variants by clicking '+'.
{% endstep %}

{% step %}
### Publish Communication

Finally, broadcast the communication. Broadcasting a campaign is executing it.

To run the campaign, set a schedule, select credentials, and click **Broadcast**. This goes as an app notification to the intended audience.
{% endstep %}
{% endstepper %}

## Manage App Notifications

To view created communications, navigate to **Communication Management** > **App Notification** > **View Communication**. The application displays schedules and event-based communications separately. Switch between the tabs to see the corresponding communications. Furthermore, you can look for a communication by name, date, and status.

> **Statuses:**
>
> These statuses help campaign managers and administrators track each communication's progress. This lets them monitor performance. These are the different communication statuses:
>
> _**Draft**_**:** The communication is in the early stages of creation or editing. It has not been finalized or scheduled for delivery yet.
>
> _**Schedule**_**:** The communication has been scheduled for delivery on a specific date and time in the future. It is awaiting execution.
>
> _**In Progress**_**:** The communication is currently being sent or is on its way to the intended recipients. This status indicates that communication is actively taking place.
>
> _**Processing**_**:** The communication is being processed or prepared for delivery. This status indicates that the system is actively working to send out the communication.
>
> _**Executed**_**:** The communication was successfully delivered to all intended recipients.
>
> _**Failed**_**:** The communication failed to be delivered to all intended recipients. This status indicates that an issue or error prevented the communication from being delivered. It may require investigation and remediation.

\<IMAGE>

To edit a communication, click ![](<../../.gitbook/assets/Edit icon.png>), and update it.

To execute a communication, click ![](<../../.gitbook/assets/Play or Execute icon.png>).

To delete a communication, click ![](<../../.gitbook/assets/Delete User.png>).

{% hint style="warning" %}
Executed communications are restricted from being edited or deleted.
{% endhint %}

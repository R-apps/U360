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

# In App Notification

In-app notifications are messages that appear within the app interface while the user is actively using the application. These notifications are typically triggered by user actions or events that occur within the app. In-app notifications are often used to provide contextual information, guidance, or alerts related to the user's current activity. Unlike app notifications, in-app notifications do not appear on the device's home screen and are only visible within the app interface.

Currently, the in-app notifications are available only for mobiles with Android OS.

Use communications to send in-app notifications.

## Prerequisites

* In-app notification template
* Customer data

## Steps to Create an In-App Communication

Follow these steps to create a communication:

{% stepper %}
{% step %}
### Create Communication

* Navigate to **Communication Management** > **In App Notification** > **Create Communication**.
* Give the communication a name and select the communication type (schedule/event/recurring/transaction).
* Select the target application.
* Select the application type as "Mobile App In Notification".
* Enter a brief description of the communication, and click **Create Communication**.

\<IMAGE>
{% endstep %}

{% step %}
### Select Audience

[Click here](audience-selection.md) to understand the audience selection.

After selecting the audience, click **Save & Continue**.
{% endstep %}

{% step %}
### Compose Content

Next, select the communication template and customize it. For more templates, \
click **Browse Templates**.

Include the required screen elements in your layout:

* In the Display setting, select the screen and show type (Single/Multiple time). It's recommended to have a single session.
* Design a layout for the communication.
* Style and position the close button to let users close the message.
* To let users take action from your message, place an icon inserting an image from the available resources and style it as required.
* Give a title and compose your message.
* If your communication includes multimedia, you can include an image, a GIF, or a video.
* If your message includes a carousel (image slider), add images using **Add** button and set its position (Absolute/Relative).

You will see a preview of your message as you begin to add elements and compose it.

\<IMAGE>
{% endstep %}

{% step %}
### Publish Communication

To run this campaign, set START and END dates, and click **Broadcast**. This goes as an in-app notification to the intended audience.

\<IMAGE>
{% endstep %}
{% endstepper %}

## Manage Communications

### View Communication

To view communications, navigate to **Communication Management** > **In App Notification** > **View Communication**. The application displays schedule and event-based communications separately. Switch between the tabs to see the corresponding communications. Furthermore, you can look for a communication by name, status, or date.

\<IMAGE>

To view the campaign stats, click '+', the application displays the total number of customers reached and the success rate.

\<IMAGE>

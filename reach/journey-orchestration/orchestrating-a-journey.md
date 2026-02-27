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

# Orchestrating a Journey

Let's see orchestrating a customer journey of reminding users to update their KYC before the deadline. First, communicate with users through Email, wait for 48 hrs, check if KYC is updated. If the action is still pending at the user end, send a communication through WhatsApp.

**Prerequisites**

Keep these handy before orchestrating a scenario:

* Communication templates with necessary call to actions
* User data

### Creating a Journey

To begin with:

* Navigate to **Journey Orchestration** > **Notification Journey** > **Create Journey**
* Give the journey a name and description. Then, click **Create Journey**

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/Journey Orchestration - Create journey.png" alt=""><figcaption></figcaption></figure></div>

* Initiate the flow by dragging the **Start** node.
*   **Select Users:** Select the users to who all you want to send reminders.\
    &#x20;                           To select, drag a source (**Contact Data**)\
    &#x20;   _**Node Configuration**: Use Custom Query to select the audience segment._\
    &#x20;                                      _Fetch the count and save it._<br>

    <div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/Journey Orchestration - Select Users.png" alt=""><figcaption></figcaption></figure></div>
*   **Add Communication Node**: Select the first preferred channel.\
    &#x20;                                                To select, drag the **Action** (Email) \
    &#x20;   _**Node Configuration**: Give the node a name. Specify the email sender and recipients._ \
    &#x20;                                        _Browse a template and personalize it with the required message._\
    &#x20;                                        _Check the preferred settings to deliver the communication._\
    &#x20;                                        _Preview the communication and save it._<br>

    <div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/Journey Orchestration - Node Configuration (2).png" alt=""><figcaption></figcaption></figure></div>

> \- For dynamic data, to insert variables, use **Personalise** option. Place the cursor where the dynamic data variable is to be inserted and click "personalise". Then, select the variable to be inserted.\
> \- To insert any action item or a clickable link (URL), first create a template with necessary CTAs and use them here. Always prefer using template based communications.

*   **Add Wait time**: Add a wait period to send a next reminder.\
    &#x20;                                To add, drag a Journey Control (**Delay By**)\
    &#x20;   _**Node Configuration**: Enter the wait time of 48hrs and save it._<br>

    <div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/Journey Orchestration - Add Wait Time.png" alt=""><figcaption></figcaption></figure></div>
*   **Check the KYC status:** Check the user's KYC update status. Based on decision outcome \
    (e.g., KYC done vs. not done). \
    &#x20;                                       To check, add a Condition (**campaign event**)\
    \
    &#x20;_**Node Configuration**: Select the Event for "Email" (first preferred channel)_\
    &#x20;                                        _Enter the email node id (Available in Email Node configuration)_ \
    &#x20;                                       _Select the event as "Event clicked" and specify the URL._\
    &#x20;                                       _If clicked, end the flow, else, use the fallback channel._<br>

    <div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/Journey Orchestration - Check event.png" alt=""><figcaption></figcaption></figure></div>
*   **Add Fallback Communication Node**: Based on decision outcome (if the link is not clicked)\
    &#x20;                                                              To add, drag the second preferred Action (**WhatsApp**)\
    &#x20;   _**Node Configuration**: Give the node a name._\
    &#x20;                                      _Browse a template that has CTA (Click to URL) option to add the URL._\
    &#x20;                                      _Personalize it with the required message._\
    &#x20;                                      _Check the preferred settings to deliver the communication._\
    &#x20;                                      _Preview the communication and save it._

    Lastly, add an **End** tool to complete the journey.

    Ensure all nodes are connected correctly before concluding a journey.<br>

    <div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/Journey Orchestration - Complete flow.png" alt=""><figcaption></figcaption></figure></div>

Finally, save the journey. The journey is saved and listed under "View Journey" with the status as "DRAFT".

Publish the journey to start sending communications to users.

### Publishing a Journey

To publish the journey, click **Publish Journey** and select **Start Date** and **End Date**, to schedule the journey execution. Then, click **Publish**. The journey gets published and its status changes to "SCHEDULE".

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/Journey Orchestration - Publish Journey 1.png" alt=""><figcaption></figcaption></figure></div>

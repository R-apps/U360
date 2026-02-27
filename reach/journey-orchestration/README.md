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

# Journey Orchestration

Journey orchestration lets you build personalized and customer-specific journeys.

Design, manage, automate, and optimize personalized customer experiences across multiple channels (like email, SMS, social media, websites, apps, etc.) in real time. These personalized communications ensure customers receive the right message, on the right channel, at the right moment—enhancing engagement, reducing drop-offs, and driving conversions efficiently.

Based on a customer's real-time behavior and preferences, you can:

* **Define journey triggers** based on events (e.g., form submission, missed payment).
* **Set up channel logic** using fallback and prioritization rules (e.g., Send via WhatsApp → fallback to SMS if not delivered).
* **Personalized response**: Sending customer a push notification (e.g., "Missed your morning cappuccino? Here’s 20% off your next one!")
* **Map time delays and conditions** to branch communication intelligently. (e.g., If you open the app later, a banner shows the same offer)
  * **Monitor journey flow** with visual insights on channel success, drop-off points, and conversions.

**Example**: Think of orchestrating a Smart GPS system. It:

* knows your destination (goal)
* adapts in real time to traffic (customer behavior)
* offers alternate routes (channels)
* gives timely instructions (messages)

### Journey Builder

Reach's drag-and-drop journey builder helps you orchestrate any workflow seamlessly from simple to complex. It offers the following tools to build the journey efficiently:

* **Start & Exit**: Use these tools to begin and end the flow.
* **Source (Contact/Event/FTP/CSV):** Use these tools to select the contacts to send communication.
* **Action (SMS/Email/WhatsApp/RCS/IVR/Call API/Update Attribute):** Use these tools to select the preferred communication channels.
* **Condition (Events/Switch Case/Decision/Split Audience):** Use these conditions to define fallback logic and automate decision making.
* **Journey Control (Delay/Time/Wait for event/Date):** Use these tools to control the actions involved in the journey.

A tool when dragged onto the canvas is referred to as a **Node**.

Configure these nodes after creating a flow. Conclude it with the "End" tool and you are done.

### Orchestrating a Customer Journey



{% stepper %}
{% step %}

{% endstep %}

{% step %}
### Select Users (Source)

Drag a source (**Contact Data**) node.

Node Configuration: Use Custom Query to select the audience segment. Fetch the count and save it.
{% endstep %}

{% step %}
### Add Communication Node (Email)

Drag the Action (**Email**) node.

Node Configuration:

* Give the node a name.
* Specify the email sender and recipients.
* Browse a template and personalize it with the required message.
* Check the preferred settings to deliver the communication.
* Preview the communication and save it.

Notes:

* For dynamic data, to insert variables, use the **Personalise** option. Place the cursor where the dynamic data variable is to be inserted and click "personalise", then select the variable to be inserted.
* To insert any action item or a clickable link (URL), first create a template with necessary CTAs and use them here. Always prefer using template-based communications.
{% endstep %}

{% step %}
### Add Wait Time (Delay)

Drag a Journey Control (**Delay By**) node.

Node Configuration: Enter the wait time of 48 hrs and save it.
{% endstep %}

{% step %}
### Check the KYC Status (Condition)

Add a Condition (**campaign event**) node.

Node Configuration:

* Select the Event for "Email" (first preferred channel).
* Enter the email node id (Available in Email Node configuration).
* Select the event as "Event clicked" and specify the URL.
* If clicked, end the flow; else, use the fallback channel.
{% endstep %}

{% step %}
### Add Fallback Communication Node (WhatsApp)

If the decision outcome indicates the link was not clicked, drag the second preferred Action (**WhatsApp**) node.

Node Configuration:

* Give the node a name.
* Browse a template that has CTA (Click to URL) option to add the URL.
* Personalize it with the required message.
* Check the preferred settings to deliver the communication.
* Preview the communication and save it.
{% endstep %}

{% step %}
### End the Journey

Add an **End** tool to complete the journey. Ensure all nodes are connected correctly before concluding a journey.

Finally, save the journey. The journey is saved and listed under "View Journey" with the status as "DRAFT".

Publish the journey to start sending communications to users.
{% endstep %}
{% endstepper %}



### Publishing a Journey

To publish the journey, click **Publish Journey** and select **Start Date** and **End Date** to schedule the journey execution. Then, click **Publish**. The journey gets published and its status changes to "SCHEDULE".

### View Journey

To view the created scenarios, navigate to **Journey Orchestration** > **Notification Journey** > **View Journey**.

The platform displays the list with the details - Id, Name, Created By, Journey Activation Date, Journey Status, and Action.

To edit a journey, click . Make necessary changes and save it.

To search for a specific journey, search with its name. Use the available search criteria to drill down your search (By status, Time period, and Created By) to get the desired results.

***

## Report

To view the consolidated and comprehensive reports, navigate to **Journey Orchestration** > **Notification Journey** > **Report**. The platform displays a **Journey Overview** dashboard, which provides you the details of:

* **User Engaged**: Total number of users who have interacted with at least one message or touch point within a journey.
* **Active Journeys**: Number of journeys currently running or scheduled.
* **Total Journeys**: The total number of journeys created to date.

The **Journey List** displays all the journeys created to date.

Click the journey id for channel view with detailed per-channel insights.

Expand the channel to view the Node-level metrics, which provides the detailed information about the delivery and interaction performance.

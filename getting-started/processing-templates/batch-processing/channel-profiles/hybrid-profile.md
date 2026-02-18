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

# Hybrid Profile

The **Hybrid channel** lets you deliver communications using **Email** and **SMS** together, based on a defined order and execution logic.&#x20;

Use Hybrid profiles when you want to configure one channel as a fallback or when both channels must be triggered as part of a single job, or as per the business requirement.

To set up a **Hybrid** profile, go to **Settings** > **Hybrid Settings.** Alternatively, press <kbd>Alt+H</kbd>&#x20;

Follow this two-step process to set up a new Print profile, and ensure you save the configuration after each step.

{% stepper %}
{% step %}
### Adding a new Hybrid profile

In the **Hybrid Settings** dialog, select **Add Profile**.&#x20;

Enter a unique name to the profile and configure the [SMS](sms-profile.md) and [Mail](mail-profile.md) channels switching to respective tabs.
{% endstep %}

{% step %}
### Define Execution Logic

To define the execution logic, switch to **Other Settings** tab.

In the **Communication Order** section, select to define how to send communications for a job.

* **Mail only:** Sends the communication using Email only
* **SMS only:** Sends the communication using SMS only
* **Mail and SMS:** Sends Email first, followed by SMS
* **SMS and Mail:** Sends SMS first, followed by Email

#### Secondary communication depends on primary communication

**Enable**: Enable this option to automatically enable the secondary channel to trigger communication if the primary channel fails to deliver.&#x20;

_Scenario_: If Email delivery fails, SMS is sent; ensuring the customer is informed even if one channel is unavailable.

**Disable**: Keep this option disabled when you have to trigger communication through both the channels. This combines rich content (Email) and instant alerts (SMS)

_Scenario_: Think of a bank that emails a customer’s monthly statement as a PDF and then sends an SMS to notify them that the statement has been delivered.&#x20;

This ensures customers are informed even if email access is delayed.

#### Job status update mode

Select the mode to control how job status updates are handled during processing.

* **Synchronous:**\
  UniServe 360 waits for the delivery status response before moving to the next step.\
  Recommended when accurate, real-time status tracking is required.
* **Asynchronous**\
  UniServe 360 continues processing without waiting for a response.\
  Suitable for high-volume jobs where speed is prioritized.

#### External data update configuration (Optional)

Use this section to update job or delivery status in an external database.

Configure database connectivity details in the **DB connection details**. This tells how UniServe 360 should connect to an external database.
{% endstep %}
{% endstepper %}

Finally, select **Ok** to save and apply the hybrid configuration.

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

# AB Testing

This feature in Reach helps you create two or more variants of the same communication and send them to different set of audience. Each version can differ in message content, subject line, call-to-action, or delivery timing. This setup helps you compare two or more message variants and automatically identify which one performs better before sending it to the rest of the audience.

A/B testing help you validate what resonates with users for new campaigns.

## When to Choose Single and A/B Testing

Choose **Single** when the content is final, time-critical, or already proven.

Choose **A/B testing** when you

* are unsure which message will perform better,
* want to improve engagement or response rates,
* are launching a new offer, or such other

**Example**: An insurer tests two renewal reminders - one highlighting _policy benefits_ and another focusing on _expiry urgency_. A/B testing shows which message drives more renewals before sending the winning version to the remaining customers.

## Steps to Perform A/B Testing

{% stepper %}
{% step %}
### Step 1: Creating Variants

In a new communication, after selecting your target audience, select for A/B testing instead of single message. Create two or more variants of your communication.

Then, click **Save & Continue.**

Let's understand this A/B testing with two variants.
{% endstep %}

{% step %}
### Step 2: Splitting Audience

Define how the test audience is split between the two versions. \
**Example**: 20% for Variant A and 20% for Variant B. \
These users receive different message versions for comparison.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (23) (1).png" alt=""><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
### Step 3: Wait Duration

Specify how long the system should wait before deciding the winner. This allows enough time to collect meaningful engagement data, such as clicks or responses.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (24) (1).png" alt=""><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
### Step 4: Specify Winner Variant Criteria

Next, to specify the winner variant criteria, select "**Send Winner Variant**" option and select:

*   **Event Category** - event to analyze the audience interest<br>

    <div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (25) (1).png" alt=""><figcaption></figcaption></figure></div>
*   **Event Name** - select what the event should analyze\
    \
    These event types change w.r.t. the event category.

    <div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (26) (1).png" alt=""><figcaption></figcaption></figure></div>
*   **Select Condition** - define the condition<br>

    <div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (27) (1).png" alt=""><figcaption></figcaption></figure></div>

For instance, let's set the criteria to check which variant gets highest click rate. To check,

* select the event as "Communication Event",&#x20;
* name as "Total Clicks", and&#x20;
* select the condition as "Highest".

\<IMAGE>

The system automatically triggers the communication with the winner variant.
{% endstep %}

{% step %}
### Step 5: Conflict Management

If there's a conflict resolution where both variants perform equally or no clear winner is identified, choose how the system should proceed.

* If you prefer sending the communication, select **Send Variant** and choose the variant to be communicated. Further, you may create a randomly created subset of your target audience to restrict receiving this communication. However, you can send a different variant to the controlled group. This helps you measure the true impact by comparing engaged users against a baseline. To do this, enable the **Control Group** option and specify the percentage.\
  \<IMAGE>
* If you prefer to stop the communication, select **Do not send the communication**.
{% endstep %}
{% endstepper %}

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

# Email

Email campaigns involve sending targeted messages to a specific group of contacts via email. Email campaigns are an excellent way to reach a large audience. They are ideal for communicating directly with your audience, personalizing messages, and delivering time-sensitive information. They offer flexibility in terms of content and timing. Use email campaigns, to communicate with your target audience, personalize messages, or deliver time-sensitive information.

## Prerequisites

* A business Email ID
* Approved Email template
* Validated audience data
* Configured Email Gateway (SMTP or API)
* Verified From Email Address and domain
* Consent and preferences

## Steps to Create an Email Communication

Follow these steps to create an email campaign:

{% stepper %}
{% step %}
### Creating an email communication

* Navigate to **Communication Management** > **Email** > **Create Communication**
* Give the email campaign a name and select the communication type (Schedule /Recurring/ Transaction)
* Enter a brief description of the campaign, and click **Create Communication**. The communication is created with a communication ID and directs you to the audience selection page.
{% endstep %}

{% step %}
### Audience selection

[Click here](audience-selection.md) to understand the audience selection.

After selecting the audience, click **Save & Continue**.
{% endstep %}

{% step %}
### Template Variant Selection

If you want to experiment a new communication and analyze the audience engagement, select [**A/B TESTING**](a-b-testing.md), else, select **SINGLE**.
{% endstep %}

{% step %}
### Compose Message Content

Before composing the message, specify these fields:

* **From Alias** - Enter the sender's name instead of email ID. For example, instead of using a generic “noreply@xyz.com,” you could set it to “XYZ Support Team”.
* **Reply To** - Enter the alternative email ID to receive replies. This is useful when using a noreply or generic email ID for mail-sending purposes.
* **Subject** - Enter the subject line. To insert dynamic data in the subject, click <>, and select the variable(s) to insert.
* **Pretext** - Reinforce the subject line or provide a brief overview of what the email contains.

Then, compose the email message.

#### Compose using a predefined template

To use a predefined template, click **Browse Template** and select the required one.

Then, use the drag-and-drop editor to customize it to your requirement. Right-click the element in the template to modify. Make sure to use appropriate font, style, and necessary inserts, to match your brand.

\<IMAGE>

#### Compose using Generative AI

You can even use the Gen AI feature to draft your email message. Click <>, tell the context, specify word limit, language and click **Generate**. Preview the generated template and copy it to use.

\<IMAGE>

#### Compose using HTML Code

Use HTML code to build your email template when you

* have an approved HTML email design
* need full control and advanced formatting not supported by drag-and-drop editor
* have strict layout and visual guidelines

To use HTML code feature, click <> and paste your complete HTML code into the editor. Ensure the HTML code is inline styled to avoid external CSS and responsive for mobile devices.

Then, click **Save**.

\<IMAGE>

Insert dynamic fields to personalize communications, ensuring all variables are correctly mapped to the audience data.
{% endstep %}

{% step %}
### Preview & Test

Click <> to preview the email across desktop and mobile views.

\<IMAGE>

Then, test the communication. Click  option using a working email ID.

\<IMAGE>

After testing the communication, make changes if required, else, click **Save & Continue**. The application saves your communication with a unique communication ID.
{% endstep %}

{% step %}
### Approval

This adds a control layer for regulated or high-impact communications, helping you ensure the communication is reviewed and authorized before it reaches customers. This is helpful for transactional, payment-related, regulatory, or customer-impacting communications to avoid errors.

* **Yes**: Enables the approval workflow. The communication will be sent only after approval.
* **No**: Skips approval and allows direct execution.

Select reviewer(s) and approver(s) and click **Save & Continue**.

\<IMAGE>
{% endstep %}

{% step %}
### Publish

This is the final step where you schedule and release a communication. This is where you can control timing and delivery.

* Schedule the campaign to run at a required time
* Expand **Advance Settings** to control communication delivery

Advance Settings options:

* **Test Campaign** - Marks the communication as a test. Useful for internal validation without treating it as a production campaign
* **Override DND Setting** - Select this option to bypass DND rules set by users. Bypasses Do Not Disturb rules. Typically used for urgent or regulatory messages.
* **Send to Unique Contact** - Ensures each contact receives the communication only once, even if they appear multiple times in the audience list.
* **Include Opt-Out Users** - Allows sending messages to users who have opted out. Enable this option only for critical or service-related communications.
* **Apply STO** - Applies Send Time Optimization so messages are delivered at the most effective time for each user.
* **Apply Preferred Channel** - Sends the communication through the user’s preferred channel, if configured.
* **Override Throttling Setting** – Select this option to set a limit on the number of SMS to send per minute.
* **Send To Unique Contact** - Select this to send SMS to each contact individually.
* **Override Queue Setting** – Select this to set to ‘0’ to send your communication overriding the queue. Set the Override Queue Setting to '0' to bypass the queue and send your communication directly.
* **Apply STO** – Select STO (Send Time Optimization) to send communications when recipients are most responsive.

Then, click **Broadcast** to send the communication to your audience and provide your confirmation in the displayed pop-up as the communication will be in draft mode.
{% endstep %}
{% endstepper %}

## Manage Communications

To view your email communications, navigate to **Communication Management** > **Voice** > \
**View Communication**. The application displays the communications created by you to date along with their status. Expand the communication to view its stats.

\<IMAGE>

Furthermore, you can choose to edit or delete these communications as required.

* To view a communication, click <>.
* To edit a communication, click ![](<../../.gitbook/assets/Edit icon.png>), and update it.
* To execute a communication, click ![](<../../.gitbook/assets/Play or Execute icon.png>).
* To delete a communication, click ![](<../../.gitbook/assets/Delete User.png>).

Executed campaigns cannot be edited.

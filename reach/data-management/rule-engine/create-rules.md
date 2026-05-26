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

# Create Rules

### Steps to create a rule

Before creating a rule, ensure you have the required user permissions to access the Rule Engine module.

{% stepper %}
{% step %}
#### Creating a Rule

* Go to **Rule Engine** > **Create Rules**.
* On the **Create Rule** page:
  * Enter a unique name for the rule.
  * Select the category.
  * Enter a brief summary of the rule's purpose.
  * Add a milestone if required.
  * Leave the **Rule ID** blank for the system to generate one automatically.

<div align="left"><figure><img src="../../../.gitbook/assets/image (81).png" alt=""><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
#### **Query-based Customer Data Retrieval**

Retrieve the customer data either by writing raw SQL queries or by generating queries using predefined conditions. This helps you quickly retrieve relevant information, reduce manual effort, and improve data accuracy.

In the **Data Retrieval** section:

* Select the data source.
*   Define conditions by selecting:

    * a column, such as `Policy_status`,
    * an operator, such as **Equal To**, and
    * a value, such as `Active`.

    Use **Add New Condition** or **Add New Group** to add more criteria with `AND`/`OR` logic.

<div align="left"><figure><img src="../../../.gitbook/assets/image (83).png" alt=""><figcaption></figcaption></figure></div>

* Scroll down to the **SQL Query** section to write a custom query, or select **Generate SQL from Conditions** to automatically convert your visual conditions into raw SQL code.

{% hint style="info" %}
Select **Format SQL** or press <kbd>Ctrl+Shift+F</kbd> / <kbd>Cmd+Shift+F</kbd> on Mac to check the query structure and ensure the syntax is correct and easy to read.
{% endhint %}
{% endstep %}

{% step %}
### Configure Communication Channels

Once your audience is defined, choose which communication channels — SMS, Email, or WhatsApp — the system should use to deliver the message.

To configure the channels:

* Expand the **Template Mapping** section.
* For each required channel, such as SMS, EMAIL, or WHATSAPP, click <img src="../../../.gitbook/assets/image (85).png" alt="" data-size="original"> to select your pre-configured template.

The system populates the relevant metadata, such as Reach Template ID, DLT Template ID, or Template Name.

<div align="left"><figure><img src="../../../.gitbook/assets/image (90).png" alt=""><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
### Map Template Variables

To ensure each customer receives personalized information, such as their name, account number, account ID, or other dynamic data, map the template variables to the correct data fields.

As you select the template, the system fetches the related tables and columns that store dynamic customer data.

To map customer-specific details:

* Go to the required channel and expand the **Template Variable Mapping** grid.
* Select the required column from each table.

<div align="left"><figure><img src="../../../.gitbook/assets/image (91).png" alt=""><figcaption></figcaption></figure></div>

The system replaces the dynamic variables in the template with the mapped data when it triggers communications.
{% endstep %}

{% step %}
#### Define Channel Priority

Determine the precise order in which your selected communication channels should be triggered. To define,

* Expand the **Channel Priority** section.
* Use the drop-down menus to assign numerical rankings to set the triggering sequence, where 1 represents the highest priority (e.g., setting _SMS_ to 1 and _WHATSAPP_ to 2).

<div align="left"><figure><img src="../../../.gitbook/assets/image (92).png" alt=""><figcaption></figcaption></figure></div>

The system sends communication through the highest-priority channel first and moves to the next one if needed.
{% endstep %}

{% step %}
### Configure Fallback Management

Fallback management ensures your message is safely delivered via an alternative channel if the primary channel encounters a delay or delivery failure.

* Expand the **Fallback Configuration** section.
* For your highest-priority (primary) channel, enter the maximum duration (in hours) the system should wait before skipping to the next channel.

<figure><img src="../../../.gitbook/assets/image (93).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

Review all sections on the page and then select **Create** to publish your rule. All the published rules are listed in the [View Rules](view-rules.md) page.

Click here to learn how to [execute rules](execute-rules.md).&#x20;

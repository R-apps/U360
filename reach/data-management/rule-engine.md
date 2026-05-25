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

# Rule Engine

The **Rule Engine** helps businesses automate communication decisions using configurable logic, ensuring the right action is taken at the right time.&#x20;

By creating a rule, you can extract specific customer data segments, link them to multi-channel communication templates, define channel priorities, and establish automated fallbacks if a delivery channel fails.

### How it works

* Define a rule with conditions
* Configure the action to perform when the condition matches
* The system evaluates incoming data against the rule
* If the condition is satisfied, the configured action executes automatically

The Rule Engine evaluates configured conditions and performs actions automatically when those conditions are met.

**For example**, if a bank wants to send:

* SMS alerts for transactions above ₹10,000
* Email alerts for monthly statements
* WhatsApp reminders for pending credit card payments

The Rule Engine evaluates the transaction or event and automatically triggers the appropriate communication through the configured channel.

### Steps to define a rule

Before creating a rule, ensure you have the required user permissions to access the Rule Engine module.

{% stepper %}
{% step %}
#### Creating a Rule

* Go to **Rule Engine** > **Create Rules**
* In the **Create Rule** page,&#x20;
  * enter a unique name for the rule,
  * select the category,
  * enter a brief summary of the rules' purpose, and
  * add a milestone if required.
  * leave the Rule ID blank for the system to generate one automatically

<div align="left"><figure><img src="../../.gitbook/assets/image (81).png" alt=""><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
#### **Query-based Customer Data Retrieval**

Retrieve the customer data either by writing raw SQL queries or by generating queries using predefined conditions. This helps you quickly retrieve relevant information, reduce manual effort, and improve data accuracy.

In the Data retrieval section,&#x20;

* Select the Data Source
*   Define condition(s) by selecting:

    * a column (e.g., Policy\_status),&#x20;
    * an operator (Equal To), and
    * a value (e.g., Active).

    Use 'Add New Condition' or 'Add New Group' to add more criteria with AND/OR logic.

<div align="left"><figure><img src="../../.gitbook/assets/image (83).png" alt=""><figcaption></figcaption></figure></div>

* Now, scroll down to the "SQL Query" section to write a custom query, or \
  select **Generate SQL from Conditions** to automatically convert your visual conditions into raw SQL code.&#x20;

{% hint style="info" %}
Select **Format SQL** (or press <kbd>Ctrl+Shift+F</kbd> / <kbd>Cmd+Shift+F</kbd> on Mac) to check the query structure and ensure the syntax is correct and easy to read.
{% endhint %}
{% endstep %}

{% step %}
### Configure Communication Channels

Once your audience is defined, choose which communication channels (SMS, Email, WhatsApp) the system should use to deliver the message.&#x20;

To configure,&#x20;

* Expand the **Template Mapping** section.
* For each required channel (such as SMS, EMAIL, or WHATSAPP), click <img src="../../.gitbook/assets/image (85).png" alt="" data-size="original">, to select your pre-configured template.

The system populates the respective metadata data, such as Reach Template ID, DLT Template ID, or Template Name.

<div align="left"><figure><img src="../../.gitbook/assets/image (90).png" alt=""><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
### Map Template Variables

To ensure each customer receives personalized information (such as their name, account number, account ID, or other dynamic data),

As you select the template, the system even fetches related tables and columns storing dynamic (customer-specific) data data.

To map customer-specific details,&#x20;

* Go to the channel and expand the **Template Variable Mapping** grid
* Select the required column from each table

<div align="left"><figure><img src="../../.gitbook/assets/image (91).png" alt=""><figcaption></figcaption></figure></div>

The dynamic variables in the template are replaced with the mapped data while triggering communications.
{% endstep %}

{% step %}
#### Define Channel Priority

Determine the precise order in which your selected communication channels should be triggered. To define,

* Expand the **Channel Priority** section
* Use the drop-down menus to assign numerical rankings to set the triggering sequence, where 1 represents the highest priority (e.g., setting _SMS_ to 1 and _WHATSAPP_ to 2).

<div align="left"><figure><img src="../../.gitbook/assets/image (92).png" alt=""><figcaption></figcaption></figure></div>

The system sends communication through the highest-priority channel first and moves to the next one if needed.
{% endstep %}

{% step %}
### Configure Fallback Management

Fallback management ensures your message is safely delivered via an alternative channel if the primary channel encounters a delay or delivery failure.

* Expand the **Fallback Configuration** section
* For your highest-priority (primary) channel, enter the maximum duration (in hours) the system should wait before skipping to the next channel.

<figure><img src="../../.gitbook/assets/image (93).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

Review all sections on the page and then select **Create** to deploy your rule.


---
description: Add your business logic
layout:
  width: default
  title:
    visible: true
  description:
    visible: true
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
  actions:
    visible: true
---

# Conditions & Actions

UniServe processes a template using the conditions and actions defined for it.

**Business rules** in UniServe 360 are conditions or logic that control how specific parts of a template behave. They help you decide when, how, or what content should appear based on the input data.

For example, showing a “Payment Due” message only when the outstanding amount is greater than zero.

## Conditions

In UniServe 360, conditions are defined globally and can be called at any level \
(Document / Group / Page / Layer / Object) in the Template Hierarchy by defining actions.

#### Adding Conditions

Adding a condition is a 3-step process: Add -> Define -> Configure

To add a condition,&#x20;

* Go to **Tools** > **Condition Manager**. The **Condition Definition** wizard appears.&#x20;
*   In the **Available Conditions** pane, select **Add Condition** (+). Enter the condition name and select the level (File/Level1)<br>

    <div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/image (31) (1).png" alt="" width="563"><figcaption></figcaption></figure></div>
* Next, define the condition.
  * Give the condition a unique name
  * Select the source (simple object/complex object). Based on the source selected, its datatype is auto populated.
  * Select the operator (condition)
  * Select the destination type - value (**Text**) or the data object (**Object**) and specify accordingly.
  * Enable "Evaluate always" to check this condition every time.

&#x20;    Then, select **Ok**.

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/image (32) (1).png" alt="" width="563"><figcaption></figcaption></figure></div>

The defined condition is listed under 'Available Conditions'.

To know the available list of conditions, [click here](conditions-list.md).

The defined condition is now available under "Available Conditions". Click it, the condition you defined is available in the Group1 along with the condition's expression preview.

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/image (33) (1).png" alt="" width="563"><figcaption></figcaption></figure></div>

To check with multiple conditions, you can define conditions(s) within the group by clicking '+'. \
Then select the operands (AND/OR/NOT). \
For example, to check a combination of two conditions or a single condition, define conditions to build an expression like this: \[(Condition 1 **AND** Condition 2) **OR** (Condition 3)]

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/image (34) (1).png" alt="" width="563"><figcaption></figcaption></figure></div>

Similarly, you can check a group of conditions with another group using the required operands and you can add as many conditions as required.

{% hint style="info" %}
As you define the conditions, the expression is displayed instantly. If you do not see the expression, click on the condition in the left pane to get the final expression of your condition.
{% endhint %}

After defining the condition, click **View Data** to view the sample data with the conditions applied.&#x20;

Add all the business following these steps.&#x20;

### Actions

An **action** is a business logic that tells the platform what to do when (default/conditional) a condition is met. Actions change how an object appears or behaves in the template.&#x20;

Actions can be defined at Document / Group / Page / Layer / Object level.

In UniServe 360, **pre actions** and **post actions** are part of the rule execution flow. They help you control when an action should run while the system processes the template.

**Init** - This is used to initialize a database.

**Pre Actions** - These are run to prepare the object before it appears. They are used for:

* Setting or modifying values before showing the object
* Formatting or adjusting the object based on conditions

Example: Before displaying the account balance, you can format the number, add currency symbol, replace null values with "0.00", etc.

Also, we can add rows for a process complex object on Group-level pre actions.

**Post Actions** - These are run to perform follow-up tasks after the object appears. They are used for:

* Updating other objects based on what was displayed
* Triggering additional calculations or formatting

Example:  After the transaction table is rendered, you can calculate and display the total debit/credit.

#### Defining Actions

Go to **Settings** > **Distributive Options** > **Define Actions** tab.

* **Action Type - Init**\
  If the template includes fetching data from an external data source, use "Init" action. \
  Click '+', select the condition, and set it True/False as per the requirement. \
  <\<IMAGE>>\
  Now, define the action to be performed. To define,&#x20;
  * select the Action Type,
  * Define the parameters if required and&#x20;
  * Execution Mode (_Continue_ - performs action and proceeds further / _Break_ - performs action without proceeding further)

&#x20;        Similarly, define necessary pre and post actions to be performed.

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/image (35) (1).png" alt="" width="563"><figcaption></figcaption></figure></div>

#### &#x20;Reordering Actions&#x20;

The **Reorder Actions** feature allows you to change the execution sequence of actions configured. Use this feature when multiple actions are defined and you need to control the order in which they are executed.

First add all required actions and then drag to reorder them to match the intended business flow. This approach is faster and easier than re-creating actions in the exact execution sequence.

> Reordering changes only the execution sequence of actions. The action configuration and parameters remain unchanged.

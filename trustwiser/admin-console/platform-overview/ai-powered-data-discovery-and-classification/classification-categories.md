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
  actions:
    visible: false
  anchors:
    visible: false
---

# Classification Categories

The **Classification Categories** page lets administrators define how the platform identifies and classifies sensitive data. You can create categories based on the type or nature of data, assign a sensitivity level, associate regulations, and define a confidence threshold for classification.

Each category can contain one or more **classification rules**. Rules specify the patterns, keywords, data types, or other criteria the platform uses to identify data that belongs to the category. You can also configure data protection settings for a rule, where supported, to specify whether identified data should be considered for masking or encryption.

Together, **categories** and **rules** provide the criteria the platform uses to identify, classify, and assess sensitive data across connected data sources.

Configured categories are displayed as cards with the following details:

* **Sensitivity level** – Indicates how sensitive the data identified by the category is, such as _Confidential_, _Restricted_, or _Top Secret_.
* **Regulations** – Shows the regulatory frameworks associated with a category.
* **Confidence threshold** – Defines the confidence level required for a rule to identify data as belonging to the category.
* **Classification rules** – View the rules configured under each category and the criteria used to identify matching data.

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Classification Categories.png" alt=""><figcaption></figcaption></figure></div>

### Adding a Classification Category

Select **Add Category** to create a category for a specific type of data.

* Enter a **Name** for the category.
* Enter a **Description** to explain the type of data covered by the category.
* Select the [**Sensitivity Level** ](#user-content-fn-1)[^1]\(Public / Internal / Confidential / Restricted / Top\_secret)
* Enter the [**Confidence Threshold**](#user-content-fn-2)[^2]. (<mark style="color:$info;">Min Threshold: 0.7</mark>)
* Add the applicable [**Regulation Tags**](#user-content-fn-3)[^3].
*   Finally, select **Create**.<br>

    <div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Classification Categories - Add Category.png" alt=""><figcaption></figcaption></figure></div>

The new category is added to the list of classification categories.

Click the category to view the rules associated with it.

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Classification Categories - View Rules.png" alt=""><figcaption></figcaption></figure></div>

### Adding a Rule

A **classification rule** defines the criteria used to identify data that belongs to a classification category.

* Select **Add Rule**.
* Enter a **Name** and **Description**.
* Enter the required or matching **Keywords**&#x20;
* Enter a **Regex Pattern**, if required.
* Select the **Match Operator** to determine how multiple conditions are evaluated.
* Specify the possible **Data Types.**
* Enable **NLP Detection**, if required.
* Enable **AI Detection** to configure any additional detection criteria for the rule.
* Select **Next**.
* Configure **Data Protection**, if required. This lets you specify whether identified data should be assessed for protection through masking or encryption. To add,
  * Enable **Assess Data Protection** to assess the identified data for protection.
  * Select the required **Protection Controls**, such as:
    *   **Masking -** replaces or hides part of the identified data to limit exposure while retaining the required information format.

        You can select a **Masking Strategy** and provide the required **Masking Pattern**, based on the available options.
    *   **Encryption -** protects identified data by converting it into an encoded form that requires the appropriate method to access.

        Select the required **Encryption Method** from the available options.
  * Select the **Assessment Severity:**
    * _**Low**_ – Limited concern or impact; routine follow-up may be sufficient.
    * _**Medium**_ – A notable concern that may require corrective action.
    * _**High**_ – A significant concern that requires prompt attention.
    * _**Critical**_ – A severe concern that may require immediate action.
  * Select **Create** to save the rule.

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Classification Categories - Add Rule.png" alt=""><figcaption></figcaption></figure></div>

The configured rule is then available under rules list for the selected category.

### Manage categories and rules

Use the actions available for each category or rule to maintain the classification configuration.

* Select **Edit** (![](<../../../../.gitbook/assets/Edit Icon.png>)) to update a category or rule.
* Select **Delete** (![](<../../../../.gitbook/assets/Delete Icon.png>)) to remove a category or rule that is no longer required.
* Open a category to view and manage the rules associated with it.

<mark style="color:$warning;">**Queries**</mark><mark style="color:$warning;">:</mark>

1. <mark style="color:$warning;">What does Assessment Severity represent, and what factors determine each severity level?</mark>&#x20;

[^1]: Indicates the sensitivity assigned to data identified under the category.

[^2]: Determines the minimum confidence level required for a classification rule to identify data as belonging to the category.<br>

    A higher threshold can require a stronger match before data is classified under the category.

[^3]: These are institutional frameworks and laws established by governments to govern specific industries, protect consumers, ensure data privacy, and maintain cybersecurity standards.

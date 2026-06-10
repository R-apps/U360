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
    visible: true
---

# Consent Management

**Consent Management** allows you to identify customers based on their communication preferences and consent status across supported channels. You can create consent-based queries using customer data and communication channels to retrieve records that have either opted in or opted out.

This feature helps ensure that communications are sent only to customers who have provided the required consent for a specific channel.

#### Create a Consent Query

To create,

* Go to **Data Management** > **Consent Management** > **Create Query**
* Enter a unique name for consent query and a brief description
* Select one or more channels (as per the business requirement)
* Use the **OPT-IN/OPT-OUT** toggle to specify the consent status

**Define Query Conditions**

* From **Data Source**, select the customer data table to use for the query.
* Select a field from the data source.
* Select the required operator.
* Enter the comparison value.
*   To add multiple conditions:

    * Select **AND** when all conditions must be satisfied.
    * Select **OR** when any condition can be satisfied.

    Select **+ Add** or **Add New Condition** to create additional conditions.

combine multiple conditions to create more targeted consent queries.

After configuring the query, select **View Count** to view the number of records that match the selected consent criteria and conditions.

<div align="left"><figure><img src="../../.gitbook/assets/image (121).png" alt=""><figcaption></figcaption></figure></div>

**Execute the Query**

Select **Execute** to process the consent query and retrieve the matching customer records.

Select **Download** to export the query results for analysis, auditing, or operational use.

{% hint style="info" %}
Alternatively, you can use the [**Advance Consent Management** ](advanced-consent-management.md)to collect preferences and updated them in real-time.
{% endhint %}

#### Manage Consent Queries

The **View Consent Queries** page displays all consent queries created and executed within the system. Use this page to review previously executed queries, rerun existing configurations, modify query criteria, or remove queries that are no longer required.

Go to **Data Management** > **Consent Management** > **View Queries**

* **Search & Filter queries:** Enter the query name in the search box and select the date range, to find a specific consent query
* **Edit Query:** To modify an existing query, select **Edit** (![](<../../.gitbook/assets/image (122).png>)) and update the query as required.
* **Delete Query**: To delete a query that is no longer required, select **Delete** (![](<../../.gitbook/assets/image (123).png>)).&#x20;

{% hint style="info" %}
Even if a query is deleted. previously executed consent records and audit information remain available.
{% endhint %}

<div align="left"><figure><img src="../../.gitbook/assets/image (124).png" alt=""><figcaption></figcaption></figure></div>


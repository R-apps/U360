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

# Enterprise Connectivity

This provides a central place to connect and manage the organization's data sources, connectors, and event subscribers. Data sources can be configured for databases, files, APIs, and supported business applications so that the platform can access data for discovery and analysis. It provides a single view of the configured connections, making it easier to review and maintain the systems connected to the platform.

To access, navigate to **Platform** > **Enterprise Connectivity**.

### How it helps

Enterprise Connectivity helps administrators:

* Centralize connections to data sources and enterprise systems.
* Connect different types of data sources from a common interface.
* **Maintain connection details** for configured sources.
* Verify connections before saving them.
* Prepare data sources for discovery and analysis by establishing the required connectivity.

{% tabs %}
{% tab title="Data Sources" %}
This lists the data sources configured for the organization. Each data source displays its source type and basic configuration details. You can add a new data source or edit or delete an existing one.

The platform supports different types of data sources, including:

* **Database** – for relational databases.
* **NoSQL Database** – for NoSQL databases.
* **Cloud Database (DBaaS)** – for cloud-hosted databases.
* **EDW (Enterprise Data Warehouse)** – for enterprise data warehouses.
* **API (SOAP/REST)** – for services through supported APIs.
* **File** – for file-based sources.
* **CRM** – for customer relationship management systems.
* **BPM/Workflow** – for business process or workflow systems.

#### Adding a New Data Source

To add a new data source, in select **Add Data Source** the **Data Sources** tab, and follow these steps:

{% stepper %}
{% step %}
**Step 1: Basic Information**

* Select the data source type you want to connect.&#x20;
* Enter a name to identify the data source and a brief description of it.
* Select the environment associated with the source and select **Next**.

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Add Data Source - Step 1.png" alt="" width="563"><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
**Step 2: Data Source Configuration**

* Now, to configure, enter the connection details required for the selected source or integration. The fields displayed in this step depend on the source type you selected.
* Then, select **Next**.

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Add Data Source - Step 2.png" alt="" width="563"><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
**Step 3: Verify the Connection**

Select **Test Connection** to verify the connection details before you save the data source. The platform validates and displays a confirmation message if the connection is successful.

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Add Data Source - Step 3 (final).png" alt="" width="563"><figcaption></figcaption></figure></div>

Then, select **Save** to save the data source connection.

The added data source is then listed on the **Data Sources** tab. These data sources are tagged with the selected data source type and subtypes if applicable.
{% endstep %}
{% endstepper %}

#### Manage Data Sources

Use the actions available on each data source card to maintain the configured connections.

* Select **Edit** (![](<../../../.gitbook/assets/Edit icon (1).png>)) to update the data source configuration.
* Select **Delete** (![](<../../../.gitbook/assets/Delete User.png>)) to remove a data source that is no longer required.


{% endtab %}

{% tab title="Connectors" %}
A **connector** defines how the platform interacts with a configured data source to perform a specific operation.

Where the **Data Source** identifies the system or repository being connected to, the **Connector** establishes the mechanism for interacting with that source, and **Child Operations** define the specific actions to perform through the connector.

> **For e.g.,**
>
> **Data Source:** CRM system\
> **Connector:** CRM connector configured for that system\
> **Child Operations:** Read customer details, retrieve consent status, or update a record

The connector wizard guides you from basic configuration through testing and activation, helping you verify the operation before it is made available for use.

To access, navigate to **Platform** > **Enterprise Connectivity**, and select **Connectors** tab.&#x20;

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Connectors tab.png" alt=""><figcaption></figcaption></figure></div>

#### Adding a Connector

To add a connector, select **Add Connector** and follow these steps:

{% stepper %}
{% step %}
**Step 1: Basic Information**

* Select **Add Connector** in the **Connectors** tab.
* Enter a name to identify the connector and a brief description of it.
* Select the data source with which the connector should associate with.
* Select whether the connector is used to **Read** or **Write** data or **Both**.
* Set the connector status, and then select **Next.**

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Add Connector - Step 1.png" alt="" width="563"><figcaption></figcaption></figure></div>

The next steps depend on the selected data source and action.

Let's look at the steps involved in adding a connector to a database-based data source.
{% endstep %}

{% step %}
**Step 2: Configure the Data Access Details**

To define how the connector should read the data, select an option - table / view / custom SELECT query / stored procedure / function.  Depending on this selection, the next steps vary.

For "Table", search and select the schema and the required table. Then, select **Next**.

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Add Connector - Step 2.png" alt="" width="563"><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
**Step 3: Configure Request & Response Parameters**

Define the parameters required to perform the operation and handle its response.

* **Request parameters:** To define the request parameters, select the column, data type, and select 'Req' if it's a mandatory param to be passed.\
  Add more parameters as required.
* **Response parameters:** Response parameters define the fields returned by the operation. Add response parameters manually or refresh them from the data source.&#x20;

After configuring the required parameters, select **Next**.

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Add Connector - Step 3.png" alt="" width="563"><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
**Step 4: Test Connector**

Enter sample values for the configured input parameters and test the connector.

* Enter the required input values.
* Select **Test**.
* Review the test result.

A successful test confirms that the configured operation can be executed with the provided values.

Select **Next** after completing the test.

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Add Connector - Step 4.png" alt="" width="563"><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
**Step 5: Review and activate**

The final step displays a summary of the connector configuration, including the configured operation and parameters.&#x20;

Review the details to make sure that the configuration is correct.

Select **Save & Activate** to save the connector and activate it. The connector is then available under the **Connectors** tab.
{% endstep %}
{% endstepper %}

#### Connector Status

The connector can have different statuses based on its current state. The available statuses are:

* **Draft** – The connector configuration is being created or has not yet been activated.
* **Active** – The connector is available for use.
* **Disabled** – The connector is not currently active.
* **Testing** – <mark style="background-color:$warning;">The connector is being tested.</mark>
* **Error** – <mark style="background-color:$warning;">The connector has encountered an error.</mark>

#### Manage Connectors

All the configured connectors are listed in the **Connectors** tab. You can either search for a connector by its name or filter the view by selecting a data source type.

Connectors are displayed as cards with their active status, health status, connector source and environment and a few options to manage it.

* Select **Test connection** (![](<../../../.gitbook/assets/Test Connection Icon.png>)) to test the connector.
* Select **Edit** (![](<../../../.gitbook/assets/Edit Icon.png>)) to edit a connector's configuration.
* Select **Clone** (![](<../../../.gitbook/assets/Clone Icon.png>)) to create a copy of an existing connector, including its configuration. Use this option to create a similar connector with minor changes.
* Select **Enable** (![](<../../../.gitbook/assets/Enable Icon.png>)) to use the connector. To disable, select **Disable** (![](<../../../.gitbook/assets/Disable Icon.png>)).&#x20;
* Select **Delete** (![](<../../../.gitbook/assets/Delete Icon.png>)) to delete a configured connector.
{% endtab %}

{% tab title="Event Subscribers" %}
Use Event Subscribers to share relevant consent and privacy events with connected systems in real time.&#x20;

This page provides a central place to register external systems, define the events they should receive, configure authentication, and manage their active status. While registering, configure [web hook](#user-content-fn-1)[^1] endpoint URLs to enable external systems to receive real-time events such as consent updates, withdrawals, and more.

Subscribers are displayed in cards with the following information:

* **Subscriber name**, to identify the external system.
* **Visibility** indicates whether the subscriber is visible in the configured environment.
* **Authentication** – Shows the authentication method configured for the subscriber, such as Bearer token, API key, or None (No authentication).
* **Health Score** – Indicates the completeness and compliance of the subscriber configuration on a scale of 100. A subscriber that has not been assessed is shown as "Not Assessed".
* **Consent events** – Shows the events configured for the subscriber, such as Granted, Revoked, Updated, and Deleted.
* **Active status** – Indicates whether the subscriber is currently enabled.

#### Adding a Web Hook

* Select **Add Web Hook**
* Enter the **Subscriber Name** (to identify external system) and **Description** (a short detail of external system's role)
* Specify the API **Endpoint URL** through which we consent events will be sent to the external system.
* Select the **Consent Event(s)** that we pass through the specified Endpoint URL.
* Next, select the **Authentication Type** to secure the communication and the **Authentication Value** to authenticate requests.
* Keep the subscriber status "Active" to send consent events uninterruptedly. You can disable when you want to stop communicating external systems.

> Alternatively, you can find and pick a default event subscriber from the right pane and specify how we send consent events to them.

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/image (13).png" alt="" width="544"><figcaption></figcaption></figure></div>

Then, select **Add Web Hook**.&#x20;

Configured external systems are labelled with the consent events (that you are passing through its endpoint URL) and the authentication type for easy identification. \
The **Health Score** indicates the completeness and compliance of the subscriber configuration out of 100. A subscriber that has not yet been assessed is displayed as "Not Assessed."

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Enterprise Connectivity - Event Subscribers.png" alt="" width="563"><figcaption></figcaption></figure></div>

#### Manage Event Subscribers

After a subscriber is added, you can manage it from its card.

* Use the **Active** toggle to enable or disable the subscriber.
* Select **Edit** to update its configuration.
* Select **Delete** to remove the subscriber.
{% endtab %}
{% endtabs %}

<mark style="background-color:$warning;">**Queries:**</mark>

1. <mark style="background-color:$warning;">How the data sources are tagged? - for some, it is showing as "no schema selected". And for some, it is showing the access permissions to various roles like admin, config, local, etc.</mark>&#x20;
2. <mark style="background-color:$warning;">**Connectors:**</mark>&#x20;
   1. <mark style="background-color:$warning;">Are connectors required to perform operations on a configured data source?</mark>
   2. <mark style="background-color:$warning;">Add Connectors > Step 1: how the different status impacts the connector's usage? Is there any default status? Does the status changes automatically in any circumstances like the</mark> \ <mark style="background-color:$warning;">data source unavailability?</mark>



[^1]: A webhook receiver is an external system endpoint that receives notifications when selected events occur.

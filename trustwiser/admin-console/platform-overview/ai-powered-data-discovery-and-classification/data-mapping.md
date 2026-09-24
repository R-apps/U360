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

# Data Mapping

The **Data Mapping** page helps you identify relationships between data stored across connected data sources. It helps administrators identify related data, review matched and unmatched records or columns and examine the confidence of the identified matches.

Create a mapping by selecting a primary data source and key columns, configure how records should be matched, and run the mapping against one or more data sources. The results show the relationships identified between columns, helping you understand where related data is stored across your systems.

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Data Mapping.png" alt=""><figcaption></figcaption></figure></div>

### Create Mapping

* Select **Create Mapping**.
* In **Basic Information**, enter the **Mapping Name** and **Description**.
* In **Primary Identifier Configuration**, select the **Primary Data Source, Schema, Table,** and **Primary Column (Key Column)**
* Specify the **Match Key Columns** to identify corresponding data in other sources.
* In **Advanced Settings**, configure the:
  * **Sample Size** – Define the amount of data considered for matching.
  * **Confidence Threshold** – Define the minimum confidence required for a match.
* Enable **Value-Based Matching**, where required, to compare data values when identifying matches.
* Enable **Partner-Name Matching**, where required, to identify matches based on partner or related names.
* Select **Save Mapping**.

> **Note:** The available configuration options may vary based on the selected data source and the platform configuration.

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Data Mapping - Create.png" alt=""><figcaption></figcaption></figure></div>

The mapping is created and appears on the **Data Mapping** page.

### Run a data mapping

After creating a mapping, you can run it against the available data sources.

* Point to the required data mapping and select **Run**.
* In the **Run Mapping** window, select&#x20;
  * All data sources, or
  * The specific data sources you want to scan.
* Select **Run Mapping**.

The platform processes the selected sources using the configured mapping and records the result.

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Data Mapping - Run Result (1).png" alt=""><figcaption></figcaption></figure></div>

### View Mapping History

Select **History** for a mapping to view its previous runs.&#x20;

Open a completed mapping run to review the identified relationships. The history shows information such as Run ID, Run date, Duration, Status, Number of tables processed and Total rows processed.

Select **View** for detailed result, which provides information such as:

* Number of data sources included in the run
* Number of matches identified
* Match confidence
* Number of unmatched items
* Relationships identified between columns

The **Relationship Mapping View** provides a detailed view of the relationships identified during the mapping run.

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Data Mapping - Execution History.png" alt=""><figcaption></figcaption></figure></div>

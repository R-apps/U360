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
    visible: true
---

# Discovery & Classification

The **Discovery & Classification** page lets you scan connected data sources to identify data columns and classify them using the configured classification rules. This page provides a central view of classification activity across data sources, including the last run time, the number of classified columns, and access to previous run details.

You can run classification for individual data sources or across all available sources. Individual and bulk classification runs helps you understand what data they have, identify information that may require additional protection, and monitor classification coverage across connected systems.

During a classification run, the platform examines the available tables, columns, and sample data to identify and classify information using your configured classification categories and rules. You can also enable AI classification to analyze columns that remain unclassified after rule-based checks.

**History** lets you review previous runs to monitor classification activity and identify sources that may need attention. The page also indicates when a data source has not been scanned or when classification functionality is not yet available for that source.

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Discovery &#x26; Classification.png" alt=""><figcaption></figcaption></figure></div>

### Run classification for an individual data source

Use this option when you want to classify data from a specific source.

To run classification for a single data source:

* Locate the data source you want to scan and select **Run**.
  * Review the data source details, including the source type, schemas, configured categories, and rules.
  * Under **Data consideration**, configure how many sample rows the platform should read from each table or file. The default is 10 rows per table or file.
  * Enable **AI Classification** if you want the platform to use AI to classify columns that remain unclassified after rule-based checks. The AI service uses the available category descriptions, keywords, and regular expressions to identify potential matches. High-confidence matches are applied to the results.&#x20;
  *   Select **Confirm & Run** to start the classification process.

      <div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Run Classification.png" alt="" width="410"><figcaption></figcaption></figure></div>
*   The platform starts the classification run for the selected data source. You can monitor its progress. Select **Run in Background** to continue working while a classification run is in progress. When the run completes, the platform sends an email notification with a summary of the results to your registered email address.<br>

    <div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Run Classification - In progress.png" alt="" width="395"><figcaption></figcaption></figure></div>

    <div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Run Classification -Completed.png" alt="" width="563"><figcaption></figcaption></figure></div>
*   Select **View Results** to review the results.<br>

    <div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Run Classification - Run results.png" alt="" width="563"><figcaption></figcaption></figure></div>

    The results page provides a summary of the classification run, including:

    * **Total Tables** – The number of tables examined.
    * **Total Columns** – The total number of columns examined.
    * **Classified** – The number of columns that received a classification.
    * **Unclassified** – The number of columns that do not have a classification result.
    * **Classification coverage** – The percentage of columns classified during the run.

    The results are grouped by classification category, such as Personal Identification Information (PII), Contact Information, Financial Information, Authentication & Security Information, and Demographic Information.

    Select a category to review the columns classified under it. You can also view all categories or filter the results to focus on AI-based matches.

Use the search field to find specific columns.

Use **Export Classification Report** or the available **Export** option to export classification results. Depending on the export option, you can download the results in CSV, Excel, or PDF format.

#### Adding a field from classification

The clasification report facilitates you to create a field from a classified database column and configure it for use in the Privacy Center. helps connect the information identified during classification with the fields used for privacy management.&#x20;

For example, consider the classified report has a database column - `recipient_user_id`. \
You can add this column as a field named `RECIPIENT_USER_ID` and configure its properties, customer visibility, and data mapping.

To add a field,

*   Select **Add Field** against a column in the Classification Report. The field details are prefilled using the selected column's information.<br>

    <div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Add Field - Prefilled data.png" alt="" width="563"><figcaption></figcaption></figure></div>
*   Select the business object and data category, and define the field name, description, and field type. Configure whether the field is visible, sensitive, editable, or deletable by customers.<br>

    <div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Add Field - Configure field details.png" alt="" width="517"><figcaption></figcaption></figure></div>
*   Select the data source, connector, and response parameter to specify how the field's current value can be retrieved.<br>

    <div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Add field - Map datasource.png" alt="" width="452"><figcaption></figcaption></figure></div>
* Select **Create Field** to create a field in the privacy center with the configured data.

#### Schedule an automatic classification run

You can schedule classification runs to automate the process of scanning a data source. This helps keep classification results updated without requiring you to start every run manually.

To schedule a classification run:

1. Navigate to the data source and select the **Schedule** (![](<../../../../.gitbook/assets/Schedule Run icon.png>)) icon.
2. Toggle to enable the **Automatic classification** and select a scheduling option from the displayed list of scheduling options.
3. Save the schedule.

The platform runs classification according to the configured schedule.

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Run Classification - Schedule.png" alt="" width="480"><figcaption></figcaption></figure></div>

### Run classification for all data sources

Use this option to run classification across all supported data sources in a single action.

To run classification across all available data sources:

* Select **Run All Data Sources**.
* Follow the prompts to start the classification process.
* Review the results after the runs complete.

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Run All Data Sources  - all in one.png" alt="" width="563"><figcaption></figcaption></figure></div>

### View classification history

Use classification history to review earlier runs and track classification activity over time.

To review previous classification runs, select **History**.

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Classification - Version History.png" alt="" width="563"><figcaption></figcaption></figure></div>

Select a version to view its detailed report.

#### **Compare classification versions**

You can compare any two versions of an individual data source's classification history to identify differences between their results.

* Select the two versions you want to compare.
* Select **Compare**.
* Review the differences between the selected versions. You can view the combined results or the full results for further analysis.

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Classification - Compare versions.png" alt="" width="563"><figcaption></figcaption></figure></div>

#### **Delete classification versions**

You can delete versions that are no longer required. Review the selected version before deleting it.

<mark style="color:$warning;">Queries:</mark>

* <mark style="color:$warning;">Can we identify AI-based matches in the classification results?</mark>
* <mark style="color:$warning;">Do we have an option to filter the results to focus on AI-based matches?</mark>

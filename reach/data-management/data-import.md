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

# Data Import

Data Import is the process of uploading structured data into Reach using CSV/XLSX/TXT files or an API. This data becomes the foundation for sending targeted communications across channels - SMS, Email, RCS, WhatsApp, Voice, and other.

Data import helps you:

* Store customer details in a centralized system
* Personalize messages using customer-specific information
* Create accurate audience segments

Options available to enable users to import customer data seamlessly from various sources:

#### **1. File upload**

* Go to **Data Management** > **Import** > **Data** **Import**
* In the **File Upload** tab:
  * Select the file format (CSV/XLSX/TXT). For CSV files, select the delimiter (Comma, Tab, Semicolon, Pipe)
  * Select **Choose File** and select the file to upload. After uploading, Reach displays a preview of the records.
  * Verify the displayed data and click **Submit Data** to complete the import.

The platform stores the uploaded data in its default data source.

The imported data will then be available for segmentation and campaign execution.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/Data Import.png" alt=""><figcaption></figcaption></figure></div>

To select a column to use in the report, use "**Advance Option**". Select the column and save.

Similarly, upload the consent, exclusion list, and the dynamic attachment files.

> While uploading:
>
> * the consent, make sure the file includes the **Audience ID** and **Country Code**.
> * a dynamic attachment, make sure the **File path** and **Customer ID** are included.
> * an execution list, make sure the file includes the **Campaign\_Category** column.

#### **2. Schedule Import Setting**

The **Schedule Import Setting** allows you to set up recurring data imports to keep your records up to date. Use this option when your data changes regularly and needs to stay in sync without manual effort.

For any data type (Contact Data, Transactional Data, Preference Data, or Consent Management), existing records remain unchanged. Only new records from the imported file are added to the existing table. This approach prevents data duplication and maintains data integrity.

{% stepper %}
{% step %}
### Select Data Type and Manage Tables

To view records in an existing table, click **View Tables** and select a table from the displayed list. As you select, the records in it are displayed. If any of the displayed column(s) contain Personally Identifiable Information (PII), select the "is PII" option for those columns.

You can add new tables too. To add, click **Add New Table** and:

* Enter a unique table name, and
* Define the table headers. Add headers in either way:
  * If they are readily available, select **Upload Headers** and upload the file.
  * Else, select **Add Headers** option and add the table headers manually. Use **Add** to add more headers.

By default, each newly added header is marked as a **Primary Key**. Ensure you select the correct primary key for faster data retrieval. If any field(s) contains PII, enable **Is PII** option.

Then, click **Next** to move to the next step.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/Data Import - Schedule Import Setting.png" alt=""><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
### Add the file directory

Enter the file path and select the file type. Then, click **Next** to continue.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/Schedule Import Setting- Step2.png" alt=""><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
### Schedule the import

Select the date and time to start the file import and choose the import frequency.

If required, enable the following options:

* Receive updates when duplicate primary keys are detected
* Import only files that contain headers
* Skip mandatory fields that contain blank values

Finally, click **Save** to save your schedule import settings.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/Schedule Import Setting- Step3.png" alt=""><figcaption></figcaption></figure></div>

After saving, the scheduled import runs automatically and keeps your data consistently updated.
{% endstep %}
{% endstepper %}

#### **3. APIs for real-time communications**

This helps you to import the uploaded client data using an API.

A sample API request with the API method, end-point URL, a sample request and responses are available for your reference.

To use this reference request, use **Copy To Clipboard** option.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/Data Import - APIs.png" alt=""><figcaption></figcaption></figure></div>

To view the data uploaded, [click here](view_data.md).

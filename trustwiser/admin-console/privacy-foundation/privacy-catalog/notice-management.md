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

# Notice Management

Notice Management lets you create and manage reusable privacy notices for customer consent, read confirmation, and information display. You can configure the notice type, write customer-facing content, and track the notice's approval status and version.

The summary cards display the total number of notices, pending notices, displayed notices, and decision-based notices. These counts help you monitor notice status and usage at a glance.

Notices are displayed as cards with notice name, type, description, and approval status if applicable.

To access, got to **Privacy Foundation** > **Privacy Catalog** > **Notice Management**

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Notice Management.png" alt=""><figcaption></figcaption></figure></div>

### Add a New Notice

* Select **Add Notice**.
* Enter the **Notice Name** and **Notice Description**.
* Select a **Notice Type**:
  * _Display Only_: Displays information to customers without requiring confirmation or consent.
  * _Acknowledge_: Requires customers to confirm that they have read the notice.
  * _Accept/Reject_: Supports consent flows in which customers can grant or reject consent.
* Enter the customer-facing content in the **Inform Message** editor. Use the formatting tools to structure the content.
* Then, select **Create Notice** to save it.

#### Adding Notices in Bulk

To add multiple notices at once, select **Download Excel Template** (![](<../../../../.gitbook/assets/Download Excel Template icon.png>)) to download the template. Enter the fields details in the specified format and save the file.

Then, select **Import** (![](<../../../../.gitbook/assets/Import from Excel.png>)) and upload the excel file.&#x20;

### Manage Notices

*   To edit a notice, select **Edit** (![](<../../../../.gitbook/assets/Edit icon (1).png>)) on the card. Make necessary changes and update. Every time you edit and save creates a new version. Use **Version history** (![](<../../../../.gitbook/assets/Version history icon.png>)) to view.<br>

    <div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Notice Management - Version history.png" alt="" width="563"><figcaption></figcaption></figure></div>
* Use **Clone** (![](<../../../../.gitbook/assets/Clone Icon (1).png>)) to create a copy of a notice.
* Use **Delete** (![](<../../../../.gitbook/assets/Delete Icon.png>)) to remove a notice that is no longer required.
* Use **Refresh** (![](<../../../../.gitbook/assets/Refresh icon.png>)) to load all the notices added to date.
* To export the data fields to an excel file, select **Export** (![](<../../../../.gitbook/assets/Export to Excel.png>)).
* Filter notices by type or search by its name.
* Switch between **Cards View** (![](<../../../../.gitbook/assets/Cards View icon.png>)) and **Table View** (![](<../../../../.gitbook/assets/Table View icon.png>)) to display the notices in your preferred layout.



<mark style="color:$warning;">**UX Observations**</mark><mark style="color:$warning;">:</mark>

* <mark style="color:$warning;">**Terminology Consistency**</mark><mark style="color:$warning;">: Although the terms - 'Add' and 'Create', both are correct in terms of functionality, use one standard term (Add or Create) consistently across the platform.</mark>&#x20;
* <mark style="color:$warning;">**Inform Message**</mark><mark style="color:$warning;">: This is unclear. Consider using "Message Content" or "Notice Content".</mark>
* <mark style="color:$warning;">**Metric Labels**</mark><mark style="color:$warning;">: Clarify the metric labels and their definitions. If these represent notice types, consider</mark> <mark style="color:$warning;"></mark><mark style="color:$warning;">**Display-only notices**</mark> <mark style="color:$warning;"></mark><mark style="color:$warning;">and</mark> <mark style="color:$warning;"></mark><mark style="color:$warning;">**Decision-based**</mark> <mark style="color:$warning;">**notices**</mark><mark style="color:$warning;">. If they represent usage or status, label them accordingly.</mark><br>

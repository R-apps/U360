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

# Data Fields

The **Data Fields** section lets administrators configure the personal information fields to present relevant personal information to customers, control which fields customers can view or update, identify sensitive information, and connect customer-facing fields to values stored in enterprise systems. This supports consistent data management across the Privacy Catalog and customer portal.

Configured data fields are displayed as cards with field name, description, business object and data category, visisbility status, approval status, editability, and field type.

To access, go to **Privacy Foundation** > **Privacy Catalog** > **Data Fields**

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Privacy Catalog - Data Fields.png" alt=""><figcaption></figcaption></figure></div>

### Adding a Data Field

Define each field, associate it with a business object and data category, and control whether customers can view, edit, or request updates to their information. Then, map the field to a data source and connector to retrieve the customer's current value.

To add a field,

* Select **+ Add Field**&#x20;
* In the **Create Personal Information Field** window,&#x20;
  * Select the business object to which the field belongs.
  * Select the category associated with the business object.
  * Enter the field name and describe the information the field represents.
  * Select the data type for the field.
* Then, configure how customers can interact with the field:
  * _Visible to Customer_ – Enable this option to display the field in the customer portal.
  * _Mark as Sensitive Information_ – Enable this option to mark the field as sensitive.
  * _Editable by Customer_ – Enable this option to allow customers to update the field.
  *   _Deletable by Customer_ – Enable this option to allow customers to delete the field.<br>

      <div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Privacy Catalog - Adding a Data Field.png" alt="" width="488"><figcaption></figcaption></figure></div>
* Select **Next** to configure field mapping.
  * _Data source_ – Select the source from which to retrieve the customer's current value.
  * _Connector (read)_ – Select the connector used to retrieve the value.
  * _Response parameter_ – Select the response parameter that contains the field value.
*   Then, select **Create Field**. The field gets added to the Data Fields list with the configured settings.<br>

    <div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Privacy Catalog - Mapping field to data source.png" alt="" width="476"><figcaption></figcaption></figure></div>

#### Adding Data Fields in Bulk

To add multiple data fields at once, select **Download Excel Template** (![](<../../../../.gitbook/assets/Download Excel Template icon.png>)) to download the template. Enter the fields details in the specified format and save the file.

Then, select **Import** (![](<../../../../.gitbook/assets/Import from Excel.png>)) and upload the excel file.&#x20;

### Manage Data Fields

* To edit a data field, select **Edit** (![](<../../../../.gitbook/assets/Edit icon (1).png>)) on the card to modify the field's details and configuration.
* Use Visibility toggle to enable or disable the field's visibility in the customer portal.
* Use **Clone** (![](<../../../../.gitbook/assets/Clone Icon (1).png>)) to create a copy of a data field.
* Use **Delete** (![](<../../../../.gitbook/assets/Delete Icon.png>)) to remove a field that is no longer required.
* Use **Refresh** (![](<../../../../.gitbook/assets/Refresh icon.png>)) to load all the data fields added to date.
* To export the data fields to an excel file, select **Export** (![](<../../../../.gitbook/assets/Export to Excel.png>)).
* To reorder the data fields, hover over it, hold the **Drag to reorder** ( ![](<../../../../.gitbook/assets/Drag icon.png>)) icon and drag it to the required position.
* Filter and search field either by its name or other search criteria.
* Switch between **Cards View** (![](<../../../../.gitbook/assets/Cards View icon.png>)) and **Table View** (![](<../../../../.gitbook/assets/Table View icon.png>)) to display the data fields in your preferred layout.

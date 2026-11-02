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

# Consent Categories

Define and manage consent categories used to organize customer consent by product, service, or business activity. For example, you can configure categories for insurance products, credit card offers, loan offers, and payment services. Manage category visibility, approval status, default settings, and activation.

Consent categories help organizations define consent purposes, improve transparency, manage consent validity, and link related configurations.

To access, got to **Privacy Foundation** > **Privacy Catalog** > **Consent Categories**

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Consent Categories.png" alt=""><figcaption></figcaption></figure></div>

### Add a New Category

* Select **Add Category**.
* Enter the **Category Name** and **Description** explaining the category purpose. Select **Plain text** for a simple description or **Rich text** to format the content, where supported.
* Select the **Consent purpose** from Purpose Management to define why it is required.
* Select an associated **Consent notice**, if applicable.
* Set the category's **Default state**. (For new customers, it is enabled by default.)
* Set the **Consent Expiry** if applicable by selecting the period, else, select **No expiry.**
* Use the **Legal basis and retention** section to define how the category's consent records are governed. You can either&#x20;
  * Enable **Inherit from RoPA** option to inherit settings from the selected Record of Processing Activities (RoPA) activity, or
  * Manually select the following:
    * **Legal basis**: Select the applicable legal basis, such as Consent.
    * **Retention period**: Specify how long the records should be retained.
    * **Retention trigger**: Select the event that starts the retention period.
    * **Retention action**: Select the action to perform when the retention period ends.
* Use the **Linked options** section to associate the consent category with other Privacy Catalog components. To link communication channels, select **Channels**, and select the checkboxes for the channels you want to associate. Use the other options to configure the corresponding links. As you select, the count gets displayed under each option.
* Then, select **Create Category** to save it.

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Add Consent Category.png" alt=""><figcaption></figcaption></figure></div>

#### Adding Categories in Bulk

To add multiple categories at once, select **Download Excel Template** (![](<../../../../.gitbook/assets/Download Excel Template icon.png>)) to download the template. Enter the fields details in the specified format and save the file.

Then, select **Import** (![](<../../../../.gitbook/assets/Import from Excel.png>)) and upload the excel file.&#x20;

### Manage Categories

* Use Visibility toggle to enable or disable the category's visibility in the customer portal.
* To edit a category's information, select **Edit** (![](<../../../../.gitbook/assets/Edit icon (1).png>)) on the card. Make necessary changes and save them.
* Use **Delete** (![](<../../../../.gitbook/assets/Delete Icon.png>)) to remove a category that is no longer required.
* Use **Refresh** (![](<../../../../.gitbook/assets/Refresh icon.png>)) to load all the categories added to date.
* To export the categories list to an excel file, select **Export** (![](<../../../../.gitbook/assets/Export to Excel.png>)).
* To rearrange, hover over a category card and use the **Drag to reorder** icon (![](<../../../../.gitbook/assets/image (34).png>)) to drag and place it in the required position.
* Switch between **Cards View** (![](<../../../../.gitbook/assets/Cards View icon.png>)) and **Table View** (![](<../../../../.gitbook/assets/Table View icon.png>)) to display the partners in your preferred layout.

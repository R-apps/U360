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

# Systems

This lets you configure integrations between the Consent Management Platform (CMP) and external systems, such as core banking, CRM, KYC, and campaign management platforms. It helps you define what personal information is shared with each system, map data fields to the appropriate sources, and configure data governance settings.

These integrations help organizations maintain visibility into how customer data flows between systems, support privacy governance, and manage data sharing in line with their data protection requirements under the Digital Personal Data Protection (DPDP) Act.

To access, got to **Privacy Foundation** > **Privacy Catalog** > **Systems**

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Systems.png" alt=""><figcaption></figcaption></figure></div>

### Add a New System

* Select **Add Integration**.
* In the **Platform Type** field, select the type of system you want to integrate, such as a KYC platform.
* Enter the **Integration Name** and **Description** to identify the integration and explain its purpose.
* Under **Data Governance**,&#x20;
  * Select the personal information fields the system can access.
  * Select **Add mapping** to map each selected data field to its data source, connector, and output parameter.&#x20;
  * The **Risk Level** is automatically assigned based on the selected personal information fields and their sensitivity settings.
  * Select the applicable status of the Data Processing Agreement (DPA)
  * Specify the region where the integration processes customer data.
* Then, select **Create Integration**.

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Add Integration.png" alt=""><figcaption></figcaption></figure></div>

#### Adding Integrations in Bulk

To add multiple integration systems at once, select **Download Excel Template** (![](<../../../../.gitbook/assets/Download Excel Template icon.png>)) to download the template. Enter the fields details in the specified format and save the file.

Then, select **Import** (![](<../../../../.gitbook/assets/Import from Excel.png>)) and upload the excel file.&#x20;

### Manage Integrations

* Use Visibility toggle to enable or disable the integrated system's visibility in the customer portal.
* To edit an integration, select **Edit** (![](<../../../../.gitbook/assets/Edit icon (1).png>)) on the card. Make necessary changes and save changes. Run the assessment to evaluate the privacy risks associated with sharing personal data with the external systems or service providers.&#x20;
* Use **Delete** (![](<../../../../.gitbook/assets/Delete Icon.png>)) to remove a integration that is no longer required.
* Use **Refresh** (![](<../../../../.gitbook/assets/Refresh icon.png>)) to load all the integrations added to date.
* To export the integrations list to an excel file, select **Export** (![](<../../../../.gitbook/assets/Export to Excel.png>)).
* Switch between **Cards View** (![](<../../../../.gitbook/assets/Cards View icon.png>)) and **Table View** (![](<../../../../.gitbook/assets/Table View icon.png>)) to display the integrations in your preferred layout.

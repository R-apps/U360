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

# RoPA Registration

The **Record of Processing Activities (RoPA)** feature helps organizations document and maintain records of how they collect, use, store, share, and retain personal data. It's a structured way to record processing activities, link them to business processes and systems, identify the personal information involved, and define applicable legal bases and retention controls.

Maintaining RoPA records helps organizations understand their data-processing activities, assess privacy risks, establish accountability, and maintain documentation to support compliance with the Digital Personal Data Protection (DPDP) Act and other applicable data protection requirements.

To access, go to **Privacy Foundation** > **Privacy Governance** > **RoPA Register**.&#x20;

The RoPA Register provides an overview of the processing activities recorded in the platform. Each RoPA record provides details about the associated processing activity, including its purpose, business owner, linked configurations, and retention information.

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/RoPA Register.png" alt=""><figcaption></figcaption></figure></div>

### Creating a RoPA Register

RoPA registration is a six-step process. Select **Create RoPA Register** and follow these steps:

{% stepper %}
{% step %}
#### Activity

Define the processing activity and its ownership.

* **Activity Name**: Enter a name that clearly identifies the processing activity, such as \
  "KYC Verification".
* **Legal Entity / Owner**: Specify the legal entity or business owner responsible for the processing activity. This establishes accountability for the activity.
*   **Description**: Describe what the activity involves and why personal data is processed.<br>

    <div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/RoPA - Step1 (Activity).png" alt="" width="563"><figcaption></figcaption></figure></div>

Select **Next** to proceed to business mapping.
{% endstep %}

{% step %}
#### Mapping

Link the processing activity to the relevant configurations in Privacy Catalog.&#x20;

* **Linked Consent Categories**: Select the consent categories associated with the processing activity.&#x20;
* **Channels** (**Auto-linked**): Select the communication channels associated with the selected consent categories, to provide visibility into how customers are contacted for the relevant activity.
* **Sharing Partners**: Select external partners with whom the personal data is shared as part of the processing activity, to identify third-party data-sharing arrangements.
*   **Systems / Integrations**: Select the systems involved in processing or managing the personal data, to keep track where the data is used or transferred.<br>

    <div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/RoPA - Step2 (Mapping).png" alt="" width="563"><figcaption></figcaption></figure></div>

Select **Next** to continue.
{% endstep %}

{% step %}
#### DPIA

Document the data protection impact assessment associated with the processing activity.

* **Data Categories**: Select the categories of individuals whose personal data is processed, such as Customers, Employees, Vendors, based on the available options, to help identify whose data is involved.
* **Personal Processing Purpose**: Describe why the personal data is collected and processed.&#x20;
* **Security Measures**: Describe the safeguards implemented to protect personal data, such as access controls, encryption, or other security measures, to define how the organization protects the data.
*   **Cross-border Transfer**: Enable this option if the processing activity involves transferring personal data outside the country.<br>

    <div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/RoPA - Step3 (DPDP).png" alt="" width="563"><figcaption></figcaption></figure></div>

Select **Next** to proceed to personal data identification.
{% endstep %}

{% step %}
#### PII

This displays the personal data fields identified for the processing activity based on the configured data mappings. Each field appears with its associated business object and data category.&#x20;

For example, the selected fields may include Aadhaar Number, Date of Birth, Email Address, PAN, Mobile Number, and other.

It even displays the **suggested Risk Level** based on the selected personal information and its sensitivity.&#x20;

Review and select **Next** to configure governance and retention settings.

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/RoPA - Step4 (PII).png" alt="" width="563"><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
#### Governance

Define the ownership, legal basis, and retention requirements for the processing activity.

* **Business Owner**: Identify the person, department, or business function responsible for the processing activity.&#x20;
* **Legal Basis**: Select the applicable legal basis for processing personal data, such as Consent or Contractual Obligation.&#x20;
* **Retention Period**: Specify how long the personal data or associated records should be retained.
* **Retention Trigger**: Select the event from which the retention period begins, such as Creation Date. This establishes when the retention period is calculated.
*   **Retention Action**: Select what should happen when the retention period ends.<br>

    <div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/RoPA - Step5 (Governance).png" alt="" width="563"><figcaption></figcaption></figure></div>

These settings help organizations establish clear ownership and define how personal data should be retained and handled throughout its lifecycle.

Select **Next** to review the registration details.
{% endstep %}

{% step %}
#### Review

The Review section provides a consolidated view of the information entered in the previous steps.&#x20;

Review and then select **Create RoPA** to complete the registration.

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/RoPA - Step7 (Review).png" alt="" width="479"><figcaption></figcaption></figure></div>
{% endstep %}
{% endstepper %}

### Mange RoPA Records

* Use Visibility toggle to enable or disable the record's visibility in the customer portal.
* To edit a record, select **Edit** (![](<../../../../.gitbook/assets/Edit icon (1).png>)) on the card. Make necessary changes and update.
* Use **Delete** (![](<../../../../.gitbook/assets/Delete Icon.png>)) to remove a record that is no longer required.
* Use **Refresh** (![](<../../../../.gitbook/assets/Refresh icon.png>)) to load all the records created to date.
* To export the records list to an excel file, select **Export** (![](<../../../../.gitbook/assets/Export to Excel.png>)).
* To rearrange, hover over a record and use the **Drag to reorder** icon (![](<../../../../.gitbook/assets/image (34).png>)) to drag and place it in the required position.
* Switch between **Cards View** (![](<../../../../.gitbook/assets/Cards View icon.png>)) and **Table View** (![](<../../../../.gitbook/assets/Table View icon.png>)) to display RoPA records in your preferred layout.

{% hint style="info" %}
Review the processing activity, associated personal information, and retention requirements periodically. Update the RoPA record whenever there are changes to the purpose of processing, data categories, systems, sharing partners, or data retention practices.
{% endhint %}

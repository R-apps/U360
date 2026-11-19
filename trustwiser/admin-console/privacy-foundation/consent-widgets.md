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

# Consent Widgets

In the customer-facing portal, the different sections visible to users are referred as **Widgets**.

Use **Consent Widgets** section to create, customize, and deploy consent interfaces on customer-facing portals. These widgets allow visitors to grant, update, or revoke permissions for data processing, communications, and privacy preferences across applications.

The page displays existing widgets with details such as their status, consent counts, opt-in rates, and recent submission trends. Use these details to monitor widget activity.&#x20;

To access, go to **Privacy Foundation** > **Consent Widgets**.&#x20;

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Consent Widgets.png" alt=""><figcaption></figcaption></figure></div>

### Creating a Consent Widget

The widget builder guides you through a seven-step configuration process.&#x20;

Select **+ Create Widget** to configure a new widget. You can select **Save Draft** at any stage to save your progress or select **Next** to proceed to the next step.

{% stepper %}
{% step %}
### Details

Enter the basic information (Widget Name, Description, and Logo) to identify the widget and describe where it will be displayed.

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Create widget- Step1 (Details).png" alt=""><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
### Notice (Purpose)

Select the data processing purposes for which customer consent is required.

Linking consent to specific purposes helps customers understand why their personal data is being processed and manage their permissions accordingly.

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Create widget - Step2 (Notice) .png" alt=""><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
### Data Fields

Select the data fields, such as contact information, profile details, or usage records.

Identifying the relevant data types helps establish what personal information is covered by the consent request.

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Create widget- Step3 (Data Fields).png" alt=""><figcaption></figcaption></figure></div>

#### 4. Preferences

Configure the preference controls customers can manage through the widget, such as communication frequency or topic preferences.

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Create widget- Step4 (Preferences).png" alt=""><figcaption></figcaption></figure></div>

#### 5. Channels

Select the communication channels to which the consent applies, such as Email, SMS, or Push Notifications. Channel-specific consent helps customers manage their communication permissions independently across different channels.

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Create widget- Step5 (Channels).png" alt=""><figcaption></figcaption></figure></div>

#### 6. Notices & Policies

Attach the relevant privacy notices and legal disclosures that customers can review before submitting their consent choices.

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Create widget- Step6 (Sharing Partners).png" alt=""><figcaption></figcaption></figure></div>

#### 7. Appearance

Select a visual theme for the widget and review it in the live **Preview** pane.

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Create widget- Step7 (Appearance).png" alt=""><figcaption></figcaption></figure></div>

Live preview helps you to view how the widget appears on the customer portal before publishing it.
{% endstep %}
{% endstepper %}

Finally, select **Create**. The widget gets created and previews the widget info such as widget id, version, embed script, enabling you to copy them or directly open it in the editor.&#x20;

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Create widget- Preview.png" alt=""><figcaption></figcaption></figure></div>

### Manage Consent Widgets

* Use **Toggle button** (![](<../../../.gitbook/assets/Toggle icon.png>)) to **Publish** or **Unpublish** a widget. Only published widgets are displayed in the customer-facing portal.
* Use **Show script** (![](<../../../.gitbook/assets/Show Script icon.png>)) to view the embed script within the widget card.\
  ![](<../../../.gitbook/assets/View script (Consent Widgets).png>)
* Use **Edit widget** (![](<../../../.gitbook/assets/Edit icon (1).png>)) to make necessary changes in the widget configuration.
* Use **Clone widget** (![](<../../../.gitbook/assets/Clone Icon (1).png>)) to create a copy of the widget.
* Use **Preview widget** (![](<../../../.gitbook/assets/Preview widget - icon.png>)) to see how the widget appears at run time.
*   Use **SDK** (![](<../../../.gitbook/assets/SDK icon.png>)) to get the links to access the widget's integration resources.<br>

    <div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/SDK - Widget Integration Resources.png" alt="" width="320"><figcaption></figcaption></figure></div>
* Use **Copy embed script** (![](<../../../.gitbook/assets/Clone Icon (1).png>)) to copy the script without viewing it.
* Use **Delete widget** (![](<../../../.gitbook/assets/Delete WIdget - icon.png>)) to delete a widget that is no longer required.

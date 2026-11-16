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

# Cookie Consent Widget

Use the **Cookie Consent Widget** tab to create and manage cookie consent widgets for your websites and applications. Configure the consent banner, customize its appearance, and preview how it appears to visitors before deploying it.

Only the cookie categories enabled in the widget configuration are displayed to visitors. Disabled categories are not loaded on the website.

To access, select the **Cookie Consent Widget** tab. This displays the configured widgets, including their name, ID, version, status, and last updated date. The widget status indicates whether it is _Published_ or in _Draft_.

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Cookie Consent widget.png" alt=""><figcaption></figcaption></figure></div>

### Create and Configure a Cookie Widget

* Select **Create Cookies Widget**.
* Enter the widget name.
* Configure the widget using the available settings.

The configuration screen provides two main tabs:

1.  **Sections:** Use this tab to configure the banner content, website association, and consent options.\
    The available configuration sections allow you to define the banner's identity, website association, consent options, and other settings.<br>

    <div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Cookie Consent Widget - Create (Sections).png" alt="" width="563"><figcaption></figcaption></figure></div>
2.  **Appearance:** Use the available settings to customize the visual presentation of the consent banner and preference center.<br>

    <div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Cookie Consent Widget - Create (Appearance).png" alt="" width="563"><figcaption></figcaption></figure></div>

The **Live Preview** panel displays the widget as you configure it. Switch between the Desktop, Mobile, and Full Width Preview options to see how your widget apers in different devices.

Then, select **Save** to save the configuration. The configured widget appears in the Cookie Consent Widget page.

#### Configure Script Setup

Deferring tracking scripts prevents non-essential cookies and trackers from executing before visitors provide consent. It also ensures that website tracking behavior aligns with the configured cookie categories and visitor preferences.

The **Script Setup – defer scripts on your website** section provides code examples and integration instructions to ensure that tracking scripts execute only after visitors provide the required consent.\
Each cookie category has a corresponding `data-cookie-category` attribute. Assign the appropriate value to each tracking script.

The section provides examples for:

* **External Script:** For scripts hosted on external servers.
* **Inline Script:** For JavaScript embedded directly in the website's HTML.

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Cookie Consent Widget - Script Setup.png" alt=""><figcaption></figcaption></figure></div>

Select **Copy** next to an example to copy its code for integration. Follow the specified steps to integrate cookie consent controls

### Manage Cookie Consent Widgets

* Use **Edit** (![](<../../../../.gitbook/assets/Edit Icon.png>)) option to update a widget's configuration.
* Use **View** (![](<../../../../.gitbook/assets/View icon.png>)) option to preview the widget's configuration.
* Use **Copy embed script** (![](<../../../../.gitbook/assets/Clone Icon (1).png>)) option to reuse a widget's script.
* Use **Publish** (![](<../../../../.gitbook/assets/Publish icon.png>)) and **Unpublish** (![](<../../../../.gitbook/assets/Unpublish icon.png>)) options to publish/unpublish a widget.
* Use **Delete** (![](<../../../../.gitbook/assets/Delete Icon.png>)) option to remove a widget that is no longer required.

<mark style="color:$warning;">**Queries**</mark><mark style="color:$warning;">:</mark>

* <mark style="color:$warning;">What represents the 'Batch' tag on a widget card?</mark>
* <mark style="color:$warning;">How the "copy embed script" option helps?</mark>

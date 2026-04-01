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

# Consent Management

Use this section to customize what appears on the customer-facing portal.&#x20;

You (The Client) can configure widgets, categories, response patterns, integrations, and communication channels based on your business requirements, and control which consent and data preference options are presented to users.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure></div>

> For each consent type, you can control the section's visibility (enable or disable).&#x20;

<details>

<summary><strong>Customer Data Field Configuration</strong></summary>

This widget helps you display the customer profile information with data fields such as Name, Mobile Number, Email, Date of Birth, and more.&#x20;

**Adding a new field**

* Select **Add** **Field**
* Enter the field name and description
* Select the Field Type (data type)
* Specify the Data Source Endpoint (API endpoint) from where the system can fetch the field value
* Next, scroll down to select the View, Edit, and Delete options to allow/restrict the customer to make changes to this field.
* If you are enabling the Edit/Delete options, configure Update Notice Message/Delete Notice Message to tell the system what message to display when users attempt to perform these actions.&#x20;

Then, select **Create Field.** The field gets created and is displayed in the \
**Customer Data Fields** section.

> Alternatively, you can use the default field types available on the right. To use, \
> select and customize them as required.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure></div>

You can manage the field and control its visibility even from here.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure></div>

Similarly, as many field as you require to display your customer profile information.

{% hint style="info" %}
* If edit or delete permissions are not enabled, the field is marked as **Read-only**; otherwise, it is marked as **Editable**.
* Fields are labeled **Visible** when the _Visible to customer_ option is enabled; otherwise, they are labeled **Hidden**.
{% endhint %}

You can also rearrange fields based on how you want them to appear to users. To rearrange, hover over a field and use this icon (![](<../../.gitbook/assets/image (34).png>)) to drag and place it in the required position.

</details>

<details>

<summary><strong>Consent Categories</strong></summary>

This widget helps you define and manage categories (for example, loan offers, insurance products) of all your products/services for which you need to collect customer consent.

You can also .

To add a category,

* Select **Add Category**
* Enter the category name and description&#x20;
* Enter a unique Id and description to define the consent purpose
* Configure consent notice message to tell the system what to display when users attempt to enable (grant) or disable (revoke) the consent.&#x20;
* Specify the default consent behavior when no response is received

> Alternatively, you can use the default categories available on the right. To use, \
> select and customize them as required.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (1) (1).png" alt=""><figcaption></figcaption></figure></div>

Then, select **Create Category**. The category is created and appears in the \
**Consent Categories** section.

Similarly, add all the categories for which the customers consent is required.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure></div>

Manage and control the category visibility from here.&#x20;

{% hint style="info" %}
Categories are labelled with their default status (Enabled/Disabled)
{% endhint %}

You can also rearrange categories based on how you want them to appear to users. \
To rearrange, hover over a category and use this icon (![](<../../.gitbook/assets/image (34).png>)) to drag and place it in the required position.&#x20;

</details>

<details>

<summary><strong>Channels</strong></summary>

Add all your preferred communication channels (SMS, Email, WhatsApp, App Push Notifications, and more) here, so you can collect customer preferences which channels would prefer for business-related communications.

To add a channel,

* Select **Add Channel**
* Enter the channel Name and Description
* Enter a unique Id and description to define the purpose of collecting consent
* Configure consent notice message to tell the system what to display when users attempt to enable (grant) or disable (revoke) a channel.&#x20;
* Specify the default consent behavior when no response is received
* Set default Partner status (Enabled/Disabled)

> Alternatively, you can pick a default channel from the right pane and customize it as required.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure></div>

Then, select **Create Channel**. The channel is created and appears in the **Channels** section.

Repeat the same steps to add all the communication channels you currently use.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure></div>

Manage and control channel visibility from here.

{% hint style="info" %}
Channels are labelled with their default status (Enabled/Disabled)
{% endhint %}

You can also rearrange channels based on how you want them to appear to users. \
To rearrange, hover over a channel and use this icon (![](<../../.gitbook/assets/image (34).png>)) to drag and place it in the required position.&#x20;

</details>

<details>

<summary><strong>Data Sharing Partners</strong></summary>

Manage all the data sharing partners or third-party applications that uses customer data for communication or service delivery, based on customer consent.

To add a data sharing partner,

* Select **Add Partner**
* Enter the Partner Name and Description
* Specify the channel key - a unique identifier
* Configure consent notice message to tell the system what to display when users attempt to enable (grant) or disable (revoke) a channel.&#x20;
* Specify the default consent behavior when no response is received
* Set default Partner status (Enabled/Disabled)

> Alternatively, you can pick a default partner from the right pane and customize it as required.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure></div>

Then, select **Add Partner**. The partner is created and appears in the **Data Sharing Partners** section.

Repeat the same steps to add all the partners who uses your customer data with consent.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure></div>

Manage and control partner visibility from here.

{% hint style="info" %}
Partners are labelled with their default status (Enabled/Disabled)
{% endhint %}

You can also rearrange these partners based on how you want them to appear to users. \
To rearrange, hover over a partner and use this icon (![](<../../.gitbook/assets/image (34).png>)) to drag and place it in the required position.&#x20;

</details>

<details>

<summary><strong>Event Subscribers (External Systems)</strong></summary>

Register external systems that uses this CMP for their customers' consent. While registering, configure [web hook endpoint URLs](#user-content-fn-1)[^1] to enable external systems to receive real-time events such as consent updates, withdrawals, and more.

To register an external system,

* Select **Add Web Hook**
* Enter the Subscriber Name (to identify external system) and Description (a short detail of external system's role)
* Specify the API endpoint URL through which we consent events will be sent to the external system.
* Select the consent event(s) that we pass through the specified Endpoint URL.
* Next, select the Authentication Type to secure the communication and the Authentication Value to authenticate requests.
* Make sure to keep the external system's status as "Active" to send uninterrupted consent events. You can disable when you want to stop communicating external systems.

> Alternatively, you can pick a default event subscriber from the right pane and specify how we send consent events to them.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (13).png" alt="" width="544"><figcaption></figcaption></figure></div>

Then, select **Add Web Hook**. The system adds the external system and appears in the \
**Event Subscribers** section.

{% hint style="info" %}
* **Request Format**:

This request format is used by CMS to send consent updates to the configured event subscriber (web hook URL).

```json
{
"event_type": "GRANTED",
"category": "CHANNEL",
"identifier": "SMS",
"timestamp": "2026-02-18T10:01:00Z",
"customer_id": "12345",
"tenant_id": "prime_3242"
}
```

Supported identifier values: PHONE\_CALL, EMAIL, SMS, WHATSAPP

* For more information, click ![](<../../.gitbook/assets/image (14).png>) in the Event Subscribers section.
{% endhint %}

Configured external systems are labelled with the consent events (that you are passing through its endpoint URL) and the authentication type for easy identification.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure></div>

Manage event subscribers from here. You can disable, edit, or delete an event subscriber.

</details>

<details>

<summary><strong>Systems Integration</strong></summary>

To integrate with any communication platforms, CRM applications, notification services, or campaign management platforms, configure and manage those integrations here.

To add an integration,

* Select **Add Integration**
* Enter the Integration Name and Description
* Select the Authentication Type (OAuth 2.0, Basic Authentication, API Key, Bearer Token, Custom) and specify its details
* Specify the API endpoint URL
* Mark it "Active" to keep this integration method active

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (16).png" alt="" width="347"><figcaption></figcaption></figure></div>

Then, select **Create Integration**. The added integration method appears in the main section.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (17).png" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
The added integrations are labelled with the authentication type and base url for easy identication.
{% endhint %}

You can manage these integrations right from this page too. You can disable it, make changes to it, or even delete it.

</details>

<details>

<summary><strong>Consent Widgets</strong></summary>

In the customer-facing portal, the different sections visible to users are called **Widgets**.\
Widgets allow you to group and display consent sections in a structured way.

You can:

* Embed multiple consent sections within a single widget, or
* Distribute consent sections across multiple widgets, based on your requirement

You can even customize the appearance of each widget to match your brand, ensuring a consistent user experience.

To configure a widget,

* Select **Create Widget**
* First, click![](<../../.gitbook/assets/image (18).png>) and rename the widget
*   Select the section(s) to be displayed in this widget. As you select, you see a live preview to the right. This helps you to view how it appears on desktop and mobile devices. <br>

    <div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (19).png" alt="" width="563"><figcaption></figcaption></figure></div>
*   Now, to style your widget, switch to the **Appearance** tab. You can select an available preset mode or you can create a custom preset.&#x20;

    *   If you apply an available preset, see how it appears in the preview.\
        &#x20;

        <div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure></div>
    *   For custom style, select **New** to create a new preset.

        * Enter the basic details like preset name and description
        * Select the Primary color and Text color
        * Specify the labels for Grant and Revoke actions

        <div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (21).png" alt="" width="432"><figcaption></figcaption></figure></div>

        * In the **Sections** tab, for each section, define the title, button position, helper text, and footer summary label.

        <div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (22).png" alt="" width="427"><figcaption></figcaption></figure></div>

        * In the **Custom CSS** tab, define all the elements in the available code with standard CSS selectors. Then, select **Preview** to view how the element appears.

        <div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (23).png" alt="" width="432"><figcaption></figcaption></figure></div>

        * Then, select **Create Mode**. This custom preset is then listed in the custom presets from where you can select to apply it to the widget.
    * Now, apply this preset to the widget and see its preview.

    <div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (24).png" alt="" width="563"><figcaption></figcaption></figure></div>

This is how you can customize the widget's appearance.

{% hint style="info" %}
Use **Documentation** to understand the standard CSS selectors.
{% endhint %}

Next, **save** the widget.&#x20;

Then, publish it to display in the customer-facing portal. To publish, select **Publish** and specify the version and a short description.&#x20;

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (25).png" alt="" width="253"><figcaption></figcaption></figure></div>

{% hint style="info" %}
* Whenever you edit this widget, publish it with incremented version number and specify the changes made to it. This helps you track the changes made in each version.
* Only published widgets are displayed in the customer-facing portal.
{% endhint %}

View all the widgets created to date in the **Consent Widgets** dashboard.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure></div>

#### Manage Widgets

* The latest version of the widget will be active by default. You can select a previous version of it, if required.
* View its analytics like clicks, impressions, and CTR for each widget.
* Click <img src="../../.gitbook/assets/image (26).png" alt="" data-size="original"> to make changes and publish it as a new version.
* Click ![](<../../.gitbook/assets/image (28).png>) to unpublish the widget.
* Click ![](<../../.gitbook/assets/image (29).png>) to view its analytics
* Click ![](<../../.gitbook/assets/image (30).png>) to preview it.
* Click ![](<../../.gitbook/assets/image (31).png>) to delete the widget.

</details>

[^1]: 

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

# Portal Studio

The **Portal Studio** is where you can create, configure, and publish customer-facing portals that allow customers to manage their personal information, consent preferences, communication settings, and privacy requests.

Customize each portal by adding the required page sections and components, configuring their settings, and mapping business objects to the appropriate portal.

This reduces dependency on manual support, improves customer control over personal data, and provides a centralized approach to privacy and consent management.

To access, go to **Privacy Foundation** > **Portal Studio**.The Portal Dashboard displays the available customer portals, along with their names, descriptions, GUIDs, versions, and publishing statuses.

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Portal Studio.png" alt=""><figcaption></figcaption></figure></div>

### Create a New Customer Portal

* Select **+ Add Portal**.
* In the **Create Customer Portal** window,&#x20;
  * Enter the portal a unique name to identify the portal easily, and
  * A brief description explaining the portal's purpose.
*   Then, select **Create Portal**. <br>

    <div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Create new portal.png" alt="" width="563"><figcaption></figcaption></figure></div>

The platform creates the portal opens it in the configuration workspace.

### Configuring the Portal

Organizing portal content into dedicated pages makes it easier for customers to find and manage specific privacy-related information without navigating through unrelated options.

The builder allows you to customize the portal's pages, add components, configure their settings, and preview the customer-facing interface.

{% stepper %}
{% step %}
#### **Portal Pages**

The Page dropdown in the left panel lists the available pages.\
![](<../../../.gitbook/assets/Portal - pages.png>)&#x20;

You can manage these pages as required.&#x20;

* To add a new page, select **Add page** (**+**).
* To modify the selected page's details, select **Edit page** (![](<../../../.gitbook/assets/Edit portal- icon.png>)). You can also choose to delete the page if it is no longer required.&#x20;

After defining the required pages, configure components in each page.&#x20;
{% endstep %}

{% step %}
#### **Adding and Configuring Components**&#x20;

The **Components** tab provides the available components that you can add to a portal page. Select the page and then select component(s) to be displayed in the selected page.

Next, in the **Configuration** tab, configure how the selected components should appear in the portal. You can apply a theme of your choice, set layout preferences and navigation, notice appearances, and more.

As you select the component or configure, every change is live previewed in the right-pane.

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Portal - Page configuration.png" alt="" width="563"><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
#### **Customize the portal appearance**

Use the controls available in the builder to customize and review the portal layout.

* **Desktop, Tablet, and Mobile**: Switch between device views to check how the portal appears on different screen sizes.
* **Language**: Select the language in which you want to configure or preview the portal. The TrustWizer paltform currently supports [13 different languages](#user-content-fn-1)[^1].
* **Mode**: Switch between the available editing and preview modes.
* **Preview**: Review the portal's appearance before publishing.

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Portal - customization.png" alt=""><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
#### **Save and publish the portal**

After completing the configuration:

* Save your changes without publishing the portal. You can continue editing it later.
* Preview the configured portal before making it available. The preview helps verify the page layout, navigation, content, and components from the customer's perspective.
* Publish the portal to make the configured experience available to customers.
{% endstep %}
{% endstepper %}

The platform publishes the portal and the portal appears in the portal dashboard displays the publishing status and version of each portal, helping administrators track its configuration and deployment state.

### Map Business Objects to Customer Portals

Mapping ensures that each [business object](../platform-overview/business-objects.md) is associated with the appropriate customer-facing portal. It helps organizations manage different user groups through separate portals while maintaining a consistent privacy management experience.

To configure,&#x20;

* Select **Mapping** in the **Portal Dashboard.**
* For each business object, select the appropriate portal from the dropdown list.

Then, select **Save Mapping** to apply the mappings.

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Portal - Mapping.png" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
Each business object can be mapped to only one portal. Only published portals are available for mapping.
{% endhint %}

[^1]: 1. English (EN)
    2. Hindi (HI)
    3. Telugu (TE)
    4. Bengali (BN)
    5. Marathi (MR)
    6. Tamil (TA)
    7. Urdu (UR)
    8. Gujarati (GU)
    9. Kannada (KN)
    10. Oriya (OR)
    11. Malayalam (ML)
    12. Punjabi (PA)
    13. Assamese (AS)
    14. MAI (Maithili)

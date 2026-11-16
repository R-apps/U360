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

# Cookie Inventory

Use **Cookie Inventory** to view, classify, and manage all cookies and tracking scripts discovered across your registered websites. This helps ensure that your consent banner handles trackers according to their assigned categories and supports compliance with privacy regulations.

To view, select the **Cookie Inventory** tab. The platform displays a summary of your website's tracking activity in the **Overview**, **Cookies**, and **Scripts**.

{% tabs %}
{% tab title="Overview" %}
The **Overview** tab displays a summary of your website's tracking activity.

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Cookie Inventory - Overview.png" alt=""><figcaption></figcaption></figure></div>
{% endtab %}

{% tab title="Cookies" %}
The **Cookies** tab to review discovered cookies and assign them to the appropriate consent categories. To update a cookie category, select the required category from the drop-down.

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Cookie Inventory - Cookies.png" alt=""><figcaption></figcaption></figure></div>
{% endtab %}

{% tab title="Scripts" %}
Select the **Scripts** tab to review and categorize JavaScript tags discovered during website scans. Categorizing scripts helps the consent management platform defer their execution until visitors provide the required consent.

* **External:** Scripts hosted on third-party servers.
* **Inline:** Scripts embedded directly in the website's HTML.
* Select the dropdown in the **Category** column and assign the appropriate consent category.
* Review the **Defer as** attribute and the **URL/Snippet** preview to understand how the script is configured to behave before consent is provided.

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Cookie Inventory - Scripts.png" alt=""><figcaption></figcaption></figure></div>
{% endtab %}
{% endtabs %}


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
---

# Best Practices for Template Creation

These are some of the best practices that we recommend following when creating a template.

1. Creating separate layers for the following makes maintenance easier and avoids frequent layout changes.

* Header/Footer
* Branding blocks
* Static/Dynamic content
* Conditional sections

<mark style="color:yellow;"><\<IMAGE>> - Sample image displaying all parts of the template</mark>

2. Keeping the template design simple. A well-organized layout improves readability and reduces rendering time.  Avoid heavy backgrounds or too many decorative elements.
3. Before designing complex layouts,

* Review the input XML/JSON
* Ensure field names match&#x20;
* Check for null or optional fields

&#x20;Early data validation prevents rework after the layout is complete.

{% hint style="info" %}
Since the input identifiers and tags are case-sensitive, handle bulk input files carefully.
{% endhint %}

4. Preview the created template with multiple data sets. It helps catch alignment and overflow issues.
5. When working with dynamic objects, map the data cautiously.&#x20;
6. Follow your organization's standards for font, color, logos, and other UI standards, to maintain a unified customer experience across channels.
7. Use business rules for layout switching, enabling/disabling layers/pages, and other carefully.&#x20;
8. Always create a new version before making changes.\
   Name versions clearly along with the user's name. For example:

&#x20;                       “v2 – Added new address field - John”\
&#x20;                       “v3 – Updated billing summary table - Mathew”

A template should behave consistently, regardless of the delivery channel.

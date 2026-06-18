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
    visible: true
  pagination:
    visible: true
  metadata:
    visible: false
  tags:
    visible: true
  actions:
    visible: true
---

# Template Migration

Template Migration allows you to move templates and their associated configurations between UniServe 360 environments without recreating them manually.

This feature is commonly used to promote templates across environments, such as Development, Testing, UAT, and Production, while maintaining consistency in template design and configuration.

Template Migration uses UniServe package files (**TDPKG**) to export and import templates as a single deployment unit.

### How Template Migration Works

Template Migration consists of two operations:

1. **Export Templates** – Creates a package containing the selected templates and associated configurations.
2. **Import Templates** – Deploys the exported package into another UniServe 360 environment.

The exported package is saved in **TDPKG** format and can be imported into another UniServe 360 instance.

{% hint style="info" %}
Template Migration is intended for UniServe-to-UniServe migration. It does not import external file formats such as DOCX, PDF, HTML, or templates created in other communication management platforms.
{% endhint %}

## Export Templates

The **Export Templates** feature allows you to export individual or multiple templates as a single package. When you export templates, the system generates a package that includes the selected template(s), template settings, and associated application configurations.

Before you begin, ensure that:

* The templates are available in the source environment.
* The templates are checked in and ready for deployment.
* You have the required permissions to export templates.

To export an individual template,&#x20;

* In the **My Templates** page and navigate to the template to be exported.
* Select **Actions** (![](<../.gitbook/assets/image (134).png>)) > **Export**

<div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/Export single template.png" alt=""><figcaption></figcaption></figure></div>


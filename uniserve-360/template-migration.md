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

### Export Templates

The **Export Templates** feature allows you to export individual or multiple templates as a single package. When you export templates, the system generates a package that includes the selected template(s), template settings, and associated application configurations.

Before you begin, ensure that:

* The templates are checked in and ready for deployment.
* You have the required permissions to export templates.

#### Individual Template Export

To export an individual template,

* In the **My Templates** page, navigate to the template to be exported.
* Select **Actions** (![](<../.gitbook/assets/image (134).png>)) > **Export**

<div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/Export single template.png" alt=""><figcaption></figcaption></figure></div>

The template gets exported as a package to your machine's local storage.

#### Bulk Export

To export multiple templates at once,

* In the dashboard, select **Export.**
* Choose the templates to be exported and select **Next**.
*   Review the selected templates and select **Export Templates**.

    <div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/Bulk export templates.png" alt=""><figcaption></figcaption></figure></div>

### Import Templates

The **Import Templates** feature allows you to migrate templates and their associated configurations from one UniServe 360 environment to another.&#x20;

Depending on how the package was created, it can include:

* Template definitions
* Associated template configurations
* Application-level settings (where applicable)
* Template dependencies

Before you begin, ensure the package (`.TDPKG`) was exported from a compatible UniServe 360 environment and you have permission to import templates.

To import,

* In the **Templates Dashboard**, select **New** > **Import**.
*   Browse to and select the required .TDPKG file.

    <div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/Import Template - Package selection.png" alt=""><figcaption></figcaption></figure></div>
* UniServe initiates the import process. Follow the steps in the Import wizard.
* Review the import summary, and then complete the import.

During the import process, UniServe 360 validates the selected package and checks whether any templates already exist in the target environment. Templates that already exist are marked with an **Exists** tag. You can choose whether to overwrite these templates during the import.

<div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/Import Template - Exists Tag.png" alt=""><figcaption></figcaption></figure></div>

If you choose to overwrite an existing template, UniServe 360 automatically creates a backup of the current template and stores it in the **Rollback** folder before replacing it. \
You can use this backup to restore the previous version if required.

<div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/Import Template - Rollback.png" alt=""><figcaption></figcaption></figure></div>

* Use **Next** to preview every step of import process.

#### Auto Check-in

The final step of the Import wizard includes the **Check-in on Import** option.&#x20;

Enable this option to automatically check in all imported templates after the import completes.

<div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/Import Template - auto check-in.png" alt=""><figcaption></figcaption></figure></div>

### Import and Export Logs

UniServe generates log files for both import and export operations.

These logs help administrators:

* Verify successful migrations.
* Identify failed imports or exports.
* Troubleshoot deployment issues.
* Review migration activity.

Import and export logs are stored in their respective configured log locations.

Review these logs after each migration to confirm that all templates, dependencies, and configurations were processed successfully and to quickly identify any issues that require corrective action.

#### Admin-controlled Template Migration

Admin-controlled Template Migration helps organizations streamline template deployment by allowing users with **'**&#x41;dministrator' or 'Super Administrator' permissions to manage **Import** and **Export** operations from a central location.

This feature is beneficial for organizations with multiple template designers and structured release processes. It helps:

* **Reduced deployment effort** by eliminating the need for individual designers to migrate their own templates.
* **Protect template integrity** by allowing administrators to migrate templates without accessing or modifying their design.
* **Scale deployment operations** by providing a consistent migration process, regardless of whether the organization has a few template designers or large design teams.

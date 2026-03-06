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

# Process Management

**Process Manager** allows you to start template processing without launching the full UniServe application interface. You can run processing in the following modes:

* User Process
* Daemon Process
* Scheduled Process

The following table helps you understand when to use each processing mode.

<table data-full-width="false"><thead><tr><th width="157" valign="middle">Processing Mode</th><th width="289" valign="middle">Description</th><th valign="middle">When to Use</th></tr></thead><tbody><tr><td valign="middle"><strong>User Process</strong></td><td valign="middle">Processes when a user manually triggers the template execution.</td><td valign="middle">Use when template processing needs to be started manually for specific jobs or testing purposes.</td></tr><tr><td valign="middle"><strong>Daemon Process</strong></td><td valign="middle">Processing runs continuously in the background and automatically processes templates when data becomes available.</td><td valign="middle">Processing runs continuously in the background and automatically processes templates when data becomes available.</td></tr><tr><td valign="middle"><strong>Scheduled Process</strong></td><td valign="middle">Processing is executed at predefined times based on a schedule.</td><td valign="middle">Use when template processing must occur at fixed intervals, such as daily or periodic batch runs.</td></tr></tbody></table>

{% hint style="info" %}
Processing in different modes depends on the requirement and operational setup.
{% endhint %}

Using Process Manager, you can:

* Configure a [**MPT**](multi-processing-templates.md)
* Configure a **User Process**
* Configure a **Daemon Process**

Process Manager also supports **MPTs** (Multi-Processing Templates), which allow multiple processors to handle template processing simultaneously for improved performance.

The process configuration includes Primary and Secondary clients, as defined in the Environment Configuration. While creating a configuration, specify the template name, description, and select the template from the server template list.

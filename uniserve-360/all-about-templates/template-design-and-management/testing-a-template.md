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
    visible: true
---

# Testing a Template

Validate your template by generating and previewing multiple output formats from a single test run.

The **Template Testing** feature allows you to upload a sample input file (such as an XML file) and execute a test directly from the Designer interface. UniServe 360 automatically identifies the associated FGT and generates the configured output formats.

### Why use Multi-output View?

Instead of running separate tests for each output channel, this feature allows you to treview all generated outputs from a single test execution, making template validation faster and more efficient.

This helps you:

* Verify that the template renders correctly across different output formats.
* Validate data mapping and dynamic content.
* Reduce the number of test executions.
* Identify formatting issues early.
* Improve template quality before deployment.

#### How to test a template?

To test a template,

* In the Designer interface, select **Test Process**
* Upload the test data source file (XML, JSON, DB, or Text file)
* Select custom index and client settings, if required.

Then, select **Start Test Process**.

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Testing Template - Input Data.png" alt=""><figcaption></figcaption></figure></div>

After completing the test run, UniServe 360 displays the test result, as shown in the illustration below.

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Test Process Result (2).png" alt="" width="563"><figcaption></figcaption></figure></div>

* To download the document, select **Download** **File** (![](<../../../.gitbook/assets/Download Doc icon.png>))
* To view, the document, select **View** (![](<../../../.gitbook/assets/View icon.png>)).

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/View Test Process Result (1).png" alt="" width="563"><figcaption></figcaption></figure></div>

{% hint style="info" %}
When uploading sample data, ensure it covers all relevant conditions and business rules. This helps verify that the template processes data accurately and behaves as expected across different scenarios.
{% endhint %}

> #### Best practices
>
> * Use representative sample data when testing templates.
> * Review the generated output carefully before deploying the template.
> * Repeat the test after updating layouts, business rules, or dynamic content.
> * Validate both static and dynamic sections of the template.

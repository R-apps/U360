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

Validate your template using sample input data before deploying it.

The **Test Process** feature allows you to verify how a template is processed with your input data. Upload a supported data file, run the test, and review the generated output without affecting production processing.

UniServe 360 automatically identifies the associated **FGT** for the selected template and uses it during the test process. The generated output is displayed in the multi-output view, allowing you to review the results within the testing interface.

#### Why testing is important?

Testing helps you ensure that the template is production-ready and reliable. It ensures:

* Accurate data rendering
* Correct application of business rules
* Consistent layout across pages
* Compliance with branding and regulatory requirements

#### How to test?

To test a template,

* In the Designer interface, select **Test Process**
* Upload the test data source file (XML, JSON, DB, or Text file)
* Select custom index and client settings, if required.

Then, select **Start Test Process**.

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Testing Template - Input Data.png" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
When uploading sample data, ensure it covers all relevant conditions and business rules. This helps verify that the template processes data accurately and behaves as expected across different scenarios.
{% endhint %}

> #### Best practices
>
> * Use representative sample data when testing templates.
> * Review the generated output carefully before deploying the template.
> * Repeat the test after updating layouts, business rules, or dynamic content.
> * Validate both static and dynamic sections of the template.

<mark style="color:red;">Q: what exactly does "multiple outputs" mean in UniServe 360?</mark>

* <mark style="color:red;">Multiple output formats generated from the same test (for example, PDF, HTML, Email, SMS preview)?</mark>

&#x20;      <mark style="color:red;">or</mark>

* &#x20;<mark style="color:red;">Multiple documents/records generated from the uploaded input file (for example, if the XML contains 100 customer records, you can preview outputs for multiple customers in one testing session)?</mark>

<mark style="color:red;">Can we capture the Test Process result?</mark>

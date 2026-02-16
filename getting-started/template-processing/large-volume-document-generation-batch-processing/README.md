# Large-Volume Document Generation (Batch Processing)

**Batch processing** in UniServe 360 lets you generate large volumes of documents such as statements, notices, or bulk PDFs in one run. **Batch Configurations** help you define how and where UniServe 360 should connect when running batch jobs.&#x20;

### Checklist and Prerequisites

Before running batches, make sure the following are in place:

* UniServe 360 application is installed and running
* Required permissions are assigned to run batch jobs
* Document template is ready with the necessary business logics and is tested with sample data
* Input data readiness - batch input files are available at the configured input path or source and the file format (CSV, TXT, XML, or database input) matches the expected schema
* The target environment (QA, UAT, or Production) is set up and ready to use.
* FGT Configuration
  * Required output filters (PDF, AFP, HTML, PS) are added as plugins,
  * FGTs are created for File Level, Level1, and Level2, as needed, and
  * An accessible output path&#x20;
* Client and Channel Configuration&#x20;
  * Primary and Dependent clients are registered in UniServe 360.
  * Required channels (Print, Email, SMS, WhatsApp, or Direct Print) are configured.
* Indexing
  * Job schemas for primary and dependent clients are available.
  * Custom fields are mapped using global Data Variables, if required.

{% hint style="info" %}
**Quick Tip**:

Start with a small batch, verify the output and indexing, and only then scale to full volumes. This avoids reprocessing and data inconsistencies.
{% endhint %}

> <mark style="color:orange;">Queries</mark>
>
> 1. <mark style="color:orange;">How the Job status, delivery status, logs, and error messages are reviewed? -</mark> **Reports**

Once all these are ready,&#x20;

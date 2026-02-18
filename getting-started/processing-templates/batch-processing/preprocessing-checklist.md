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

# Preprocessing Checklist

Before running batches, make sure the following are in place:

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

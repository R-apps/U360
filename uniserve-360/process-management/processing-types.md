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

# Processing Types

### Single Server Processing

Single-server processing is the default method used to process templates in UniServe 360. In this setup, the system processes the template using a **single processing instance** on one server.

The template engine retrieves input data, applies the template design, and generates the output sequentially. Each processing task completes before the next one begins.

This approach is used

* when the volume of data is small or moderate, or&#x20;
* when the template is processed manually for testing or controlled runs.

#### How it works?

In single-server processing, all template processing activities occur on a single server instance.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (31).png" alt=""><figcaption></figcaption></figure></div>

Since the processing occurs sequentially, only one processing stream handles the workload at a time.

### Multi-Processing

Multi-processing approach allows UniServe 360 to process a template using multiple processors simultaneously.

Instead of processing records sequentially one after the other, you can distribute the workload to multiple processing instances. Each processor handles a portion of the data, enabling the system to generate outputs in parallel.

Multi-processing is configured using a [Multi-Processing Template (MPT)](multi-processing-templates.md) in the Process Manager.

This approach helps improve processing efficiency when working with large batches.

#### How it Works?

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure></div>

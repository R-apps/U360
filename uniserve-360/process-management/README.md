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

When UniServe 360 processes communications, it uses several system components to generate the final output.&#x20;

Here's a quick view of the elements involved in this process:

<table><thead><tr><th width="173">Process Element</th><th>Description</th></tr></thead><tbody><tr><td><strong>Template</strong></td><td>A design that defines how output documents or messages are generated</td></tr><tr><td><strong>Process Manager</strong></td><td>A system component used to configure and manage template processing</td></tr><tr><td><strong>Processor</strong></td><td>A system resource responsible for executing template processing tasks</td></tr><tr><td><strong>Worker</strong></td><td>A processing instance that handles part of the workload</td></tr><tr><td><strong>MPT</strong></td><td>A configuration that enables parallel template processing</td></tr><tr><td><strong>Failover</strong></td><td>A mechanism that transfers processing to a secondary server if the primary server fails</td></tr></tbody></table>

Understanding how these components work together helps you configure processing more effectively, especially when using multi-processing templates.

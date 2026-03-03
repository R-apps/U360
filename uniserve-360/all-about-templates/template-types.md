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
---

# Template Types

Templates in UniServe 360 are classified based on how they are used and processed.

#### Regular Template

A standard template, designed and processed independently. It contains layout, data mapping, business rules, all in one place; easy to manage for single-purpose communications.

Use Regular Templates when:

* The document structure and content are specific to one use case
* The template does not need to be reused across multiple documents
* Branding and layout are unique to that document

#### Global Template

A static reusable template, designed to be shared across multiple templates. It usually contains common sections that remain consistent such as branding blocks, disclaimers, regulatory text, etc.&#x20;

Use Global Templates when:

* The same content appears in many templates
* Branding or legal text must stay uniform
* Updates should reflect everywhere automatically

#### Master/Child Templates

A Master–Child template model helps you design modular templates and assemble them at runtime using [Merge Template](template-types.md#merge-templates). This approach reduces duplication, simplifies maintenance, and keeps branding consistent. Master and Child templates are maintained separately.

A Master Template defines the common structure shared across the documents.\
A Child Template holds the document-specific content&#x20;

While the Master Template acts as base frame, child templates focus only on what changes.&#x20;

Prefer using Master-Child templates when working collaboratively for a quick Turnaround Time.

**Example**:&#x20;

* _Master Template_: Bank-branded statement layout with logo, footer, and regulatory text
* _Child Templates_:
  * Credit card statement
  * Loan statement
  * Account summary

#### Merge Template

A Merge Template, merges Master and Child Templates to generate a full document. When your master and child templates are ready, create a Merge Template, load the master and add child template(s). Apply business logics, if required and then generate a single, final output.

Use Merge Template at runtime to merge the required child(s) and master to produce the final document.

#### Label Templates

<>

> <mark style="color:orange;">**Queries:**</mark>
>
> 1. <mark style="color:orange;">What are Label templates and when they are used?</mark>

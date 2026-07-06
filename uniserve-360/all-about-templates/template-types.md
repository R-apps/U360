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

# Template Types

Templates in UniServe 360 are classified based on how they are used and processed.

### Regular Template

A standard template, designed and processed independently. It contains layout, data mapping, business rules, all in one place; easy to manage for single-purpose communications.

Use Regular Templates when:

* The document structure and content are specific to one use case
* The template does not need to be reused across multiple documents
* Branding and layout are unique to that document

### Global Template

A static reusable template, designed to be shared across multiple templates. It usually contains common sections that remain consistent such as branding blocks, disclaimers, regulatory text, etc.&#x20;

Use Global Templates when:

* The same content appears in many templates
* Branding or legal text must stay uniform
* Updates should reflect everywhere automatically

### Master-Child & Merge Templates

The **Master-Child & Merge Template** model helps you build and manage related templates more efficiently. Instead of configuring common settings repeatedly, you can define them once in a **Master** template and reuse them across multiple **Child** and **Merge** templates.

The Master template contains the shared configurations, while Child and Merge templates inherit the applicable settings and maintain their own template-specific content.

This approach reduces repetitive configuration, promotes consistency, and simplifies template maintenance, especially when multiple designers work on related templates.

#### **How it works?**

The **Master** template serves as the central template for shared configurations.

When you create Child or Merge templates from a Master template, UniServe 360 automatically inherits the applicable configurations. These inherited configurations are displayed as **read-only** in Child and Merge templates to preserve consistency and prevent accidental modifications.

Any changes made to the shared configurations in the Master template are automatically reflected in the associated Child and Merge templates.

Configurations that are specific to a particular template can still be defined independently within the respective Child or Merge template.

#### Inherited configurations

The following configurations can be inherited from the Master template:

* Template layout
* Actions
* Custom Indexing
* FGT Advanced Settings such as document properties, digital signature, encryptions and more.

Inherited configurations appear as **read-only** in Child and Merge templates. This ensures that shared configurations remain consistent across all related templates.

> **Note**\
> To modify an inherited configuration, update it in the Master template. UniServe 360 automatically reflects the changes in all associated Child and Merge templates.

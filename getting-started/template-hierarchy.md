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
---

# Template Hierarchy

A template in UniServe 360 is organized into five core elements: \
**Document → Group → Page → Layer → Objects**.\
Each element serves a specific purpose and helps you structure complex, high-volume customer communications effectively.

Let's look at each element.

#### **1. Document**&#x20;

The **Document** is the topmost container of your template. It defines the overall output structure, such as a complete statement, policy document, notice, bill, or letter.\
Always - every template starts with a document.

**When to use?**

Use it to define the highest-level structure of any customer communication.&#x20;

**Example**: Monthly bank statement, credit card welcome kit, insurance policy schedule, and other.

#### **2. Group**

A **Group** is a logical section within the Document, using which you can organize the document into manageable sections. \
It helps divide the content into meaningful segments based on business logic or data requirements. Each Group can contain one or more Pages.

**When to use?**

Use Groups when your template has:

* Multiple sections
* Conditional blocks



1. **Page** - is divided into **Layers**. You can add as many Layers as needed to manage layout and control visibility.
2. **Layer** - helps you handle different parts of the template independently with full control, so you can organize the template effectively.
3. **Objects -** such as text, images, tables, lines, shapes, barcodes, and mapped data fields—are placed on Layers. These are the actual elements that appear in the final output. \
   To understand the objects available in UniServe 360, [click here](template-designer/objects-and-properties.md)

These form the basic structure of every design. This structure makes it easier to manage layout and control what appears in the output.&#x20;

This is how a template hierarchy look:

<mark style="color:$success;">**<\<IMAGE - TEMPLATE HEIRACRCHY>>**</mark>

Visibility can be controlled at both the Layer and Object level. These controls may be fixed or driven by business rules.

{% hint style="info" %}
The **Input Data**, **Properties**, and **Layers** tabs appear by default, in the right pane.&#x20;

The **Layers** tab is always available. If any other tab do not show up by default, you can turn it on by navigating to **View** menu by enabling the required option.
{% endhint %}

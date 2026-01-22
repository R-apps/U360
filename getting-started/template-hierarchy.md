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

#### **Document**&#x20;

The **Document** is the topmost container of your template. It defines the overall output structure, such as a complete statement, policy document, notice, bill, or letter.\
Always - every template starts with a document.

**When to use?**

Every template you create serves as a document.&#x20;

**Example**: Monthly bank statement, credit card welcome kit, insurance policy schedule, and other.

#### **Group**

A **Group** is a logical section within the Document, using which you can organize the document into manageable sections. \
It helps divide the content into meaningful segments based on business logic or data requirements. Each Group can contain one or more Pages.

**When to use?**

Use Groups when your template has:

* Multiple sections
* Conditional blocks

**Example**: Think of an **Insurance Policy Document** where you have to include primary policy information, Terms & Conditions and Surrender rules, benefit illustration, etc. As these information flow across the pages, you can consider grouping these pages for easy access and identification.

#### Page

A **Page** represents a physical or digital page in the output document.&#x20;

Pages allow you to add as many Layers as needed to manage layout and control page visibility. \
"Page 1" is available by default.

**Example:** In an Insurance Renewal Notice, you can use pages like this:

* Page 1: Renewal Summary
* Page 2: Premium Breakup
* Conditional Page: “No Claim Bonus” details (use conditions to show only if applicable)

#### Layer

A **Layer** sits inside a Page. Layers work like transparent sheets stacked on top of each other.

Layers helps you handle different parts of the template independently with full control using business conditions, so you can organize the template effectively.

**Example**: In a Bank Statement, you can organize communication like this:

* Layer 1: Header with logo and branch details
* Layer 2: Customer Summary
* Layer 3: Advertisements or Offers (visible only for select segments)
* Layer 4: Regulatory Disclosures (only for accounts with foreign remittances)

#### Objects

**Objects** are the individual content elements placed on Layers. They are the actual items that customers see in the final document.&#x20;

These include text, images, barcodes, shapes, tables, signatures, and dynamic fields mapped to input data. To understand the objects available in UniServe 360, [click here](template-designer/objects-and-properties.md).&#x20;

Objects can be shown or hidden based on rules - the most granular level of visibility.

**Example**:&#x20;

* **Text Objects** – Customer Name, Account Number, Policy Number
* **Image Object** – Bank Logo, Branch Stamp, Customer Photo
* **Dynamic Data Fields** – Balance, EMI Amount, Premium Due
* **Tables** – Transaction list, EMI schedule, Claim history
* **Barcodes / QR Codes** – Policy reference, payment link
* **Shapes/Lines** – Section dividers in statements

These form the basic structure of every design. This structure makes it easier to manage layout and control what appears in the output.&#x20;

This is how a template hierarchy look in UniServe360:

<div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/Template Hierarchy.png" alt=""><figcaption></figcaption></figure></div>

> Visibility can be controlled at both the Layer and Object level. These controls may be fixed or driven by business rules.

{% hint style="info" %}
The **Input Data**, **Properties**, and **Layers** tabs appear by default, in the right pane.&#x20;

The **Layers** tab is always available. If any other tab do not show up by default, you can turn it on by navigating to **View** menu and enabling the required option.
{% endhint %}

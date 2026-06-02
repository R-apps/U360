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

# Know How UniServe 360 Works

UniServe 360 works as a template-driven customer communication platform. It takes **input data**, processes it through **business logic**, and generates **personalized outputs**.

This article explains the end-to-end process so you can understand how the system works.

### **How It Works**

1. **Creating the Template**\
   The template is structured using layout components such as Document, Group, Page, Layer, and Objects and is designed by adding branding elements, sections, headers, footer, and inserting text, tables, charts, barcodes, and data fields.\
   **Example:**\
   A bank uses a single savings account statement template. All customers receive the same layout, while balances, transactions, and dates vary for each customer.
2. **Configuring Input Data Source**\
   The template is connected with customer data. Data is received from systems like core banking, policy admin, billing, etc.\
   Formats can be XML, JSON, DB, Text, etc.
3. **Mapping Data** \
   Input data (example: Name, Account Number, Transactions) is mapped to the template objects.&#x20;
4. **Adding Business Rules**\
   The template is personalized by adding the necessary conditions, events, and actions, defining what to show/hide, compute, or format.\
   For example:
   * Show a notification if Minimum Amount Due > 0
   * Display a promotional offer only when customer is eligible
5. **Processing**\
   The processing engine applies the template to the data.
   * Simple objects
   * Complex objects (tables, repeating records)
   * Pre-actions and post-actions
6.  **Generate Output**

    After mapping the data, UniServe 360 generates the output. You can generate:

    * Single communication (on demand)
    * Large batch jobs (thousands or millions)

&#x20;     The system applies business logic, merges data with the template, and generates the final output.

&#x20;      **Example:** A bank runs a monthly batch for 1.2 million credit card statements and generates PDF   \
&#x20;      statements, email, and SMS alerts for minimum due.

7. **Multi-Format Output**\
   Once processed, output can be generated in multiple formats:

* PDF
* Print streams
* Email HTML
* SMS&#x20;

8. **Delivery & Distribution**\
   Output is sent to customer channels or integrated into the enterprise system.

This improves accuracy and reduces rework in enterprise communication systems.


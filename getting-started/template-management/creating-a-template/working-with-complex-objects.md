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

# Working with Complex Objects

A complex object in UniServe 360 is a grouped set of related data elements that are displayed\
together as one unit.

Think of a monthly transactional statement, which includes multiple transactions, and every              transaction contains several fields—date, description, debit, credit, and balance. Every time the               template is generated; all these fields are rendered as a table or repeated block. This entire              grouped structure is treated as a complex object. These complex objects display multiple               records in an organized format such as a table within the template.&#x20;

Let's look at defining a complex object that uses the table data,&#x20;

* &#x20;select the "Complex Object" from the left pane. \
  &#x20; <mark style="color:green;">**<\<IMAGE>>**</mark>\
  Click <mark style="color:$success;">\<icon></mark> to define the node. Select to map the table in the input data to which the object                  refers to.\
  &#x20; <mark style="color:green;">**<\<IMAGE>>**</mark>\
  Click **Ok**.
* Now, expand the **Main** and map the Header to the Header row of the table. To map, go to                 Identifier and click <mark style="color:$success;">\<icon></mark>. It displays the mapped table. Expand it and select the table header. \
  &#x20;Then, click **Ok** to map. \
  &#x20;  <mark style="color:green;">**<\<IMAGE>>**</mark>\
  For columns in the table, check the number of columns in the mapped table and use '+' icon in                  the Header row to add the required number of columns. Select each column and specify its                 data type, column type, field to which the column should map to, and lookup (in case of DB). \
  Similarly, configure and map the other columns in the Header.&#x20;

Follow the same process for **Body** and **Footer** as well. Select the node, define the params and                map them to the table data.

{% hint style="info" %}
* As the table object renders the data as per the mapping structure, map the data correctly.
* It's not necessary to add all the columns available in the table data, you can create and map only the required columns.&#x20;
* While mapping the **Body** section (the actual table data), make sure to enable the **Row\_Definition** param as '**True**'.
* Also, you can configure only the **Header** and **Body** sections leaving the **Footer** section unconfigured in case if you do not require the footer data or if there is no footer in the table data.
{% endhint %}

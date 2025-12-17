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

# Adding Computations

### What are computations?

Computations in UniServe 360 allow you to create new values by applying formulas or text operations on the data extracted from the source file. These computations help improve the content you display in the final output, such as account statements, letters, or notifications.

You can perform computations on both **simple objects** and **complex objects**. Computations run automatically during template processing and can be reused in different areas of the template.

### When to use?

Use computations when you want to transform or calculate values before printing them. \
Some typical use cases include:

* Formatting customer names
* Adding labels or prefixes to data
* Calculating totals and balances
* Deriving values such as GST, fees, rewards, or cashback

A complex object can be processed by making it **file-level** and associating it so it can be indexed across all template levels. This is achieved by adding an **Add Row** action at the Group Pre level.&#x20;

### Adding Computations to Simple Objects

Simple compound objects help you modify the data while processing. \
For example, if the template has a data object called "CUSTOMER\_NAME" and if it has unnecessary spaces, you can use "Trim" function and remove spaces. You can even add salutations using Prefix/Suffix.&#x20;

Let's see how to create a simple compound object.

* Access the **Data Mapper** tab in the right pane and navigate to **COMPUTED**. Then, click 'S' to create a simple object.&#x20;
* Give it a name and select the Data Type.

<mark style="color:green;">**<\<IMAGE>>**</mark>

* In the **Compound String Composition** wizard, click '+'&#x20;
* Select the data object, function (computation type) and configure the function settings, if required.
* Use prefix/suffix to add a prefix or suffix to the selected data object

Then. click **Compose** to view the result string.

<mark style="color:green;">**<\<IMAGE>>**</mark>

Similarly, you can add as many computations as required. Once done, click **Ok** to add.

### Adding Computations to Complex Objects

This is often used to merge the tables by adding row(s). Let's see how to create one.

Make sure to define the complex objects with the table data. Then only you can create a complex object.

* Access the **Data Mapper** tab in the right pane and navigate to **COMPUTED**. Then, click 'S' to create a simple object.&#x20;
* Give it a name, select the Type, and select the number of columns. <mark style="color:orange;">Accordingly, the system pulls the tables available with the given number of columns.</mark> Then, click **Ok**.
*   In the **Computed Complex Object Settings,**

    * Click **Add Row** and select the complex object to be merged.
    * To define the column association, click <mark style="color:green;">**\<icon>**</mark> in the **Column Mapping** and select the column.
    * To filter the data to be merged, click **Filtering.**
      *   In the **Filter Options**, expand the **settings** and select the entity.

          * In the **Merge By**, select the column and enable **Sorting** to sort the data.
          * Then, set the **Priority** and **Sort Mode** (Ascending/Descending)&#x20;

          Then, click **Ok** to apply filter.

    &#x20;       <mark style="color:green;">**<\<IMAGE>>**</mark>

{% hint style="info" %}
- You can merge the tables with equal number of columns.
- In the event, if you want to delete any row, navigate to it and simply click <mark style="color:green;">**\<Delete Icon>**</mark>.
{% endhint %}


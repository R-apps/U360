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

# Working with Simple Objects

The data input that holds only a single value are referred to as simple objects.

For example, assume building a template for an account statement containing the customer's name, account number, and more. As these hold only single value, these are referred to as simple objects.&#x20;

To insert the customer's name in the template, locate it in the input data (e.g., \<customer\_name>), then drag and drop it on to the template. \
<mark style="color:$success;"><\<IMAGE>></mark>\
Similarly, drag all the simple objects on to the designer.

As you add data objects to the template, the data mapper auto-structures your template data. To view, enable the **Data Mapper** from the View menu, it appears as a tab in the right pane. Double-click to access it.&#x20;

The other way around to create simple objects:

* Open the **Data Mapper** tab. Access **RAW > Input > Simple** and click '**S**'.
* In the **Create Simple Objects** wizard, expand and select the data object(s).

The selected simple objects are displayed as "S\_DATAOBJECT"

<mark style="color:green;">**<\<IMAGE>>**</mark>

{% hint style="info" %}
If you select the main identifier, all the simple objects are selected by default. You can uncheck the unwanted objects.
{% endhint %}

To modify any object's properties, open the **Data Mapper** tab and expand the **RAW > Input > Simple**. Double-click the element. The **Simple Object Properties** wizard appears. \
<mark style="color:$success;">**<\<IMAGE>>**</mark>\
Here, you can:

1. Change the element name and description
2. Change the data type, if required and compose an expression to perform a specific function \
   (e.g., trimming the extra spaces, removing duplicates, etc.) for the selected object. You can add prefix/suffix to that object if required. Then, compose it, the set expression is shown in "Result string". \
   <mark style="color:$success;">**<\<IMAGE/GIF>>**</mark>
3. Apply Transformation to encode or to decode or to transform the object value from Numbers to Words.

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

# Creating a Template

Make sure your have the requirements list handy and follow these steps to create a new template:

### Step 1:  Create a template

To create a template from scratch,&#x20;

* Log in to access the UniServe 360 Designer and click **New Template.**
* Give the template a unique name
* Select the page size and orientation

This creates a template and opens up the designer.&#x20;

### Step 2: Set up Template Settings

Before you start working with the template, specify the following for the system to process and generate the output.&#x20;

To specify, go to **Settings** menu > **Template Settings**

* [**Input**](configuring-input.md) (data source)
* [**Process**](./#process) (processing levels)
* [**Output**](configuring-output.md) (Expected output type generation)

### Step 3: Input the Data

{% hint style="success" %}
Keep the "Input Data" tab enabled in the right pane for easy access.
{% endhint %}

In the **Input Data** tab, browse and upload the input file (XML/JSON/DB/Text File) based on the data source type selected in the template settings. Once added, the data gets displayed and these \
(Text File-elements / JSON -keys / XML - tags) are referred to as "Data Objects."

<mark style="color:$success;">**<\<IMAGE>>**</mark>

### Step 4: Design the Template

In the **Layers** tab, a default structure is available - a Group (Group1) with a Page (Page1) and a Layer (Layer1) within it.&#x20;

<mark style="color:$success;">**<\<IMAGE>>**</mark>

For single page templates, you can straightaway proceed with designing the template. The template you design will automatically sit in the Page 1 in the Group 1. \
You can add as many layers as required.&#x20;

But if the template includes two or more pages, maintain a separate page for each.&#x20;

For additional pages, in the right pane, expand the **Pages** section and click '+'.

<mark style="color:$success;">**<\<IMAGE>>**</mark>

{% hint style="info" %}
* While structuring the template, place different sections in separate layers for better clarity. This helps you control visibility when generating output.
* You can rename the layers and pages for easy recognition. To rename a page, click <mark style="color:$success;">\<Edit></mark> icon. Rename it and make sure it is set to 'True' to keep it active.\
  <mark style="color:$success;">**<\<IMAGE>>**</mark>
{% endhint %}

Now, let's explore designing a template that contains a Header, Footer, and Body.&#x20;

1. First, create a basic template structure (E.g., Header, Body, etc.,) using the drawing objects. \
   Add logo, name, copyrights, contact information, and other branding elements in these sections. \
   To add these elements, use the drawing objects, image, and more. \
   You can even use individual layers for Header and Footer for more control.\
   Make sure you use this layer exclusively for these elements, so you can use it across the pages without having to design the same for each page.&#x20;
2. Next, we will create one or more layers for the Body section based on the requirement. Before heading to this section, understand the [simple objects](working-with-simple-objects.md) and [complex objects](working-with-complex-objects.md) and how to handle them
   1. Use drawing objects to create different sections in the body and set their look and feel using the respective properties.
   2. Then, to insert simple data such as mobile number or customer name from the input file, simply drag each field onto the template, positioning it as needed.
   3. Next, if your template involves any table, insert the table at the desired location in the template. Click it and access its properties to design the table as required. Once the table is ready, click the Data Association (<mark style="color:$success;">**\<icon>**</mark>) and select the required complex object. Click **Ok** to map.

{% hint style="info" %}
* To know more about objects and their properties, [click here](../../template-designer/objects-and-properties.md)
* If you want to insert a dynamic variable inside a paragraph without replacing or disturbing the surrounding text, use the **Rich Text** object and press **Ctrl + Insert** on your keyboard to map and place the variable.
{% endhint %}

Likewise, complete all the data to be inserted in the "Body" section. If the template includes more\
than one page, design the Body (main content) section in rest of the pages too.

Similarly, map the footer section.&#x20;

> Mapping any  to input data is not mandatory. You can skip this step if the footer is static or if the template does not include a footer section.

This completes the template designing process.

Once the template is ready, add business rules. For more information, [click here](../conditions-and-actions/).

The next steps include, [testing](../testing-a-template.md), [version check-in](../../version-control.md), and processing the template.

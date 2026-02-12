# Custom Indexing

Instead of updating the default job tables, you can define your own entities or tables and control exactly where and how metadata is written. In addition to database indexing, UniServe 360 also allows you to export indexed metadata into different file formats for downstream use.

This helps you track documents, support audits, and regenerate documents accurately, without storing static output files.

#### When to Use?

Use custom indexing when you

* need metadata outside the standard UniServe database.
* want to generate XML, CSV, or TXT outputs.
* require custom tables or entities for downstream systems, to have a better control over what data is captured and how.

#### How to Use?

To add custom index,&#x20;

* Go to **Settings** > **Distribution Options**. Expand and select **Custom Index**.\
  ![](<../../../.gitbook/assets/Custom Index - Navigation.png>)
* Expand it and select **Configure** (+) at the required processing level (File level/Level 1). \
  The **Custom Indexing** configuration screen appears.
* In the **Template Repository** pane, select **Add Template** (![](<../../../.gitbook/assets/Custom Index - Add Template Icon.png>)). Enter a template name and click **OK**.\
  ![](<../../../.gitbook/assets/Custom Index - Creating a template.png>)
* Expand **Template Information** and select the created template to access the configuration tabs on the right:\
  &#x20;             **Field setting** - define what to capture\
  &#x20;             **Composite setting** - Specify where the data goes
  * In the **Field setting**, map global objects to index fields or create custom fields based on business needs. To map,
    * Expand the **Defined** section&#x20;
    * Give the field a name, select the data type, and select the expected value. Add as many fields as needed. \
      &#x20;![](<../../../.gitbook/assets/Custom Indexing - Field setting (1).png>)
    * Similarly add&#x20;
      * custom fields -  for business-specific data&#x20;
      * reserved fields - for predefined or system-generated values.
  * To define where and how the indexed data is stored,&#x20;
    * Switch to **Composite Setting** tab and select **Add Composition Group** (+)
    * Enter the group name and select the template type (XML/TXT/DB)
    * <mark style="color:orange;">Should this template type be matched with the input data (source data file)?</mark>\
      ![](<../../../.gitbook/assets/Custom Index - New composite group.png>)
    *


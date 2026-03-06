# Prerequisites

**Template creation checklist**:

* **Capture all formatting requirements**, including layout, branding, visual elements, and Communications.
* **List the business rules** to be applied
* **Identify the data source** you will use as input.\
  This can be a Text file, an XML file, a JSON file or from a database.
* **Review the input file** to understand its structure.\
  Check whether it contains a single customer record or multiple customer records. For multiple records, select batch processing.
* **If multiple customer records are present**, determine the customer-level identifier.\
  For example, if the input is an XML file, `CUSTBREAK` is used for file and `SUBCUSTBREAK` for secondary level as identifiers.
* **Locate the start and end tags** that define each customer’s data segment.
* **Check the image format** before adding it to the template. Only JPG and PNG are supported.

Once these inputs are finalized, you can begin building the actual template.

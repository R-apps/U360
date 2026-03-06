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
---

# Multi-Processing Templates

A **Multi-Processing Template (MPT)** allows UniServe to process a template using multiple processors or workers. This improves throughput during large batch processing.

### Prerequisites

Before creating an MPT, ensure the following:

1. The template must be active and available on the server. \
   [Click here](../../all-about-templates/template-design-and-management/version-control.md) to understand how to add a template to version control.
2. The template must be mapped to a spool path for processing. To map,
   * In **Template Designer**, open the **Tools** menu.
   * Select **Template Settings**. Alternatively, press <kbd><mark style="color:$primary;">**CTRL+ALT+D**<mark style="color:$primary;"></kbd>.
   *   Select the **Spool** tab and configure the required spool path for the template.\
       <<mark style="color:orange;">Image - not available in Thin Client</mark>><br>

       <div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/unknown.jpeg" alt="" width="349"><figcaption></figcaption></figure></div>

### Configuring an MPT for User Process

To create an MPT,

* Select the IP address of the current system where processing will run.
* Under the **Process** field, right-click the IP address and select **Configure**. \
  The **Process Configuration** dialog box appears.
* Select **User Process**. The available processors appear in the right pane.
* Select the required processor(s).
* Enable the processor in the **Use** field.
  *   Enter the number of **workers** in the text box. Workers define the number of parallel processing instances.

      7. Right-click **User Process** and select **Create**.

      The **Create Multi-Processing Template** dialog box appears.

      8. Enter the **Template Name**.
      9. Enter a **Description**.
      10. Click **OK**.

      The MPT is created and appears under **User Process**.

      11. Right-click the newly created template.
      12. Select **Save**.
      13. Click **Upload**.

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

# Print Profile

Use Print profiles to define how documents are printed, grouped, and routed to printers.

To set up SMS profiles, go to **Settings** > **Print Settings.** Alternatively, press <kbd>Alt+P</kbd>&#x20;

Follow this two-step process to set up a new Print profile, and ensure you save the configuration after each step.

{% stepper %}
{% step %}
### Adding a new print profile

In the **Print Settings** dialog, select **Add Profile**. Use the **General** tab to define how print output is grouped, processed, and organized during batch execution.

#### Profile Name

Enter a unique name to identify the print profile.&#x20;

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/Print Profile - Profile Name.png" alt="" width="519"><figcaption></figcaption></figure></div>

#### **Print Strategy**

In the **Print Strategy** section,&#x20;

* Define how documents are printed:
  * **Individual Wise:** prints each document separately at the selected processing level
  * **Batch Wise:** prints documents in batches. Choose this for high-volume print jobs where documents are processed together.
* For batch wise, enter the **Batch size** to define how many documents are included in each batch.
* **Load sharing**: Enable this to to distribute print processing across available resources.  This improves throughput for large batch runs
* **Enable PostScript page data compression:** Enable this to compress PostScript page data during processing. This reduces output size and improves performance for large print jobs.
* **Output Folder Sequence Generation:** Enable this to tell UniServe 360 to create output folders in a defined sequence during batch processing.
* **Subfolder Identifier:** Specify a value to name or group subfolders within the output directory. Use this to logically separate output based on business or processing needs.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/Print Profile - Print Strategy.png" alt="" width="517"><figcaption></figcaption></figure></div>

#### Post Component Settings

Defines actions to be applied after document generation.

* Select **NONE** if no post-processing is required.
* Use other options to merge or process output components, such as PS or PDF files. \
  Click ![](<../../.gitbook/assets/image (11).png>) to define post component settings for the selected component.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/Print Profile - Post Component Settings.png" alt="" width="521"><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
### Printer Setup

Use the **Printer** tab to define how print load is managed during processing.

To add a printer,&#x20;

* **Printer Name**: Select the printer to be used for output.\
  Only printers that are configured in the system appear in the list.
* **Batch Size**: Specify how many documents are sent to the selected printer in one batch.
* **Copies:** Enter the number of copies to print for each document.
* **Priority**: Set the priority when multiple printers are configured. \
  A lower number indicates higher priority (1, 2, 3,...). UniServe 360 core routes print output based on this set priority sequence.

Then, select **Add Printer**. The printer appears in the **Selected Printers** list.

\<IMAGE>

You can add multiple printers to balance print load, set fallback printers, and control routing.

To remove a printer&#x20;


{% endstep %}
{% endstepper %}

{% hint style="info" %}
#### Tip for first-time users:

Start with a small **Batch size** with default **Post-component settings** using a single printer, generating a single copy.&#x20;

Once validated, you can configure multiple printers and optimize settings for higher volumes or advanced routing.
{% endhint %}

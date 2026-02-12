# Creating FGTs

FGTs (File Generation Templates) act as the final execution layer in document generation. \
They help you define the output format for the processed template and the storage path for the processed output.

To create a FGT,

* Go to **Settings** > **Distribution Options** or press <kbd>**Alt + t**</kbd>&#x20;
* In the **Document Level Settings** dialog,
  * Expand **Distribution Options**, and then select **File Generation Templates**.
  * Expand **Level 1,** and then select **Add** (+) in the **Actual** item. The platform creates an FGT \
    titled "Actual1." \
    ![](<../../../.gitbook/assets/FGTs without data.png>)\
    Select **Edit** (![](<../../../.gitbook/assets/Edit FGT.png>)) and give the FGT a meaningful name for easy identification.\
    <img src="../../../.gitbook/assets/Edit FGT Dialog.png" alt="" data-size="original">
  * Select **Actual1;** its configurable properties appear on the right.
    * **Filter** - select the required output format (PDF, PS, HTML, HTML5).\
      (Only formats that are already added as plugins appear in this list.)
    * **File name** - select a naming convention for the generated output.\
      This list displays all available global data variables.\
      If no option is selected, the system automatically generates the file name using the level name and a date–time stamp.
    * **Output path** - select the location (folder path) where the processed output should be stored.
    * **Active** - Check this property to keep FGT active for document distribution.
    * **Mode** - Select "Immediate" to start document distribution immediately after generation; else, select "Delayed" to convert the document to MOF and store it in the database for later use.
    * **Index** - Check this property to store the indexed data in the database for retrieval and search.
    * **Zipped** - Check this property to compress the generated output to reduce the file size. \
      &#x20;               Uncheck to keep the output in its original format
    * **Embedded images** - Check this property to include images in the output (recommended for print). Keep it unchecked to exclude images.
    * **Tray settings** - Use this property to define tray-switching commands that are embedded in the output file for print processing.
    * **Size validation** - Check this and add the condition to verify the processed file size\
      ![](<../../../.gitbook/assets/FGT - Size validation.png>)
    * **Watermark settings** - Use this property to include a watermark (text/image) in the generated output.\
      ![](<../../../.gitbook/assets/FGT - watermark.png>)
    * **Advance settings** - Use this property for output-specific options. These options vary based on selected output format.\
      For example, if the output format is PDF, you can add encryption and digital signatures at desired positions in the document, as required.\
      ![](<../../../.gitbook/assets/FGT - Advance settings.png>)

{% hint style="info" %}
<mark style="background-color:yellow;">File level / Level1 -</mark>&#x20;

<mark style="background-color:yellow;">Actual / Virtual - when and where to be used?</mark>
{% endhint %}

You can create multiple FGTs at Level 1 and Level 2 to control output behavior for different document sections.

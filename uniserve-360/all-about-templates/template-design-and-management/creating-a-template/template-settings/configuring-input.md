# Configuring Input

Input configuration is required for batch processes.

To define input, access the **Input** tab in the **Template Settings** dialog. Alternatively, press <kbd><mark style="color:$primary;">Alt+O<mark style="color:$primary;"></kbd>

* Click **Main Information** and specify the following details for the template to understand from where and how to read the input:
  * file name,&#x20;
  * how to identify data (identify either by input-path or keyword),&#x20;
  * action to perform on processed file,&#x20;
  * select the filename pattern, and&#x20;
  *   select if it should be applied to Daemon job. Always select "Yes" for batch jobs to process templates automatically when the data is available.<br>

      <div align="left" data-with-frame="true"><figure><img src="../../../../../.gitbook/assets/image (4).png" alt="" width="563"><figcaption></figcaption></figure></div>
*   Now, click '+' to add the source information. Click it and specify the input path in the right pane. This tells the template from where it should pull and process data. Always enable "Sub Folder" to locate the exact file from the input path.<br>

    <div align="left" data-with-frame="true"><figure><img src="../../../../../.gitbook/assets/image (5).png" alt="" width="563"><figcaption></figcaption></figure></div>

Then, select **Ok** to save the input configuration.

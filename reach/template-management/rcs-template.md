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

# RCS Template

This is a pre-defined format that lets you define what the message should look like and how users can interact with it. An RCS template can include text, branding, variables for personalization, and action buttons such as links or quick replies. Once created and approved, the same template can be reused across multiple campaigns to ensure consistency and faster execution.

### Creating a RCS Template

* Go to **Template Management** > **RCS Template** > **Create Template**.
* To control template ownership and reuse, choose who can access and use this template:
  * **All** - available to all users
  * **Sub User** - limited to assigned sub-users. Select sub user(s) to specify who can access it.
  * **Self** - available only to the creator (You)
* Next, enter the template details:
  * **Template Name**: Enter a clear, identifiable name for easy search and reuse.
  * **Template Type**: Select the template format (Standard/Rich Card/Carousel)
  * **Language**: Select the language in which the message will be sent.
  * **Aggregator**: Select the RCS aggregator configured for delivery.
  * **Bot**: <>
  * **Approval Status**: Current approval state of the template
* Next, compose the message content in the **Message** field. To personalize use **Add Variable** to insert customer-specific dynamic data. The character counter helps you keep your message within allowed limits.
* Finally, [add interactive elements](rcs-template.md#Adding_Interactive_Elements) if required. A live mobile preview on the right shows how the message and buttons will appear on a user’s device.

For **Standard** templates, preview and continue to **Save** the template.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure></div>

For **Rich Card** templates, these additional steps are involved:

* Select the card orientation (vertical/horizontal) and Media Height.
* Add media file (image/video) from the Assets folder:
  * For the available asset, select it and click **Insert**
  *   For a new asset, use **Upload asset** and give it a tag for easy identification. After uploading, select it and click **Insert** to use it in the template.

      <div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure></div>

      <div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure></div>

> To preview the uploaded media, click **Preview**. Use **Replace** to change the image.

* Enter the Card Title and Description.
* For **Carousel** templates, specify height and width for each card and follow the steps involved in designing each rich card within the carousel.

#### Adding Interactive Elements

To add interactive buttons that appear with the message, click **Add Button** and define the actions, as illustrated here.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure></div>

Include as many buttons as you need.

Finally, click **Save Template** once the template is ready. The template is then ready for approval and can be used in RCS campaigns.

> Even a standard template can be converted to a RCS template. Pick it and make it interactive by adding Rich Text and Interactive elements when creating a RCS communication.

### View Templates

All the RCS templates created to date are available here.

To view, go to **Template Management** > **RCS Template** > **View Template**

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure></div>

To preview a template, hover on it and click **View**.

To edit the template, hover on it and click **Edit**.

To search for a template, type the name in the search box and click **Search**.

If you do not require a template, hover on it and click **Delete**.

{% hint style="info" %}
Managing these templates are subject to the permissions assigned to you by your Administrator.
{% endhint %}

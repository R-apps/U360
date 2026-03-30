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

# Email Templates

Email templates are pre-designed email structures that include reusable content, formatting, and branding features, as well as placeholders for personalized specifics such as the recipient's name or special content, allowing for easy customization. They enable teams to quickly execute campaigns, ensuring all messages are consistent, and simply track responses or engagement across multiple emails.

This section holds a repository of all your email templates. The templates available here will be displayed when you attempt to choose a template while creating a communication.

### Permissions

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/Email Template Permissions.png" alt=""><figcaption></figcaption></figure></div>

## Create a New Email Template

* Navigate to **Template Management** > **Email Template** > **Create Template**. A visual HTML editor with a responsive grid appears.
* Begin by creating a layout. Navigate to the **Insert** tab where the required layout elements (Header, Footer, Page Break, columns, etc.) are available. Position your cursor on the email body and select the element to insert it.\
  For example, to insert a header, select the header element and choose the header type. It places the header. Then, to customize it, select the individual sections in it and make necessary changes.
* Set the typography (Font Type, size, color, and appearance) and compose the email content.

> Alternatively, use the **built-in AI content generator** to create content seamlessly. Go to **Advanced Tools** and click **Generative AI**. Provide it with the context, tone, communication channel, and the word limit (if any). Preview the generated content in **Template Preview**. Copy it to use and paste it in the editor. Then, make necessary modifications if required.

\<SCREEN>

After composing, click **Save** . To save the template,&#x20;

* Give it a name (File name)
* Select a tag to filter and identify it
* Select a category to store it in the repository
* Select the [permission type](email-templates.md#):
  * **All**: All users in your domain can use the template
  * **Sub User**: Only sub domain users can use the template
  * **Self**: Only You (the User) can use it

## Approval Process&#x20;



The saved template will be in the Draft mode and will not be available in the repository.

#### Sending a Template for Review

To send the template for review,&#x20;

* Navigate to the **Review** tab and click **Send For Review**.
* Select the reviewer(s) from the displayed list of reviewers, and then click **Send**. You can choose to send it to a single or multiple reviewers.

\<IMAGE>

Once the template is sent for review, reviewer(s) receive a notification.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (10) (1).png" alt=""><figcaption></figcaption></figure></div>

The template then moves from "Draft" state to "Review" state. To view the template, select and apply the "Review" filter.

### Reviewer Flow

You, as a reviewer, to review, access your notifications and click the "Review Request for Email Template" notification. The template opens in review mode with the options to comment, approve, reject, and end review.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure></div>

Upon reviewing, if the template:

* seems to be perfect, approve the template
* requires one or more changes, share your feedback as comments
* does not align to the goal, you may reject it.

The approved templates will then be sent to the publisher to publish it.

By default, users with the "**Admin**" role have full access to create, review, publish, and delete. Users with roles, who are granted "Publish" permissions, can choose to either publish it directly or to send it for review.

## Export Template

You can choose to export the template to reuse it for any similar email templates.

To export, click **Export**, you get the base template code with the option for you to input the content at required places such as, title, text, links, and others. Copy this code and save it in your local storage.

## View Templates

To view created templates, navigate to **Template Management** > **Email Template** > **View Template**.

Based on the permissions assigned, you can create, edit, and manage the email templates.

*   While searching for a template, you can choose to search by name or tags or categories. After selecting the search criteria, type in the search box, and click **Search**.<br>

    <div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure></div>
* To preview a template, click **View**.
* To edit a template, click **Edit**.
* To copy a template id, click **Copy**.
* To delete a template, click **Delete**.

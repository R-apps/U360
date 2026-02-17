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

# Mail Profile

A mail profile defines how emails are sent and what content customers receive.&#x20;

To set up SMS profiles, go to **Settings** > **Mail Profile.** Alternatively, press <kbd>Alt+M</kbd>&#x20;

Follow this three-step process to set up a new Mail profile, and ensure you save the configuration after each step.

{% stepper %}
{% step %}
#### Create a New Mail Profile

* In the **Mail Settings** dialog, click **Create mail profile**.
* Enter a **Profile Name** that clearly identifies the purpose of the profile.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/Create Mail Profile.png" alt=""><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
### Mail Settings

In the **Mail Settings** section, enter the following:

* Sender's email address
* Friendly name
* Email Subject (Is this the manual entry field or a drop-down?)
* Select the Time Zone.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/Mail Profile - Mail Settings.png" alt="" width="478"><figcaption></figcaption></figure></div>

#### Optional Settings

Use optional settings only if you want to specify to which email address users can reply t or to display the sender address.

* Select **Optional Settings** and check the required options as required:
  * Reply-to address
  * Sender address
  * Number of lines
* Click **Ok** to apply the configuration.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/Mail Profile - Optional Settings.png" alt="" width="480"><figcaption></figcaption></figure></div>

#### Message Settings (Compose email)

* Select **Message Settings**
* In the **Message Body** dialog, select the Mail Body Type (Plain Text / HTML).
* To compose email, you have these three options available. Choose the option as needed.&#x20;

{% tabs %}
{% tab title="New (From scratch)" %}
To compose an email message,

* Select **New** and compose the message in the body.
* For personalized content, use dynamic variables. Place your cursor at the desired position and select the data object.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/Mail Profile - Message Body.png" alt="" width="563"><figcaption></figcaption></figure></div>

After composing, **Save** your email message.
{% endtab %}

{% tab title="Import HTML" %}
Choose this option if you have your email message outside the platform in HTML format. To import,

* Select **Import** and locate the HTML file from the server path. The file content is placed in the email body.
* Personalize it with dynamic data, if needed.
* Finally, select **Save** to save the email message.
{% endtab %}

{% tab title="Compose using AI" %}
The Platform's in-built AI composes email message for you. To use,

* In the **Message Body** dialog, select **Auto Content**
* Select the Product name and its service in the Sub Product.
* Tell the context for which you want to communicate to user
* Select the tone and specify the word count.

Then, select **Generate**. The AI model generates the content in HTML and displays it in the **Content Preview** pane.&#x20;

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/Mail Profile - Auto Content AI.png" alt="" width="563"><figcaption></figcaption></figure></div>

Make necessary changes, if needed. Then, select **Import** to have it in the message body. Remove the tags and personalize, if needed.&#x20;

After composing the mail content, select **Save** to save it.
{% endtab %}
{% endtabs %}

#### Insert Images & Hyperlinks

* To insert an image:
  * Select **Image** or press <kbd><mark style="color:orange;">Ctrl+Alt+I<mark style="color:orange;"></kbd>
  * Select the image file (PNG / JPG / JPEG) and select **Open**
* To insert a hyperlink:
  * Select **Hyperlink** or press <kbd><mark style="color:orange;">Ctrl+Alt+H<mark style="color:orange;"></kbd>&#x20;

#### Attachments

* To add attachments,&#x20;
  * Switch to **Other** tab.
  * Select a **File Path** data objects or select **Browse File** to manually select the file to be attached.&#x20;

Attach as many files as needed.

Now, in the **Post Component Settings,** determine how UniServe 360 should handle the processed files.

Select the Post Component and specify whether the processed files to be sent as attachments or should they be deleted after mail.

<<mark style="color:orange;">UI is not available for the rest of this set up</mark>>
{% endstep %}

{% step %}
### SMTP Settings

After composing the message, specify the connection details to tell how UniServe 360 should connect to the email server.

In the **SMTP Mail Settings** section,&#x20;

* Enter the **Host name** or IP address.
  * Enter the **Port number**.
  * Select the **Encryption Type** (TLS / STARTTLS / SSL)
  * Select the **Authentication type** and enter the **Username** and **Password**&#x20;

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/Mail Profile - SMTP settings.png" alt="" width="479"><figcaption></figcaption></figure></div>

After setting up the mail profile, select **Ok** to save and close. The created profile now appears in the **Mail Profiles** list.
{% endstep %}
{% endstepper %}

### Manage Mail Profiles

To view a mail profile settings, click **Edit** (![](<../../.gitbook/assets/image (8).png>))

To view the email message, click **Mail Body** (![](<../../.gitbook/assets/image (9).png>))

To delete an unwanted mail profile, click **Delete** (![](<../../.gitbook/assets/image (10).png>))

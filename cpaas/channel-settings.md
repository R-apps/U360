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

# Channel Settings

These&#x20;

### **SMS**

Configure the SMS communication gateway(s) to establish a connection with the platform. This connection enables platform to send messages SMS text messages to the target audience.

If you are using multiple gateways, use **Add New Gateway** and configure them.&#x20;

Then save your gateway(s) configuration.

Similarly, configure the gateway(s) utilizing for promotional communications and OTPs.

<div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/Settings - SMS.png" alt=""><figcaption></figcaption></figure></div>

### **Email**

To enable outbound email communication configure SMTP-based email gateway(s) by providing the necessary credentials and sender-level details for Transactional, Promotional, and OTP communications.

To add a gateway, select **Add New Gateway** and all the gateways involved.&#x20;

<div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/Settings - Email.png" alt=""><figcaption></figcaption></figure></div>

Expand to setup each email gateway to connect your platform to the email gateway service. Additionally, specify "X SES Configuration Set" if email tracking is required, and choose the applicable Country to align with regional compliance policies.

Map each individual user using the **User List** and associated Department. Define the **SMTP From Email** address to be displayed to recipients and configure a valid **Reply-To** address to manage responses. Optionally, you can include an **Unsubscribe URL** to comply with email opt-out policies.

Use **Add** to add a user.

<div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/Settings - Email1.png" alt=""><figcaption></figcaption></figure></div>

Then, save the setting.

### **WhatsApp**

Add the gateway(s) enabled for WhatsApp communications.&#x20;

To add a gateway, select **Add New Gateway** and specify all the gateways involved.

Now, expand to configure each Aggregator. Start by selecting **Aggregator** and input pricing details for **WSP Outbound**, **Inbound**, and **Marketing** messages, if applicable.

Add each user entry by selecting the **User List**, assigning the appropriate **Department**, and specifying the **Authorization Type** and **Prefix**. Then, provide the **WhatsApp Business ID**, **Phone Number ID**, and **Authorization Key** received from Infobip. Fill in the required API endpoints, including the **API URL**, **Template Create**, **Get Template**, **Delete Template**, and **Media Upload URLs**. Finally, enter the **Username** and **Password** to complete authentication.

Use **Add** to add each user entry. Finally, click **Save** to apply the configuration for the selected users.

\<IMAGE>

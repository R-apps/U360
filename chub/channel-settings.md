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
  actions:
    visible: true
---

# Channel Settings

### **SMS**

Configure the SMS communication gateway(s) to establish a connection with the platform. This connection enables the platform to send SMS text messages to the target audience.

If you are using multiple gateways, use **Add New Gateway** and configure them.

Then save your gateway(s) configuration.

Similarly, configure the gateway(s) used for promotional communications and OTPs.

<div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/Settings - SMS.png" alt=""><figcaption></figcaption></figure></div>

### **Email**

To enable outbound email communication, configure SMTP-based email gateway(s) by providing the necessary credentials and sender-level details for transactional, promotional, and OTP communications.

To add a gateway, select **Add New Gateway** and configure all the required gateways.

<div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/Settings - Email.png" alt=""><figcaption></figcaption></figure></div>

Expand each email gateway setup to connect your platform to the email gateway service. Additionally, specify **X SES Configuration Set** if email tracking is required, and choose the applicable country to align with regional compliance policies.

Map each individual user using the **User List** and associated **Department**. Define the **SMTP From Email** address to display to recipients and configure a valid **Reply-To** address to manage responses. Optionally, include an **Unsubscribe URL** to comply with email opt-out policies.

Use **Add** to add a user.

<div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/Settings - Email1.png" alt=""><figcaption></figcaption></figure></div>

Then save the settings.

### **WhatsApp**

Add the gateway(s) enabled for WhatsApp communications.

To add a gateway, select **Add New Gateway** and specify all the required gateways.

Now expand to configure each aggregator. Start by selecting **Aggregator** and entering pricing details for **WSP Outbound**, **Inbound**, and **Marketing** messages, if applicable.

Add each user entry by selecting the **User List**, assigning the appropriate **Department**, and specifying the **Authorization Type** and **Prefix**. Then provide the **WhatsApp Business ID**, **Phone Number ID**, and **Authorization Key** received from Infobip. Fill in the required API endpoints, including the **API URL**, **Template Create**, **Get Template**, **Delete Template**, and **Media Upload** URLs. Finally, enter the **Username** and **Password** to complete authentication.

Use **Add** to add each user entry. Finally, click **Save** to apply the configuration for the selected users.

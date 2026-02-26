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

# Settings

The Administrator will have privileges to configure the application settings. Configure the channel(s) that you are using to send communications to your target audience. These settings are enabled based on the customer requirements.

To set, navigate to the **Settings** menu.&#x20;

Here is the list of settings to configure:

### **Transaction Key**

Generate a transaction key for your request API.

To generate, go to **Transactional Key** and click **Generate**.\
Use **Copy to clipboard** to copy the key.

<div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/Settings - Transactional Key.png" alt=""><figcaption></figcaption></figure></div>

### **WhatsApp Number**

If you are communicating your audience through WhatsApp channel, register the WhatsApp business number in Meta and enter it here.

<div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/Settings - WhatsApp Number.png" alt="" width="414"><figcaption></figcaption></figure></div>

### **Dashboards**

In case of more than one dashboard, choose which dashboard the user should access.

To permit user access to a specific dashboard, go to **Dashboard** settings and select the dashboard.

<div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/Settings - Dashboard.png" alt=""><figcaption></figcaption></figure></div>

### **Web Push**

To send **web push messages**, connect your web application to Firebase. It authorizes Reach to use your **Firebase Web project** to send push notifications to supported browsers such as Chrome, Edge, and Firefox.&#x20;

To connect,&#x20;

* Enter the **Firebase project Id**.&#x20;
* Provide the **Client Email** generated from the Firebase service account, to authenticate requests from Reach.
* Enter the **Client key** associated with the service account, to securely authorize message delivery.

Then, save the details to connect.

<div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/Settings - Webpush.png" alt=""><figcaption></figcaption></figure></div>

### CPaaS Settings

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

### **App Push**

To set push notification for an app, connect your mobile application with Firebase so Reach can send app push notifications reliably without additional setup. To connect, add Firebase credentials for Reach to securely communicate with your mobile app and deliver notifications such as alerts, reminders, and updates in real time.&#x20;

To set up,&#x20;

* Give the Firebase connection a unique **Name**
* Specify Firebase details - **Project Id**, **Client Email**, and **Client Key**.&#x20;
* Select the **Mobile App** for which this firewall setup applies.
* &#x20;Upload the Application Certificate to establish a secure connection between Reach and Firebase.

<div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/Settings - App push.png" alt=""><figcaption></figcaption></figure></div>

Finally, **save** your settings.

For multiple Firebase configurations, use **Add**. Only one Firebase configuration is active per mobile app. Each Firebase setup is saved independently and selected based on the mobile app you associate it with.

### **Voice**

To enable automated voice calls for transactional alerts, promotional messages, or OTP notifications, configure this setup.

To setup,

* Select the message type  for which you are enabling voice communications
  * **Transactional** - for service-related or mandatory communications such as account alerts or payment confirmations
  * **Promotional** - for offers, campaigns, or awareness calls, subject to regulatory guidelines
  * **OTP -** for one-time password delivery for authentication or verification
* Select the **Aggregator** (voice service provider) and set up the following server details
  * **Authentication Key** - provided by the Aggregator
  * **Voice Language** - in which the voice message will be played
  * **Voice Server Number** - the caller Id from which the calls are placed
  * **Voice Server URL -** API endpoint URL shared by the voice service provider

Then, save the configuration.

<div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/Settings - Voice.png" alt=""><figcaption></figcaption></figure></div>

### **IVR**

Choose the message type ((Transactional / Promotional / OTP)&#x20;

Select the **Aggregator** and set up the following server details to enable voice communications :

* **IVR Server Authentication**, provided by the IVR service provider
* **IVR Server Number**
* **IVR Server URL**

Then, save the configuration.

<div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/Settings - IVR.png" alt=""><figcaption></figcaption></figure></div>

### **Fallback API**

Configure Fallback API when you orchestrate a specific journey involving fallback communication.

To configure, select the channel and click '+' to add itl. Add all the channels in the same order as how you want the journey to fallback to next available channel.&#x20;

Then, specify the wait time for each channel before the system switches to the next available channel.

Finally, save the configuration.

<div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/Settings - Fallback API.png" alt=""><figcaption></figcaption></figure></div>

### **Delivery**

Set all your communication delivery settings here, either for promotional or transactional.

To set,&#x20;

* Select the communication type (transactional/promotional)
* To configure DND settings, select the time and days of week.
* To skip delivery on specific date(s), enter them and click **Add** to include more.
* To keep a message in the queue for a specific time, use the QUEUING option.

<div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/Settings - Delivery.png" alt=""><figcaption></figcaption></figure></div>

Similarly, switch to **EMAIL**, **WHATSAPP**, **VOICE**, **APP PUSH**, and **RCS**, and configure the necessary settings for respective channels.

Once done, select **Submit** to save the settings.

Further, you can choose to limit the number of communications (such as an email, SMS) within a defined time period. This helps prevent spamming, ensuring a better user experience.

Once the limit is reached, no further messages are sent to users until you reset the cap.

To cap your communication frequency, switch to **Frequency Capping** tab and set the cap for each channel. Once done, select **Submit** to save your settings.

<div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/Settings - Frequency Capping.png" alt=""><figcaption></figcaption></figure></div>

### **Survey**

Surveys help you gather feedback, usually after an interaction. Use surveys to analyze customer experience, product experience, or service quality, influencing future journeys.

To use the segment columns,

Select the data source (Contact Table/CSV File)

Then, select the file. The application fetches the columns available in it.

Choose the column(s) you prefer to use in your survey and click **Move**.&#x20;

Select the column(s) in the **Selected Columns**. &#x20;

Finally, click **Save** to insert the data.



### **Forms**

Use form(s) at specific stages of a user journey to collect users' responses or requests such as contact preferences, service interests, or feedback from the customer. These forms serve as interactive check points, enhancing user journey.




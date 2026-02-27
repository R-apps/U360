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

# App Nudges

Nudge campaigns are subtle and indirect techniques to influence customer behavior. Nudges help you encourage your app users to take a specific action at the right moment. By analyzing user behavior, nudges can be sent at optimal times to encourage actions like completing a purchase, filling out a form, or participating in an event.

Nudges can be easily integrated into any app, whether it is Android or iOS.

**Prerequisites**

1. Mobile App
2. Device brands
3. Nudge template(s)

### Steps to Create an App Nudge

{% stepper %}
{% step %}
#### Create App Nudge

Navigate to **Nudge** > **App Nudges** > **Create App Nudge**

1. Give the nudge a name and select the target mobile application
2. Enter a brief description and click **Create.** A nudge is created with a unique ID and directs you to the audience selection page.
{% endstep %}

{% step %}
#### Audience Selection

Next, select the audience. You can select the audience in any of these ways:

&#x20;**i. Custom Query**

Choose this option to fetch the audience using a query.

\<Not working>

\<Image>

&#x20;**ii. Contact**

Choose this method to select the audience from the contact (s) stored in a database.&#x20;

This option is only available if you have the Database permissions. You can create or add an exclusion list only if your administrator grants the necessary permissions .&#x20;

To choose this option,&#x20;

* Click **Add New Condition**, select **Contact**, and click **Add**
* Select the Data Source and Query Type
* Then, build the necessary conditions to fetch the required audience.

\<Image>

Similarly, you can add multiple conditions using AND/OR operators and fetch the required record count.

&#x20;**ii. App Event**

To choose this option,&#x20;

* Click **Add New Condition**, select App Event, and click **Add**
* Select the Data Source and Query Type. (Here, the data source is referred to as events like click to actions in different pages in an app)
* Then, build the necessary conditions to fetch the required audience.

\<Image>

**iii. Mobile Devices**

Choose this option to filter the audience using different mobile brands with different OS versions.

To choose this option,&#x20;

* Click **Add New Condition**, select Mobile Devices, and click **Add**
* Then, build the condition(s) to fetch the required audience.&#x20;

In the case the OS upgrades to a newer version, that will be auto-captured and displayed here.

**iv. All**

Choose this option to send nudge notifications to the audience using Android devices, or iOS devices, or both.

To choose this option,&#x20;

* Click **Add New Condition**, select All, and click **Add**
* Then, select the OS versions (Android, iOS, or both)

If you want to send nudge notifications only to people who already have the target app, you can choose the **Static** option.\
Use **Dynamic** to send notifications to all users, even new ones who installs the target app during the campaign.

After selecting the audience, click **Save & Continue**.
{% endstep %}

{% step %}
#### Configure Nudge Notification&#x20;

Next, configure how and where the nudge notification is to be displayed. To configure,

1. Click **Browse Template**, you see a range of nudge templates, including tooltips, coachmarks, beacons, spotlights, and more. Choose a template based on how you want to display your nudge communication on your app screen.
2. Configure the nudge display settings, such as appearance, position, action buttons, and more. Let's see configuring a beacon template.
   *   In the **DISPLAY SETTING** tab, select the screen and the screen attribute As they vary between Android & iOS, toggle the mobile screen editor to get the preferred view and configuration settings. Then, select if it has to be displayed single or multiple times If you select multiple times, enter the count to tell how many times it should be displayed. Enable "Don't show notification once dismissed" option, to allows users to dismiss the notification and prevent it from appearing again.

       \<Image>
   *   In the **LAYOUT** tab, adjust the notification position and appearance. To add a background image, select it from the resources. If you don't find the one, you can create and upload in the Assets Management section, if you have the necessary permissions.

       \<Image>
   *   In the **TEXT** tab, insert the notification message and adjust its appearance such as font style, color, alignment, padding, margin, position, and others.

       \<Image>
   *   In the **BUTTONS** tab, you can include buttons to enable users to take specific action from your notification message. (A maximum of 2 buttons can be included). To add a button, enter the button text and specify what action it should take upon clicking it. (In case of all mobile devices, specify the actions separately for Android and iOS)

       \<Image>
   *   In the **ARROW** tab, set the arrow position to point exactly the target screen element.

       \<Image>
   *   In the **BEACON** tab, adjust the beacon color, position, and pointer margin.

       \<Image>

These parameters vary for each template type, configure them accordingly. As you make changes, you get a live preview in the mobile app editor.

After configuring the nudge, click **Save & Continue**.
{% endstep %}

{% step %}
#### Publish Nudge

Then, select the start date, and click **Publish** to publish the nudge.

To automatically turn off the nudge notifications after certain time, select the end date before publishing.

View the published nudge at **Nudge > App Nudges > View Mobile App Nudges**.
{% endstep %}
{% endstepper %}

### Manage App Nudges

To view the nudges, navigate to **Nudge > App Nudges > View Mobile App Nudges**. The application displays the nudges you created to date.&#x20;

<div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/View App Nudges.png" alt=""><figcaption></figcaption></figure></div>

Furthermore, you can choose to edit or delete these communications as required.

* To execute a nudge campaign, click ![](<../.gitbook/assets/Play or Execute icon.png>).
* To edit a nudge, click ![](<../.gitbook/assets/Edit icon.png>), and update it.&#x20;
* To delete a nudge, click ![](<../.gitbook/assets/Delete CSV Data.png>).

Executed campaigns cannot be edited.

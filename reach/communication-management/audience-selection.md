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

# Audience Selection

This article explains how to select audience when creating a communication irrespective of the communication channel.

You can select audience from any of the four ways - Contact / CSV / Segment / Map

\<IMAGE>

{% stepper %}
{% step %}
### CSV

Choose this option to select customers from a local CSV file.

Select the required CSV and create the condition to select the audience. If you opt to send communication to:

**All the contacts**: select any attribute, set the condition as “Not Equal” to ‘0’, and \
click **Fetch Count**. This displays the total count of all the contacts in that CSV, as illustrated below.

\<IMAGE>

**Specific users**: Use Condition Builder to select the specific audience. Select the attribute, add the required condition, and provide a value to check the condition. Then, fetch the count.

\<IMAGE>

Similarly, you can add multiple conditions using AND/OR operators. This helps you in running the campaign exclusively to the required contacts.

To view the audience list, click **Download Result**. The list gets downloaded to your local storage in Excel.
{% endstep %}

{% step %}
### Contact

Choose this method to select the audience from the contact(s) stored in a database.

Select the data source and build the necessary condition(s) using AND/OR operators to fetch the required or all records.

Further, to exclude unnecessary contacts, check **Do You Want To Add Exclusion List** option, and select the exclusion list, as shown in the illustration below.

\<IMAGE>

{% hint style="info" %}
This option is available only if you have the Database permissions. You can create or add the exclusion list only if your administrator grants the necessary permissions.
{% endhint %}
{% endstep %}

{% step %}
### Segment

Choose this option to fetch the audience categorized into different segments. Select the segment and save your communication. Add an exclusion list, if required.

Then, fetch the count to get the audience count.

\<IMAGE>
{% endstep %}

{% step %}
### Map (Location-wise users)

Choose this option to select the audience within a specific location.

Use the shapes available on the map to locate the area and fetch the count, as illustrated below.

\<IMAGE>
{% endstep %}
{% endstepper %}

After selecting the audience, click **Save & Continue**.

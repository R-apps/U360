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

# User Management

We, the REACH team (Super Admin) creates an admin account for each customer (tenant), enabling them to onboard their team assigning necessary permissions to modules based on their users' roles, ensuring role-based access control (RBAC).

### Onboard User(s)

To onboard a new user,

* Go to **User Management** > **Create New User**
* Enter the user’s details such as Name, Email, Mobile No., Department, Password, and Address.

<div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/Create User.png" alt=""><figcaption></figcaption></figure></div>

#### Assign Permissions

Permissions are grouped by modules and channels (for example: Dashboard, UniServe Editor, RNLI Data Rule Engine, SMS, Email, RCS, Print, and more). Grant access to one or more actions based on the user’s role.

* To assign permissions to the user,&#x20;
  * Switch to the **User Permissions** tab&#x20;
  * Select the module or channel in the left pane and enable necessary permissions \
    (View, Create, Edit, and Delete).

{% hint style="info" %}
Use **Select All** option to enable all the actions.
{% endhint %}

<div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/User Access Permissions.png" alt=""><figcaption></figcaption></figure></div>

After assigning permissions, click **Create User**.

The user account is created along with a unique client Id.

#### View Onboarded Users

To view onboarded users, go to **User Management** > **View Users**. The application displays a list of onboarded users to date.

<div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/View Users.png" alt=""><figcaption></figcaption></figure></div>

The created user’s account status remains inactive by default.

#### Manage Users

To activate a user, click ![](<../.gitbook/assets/Activate User.png>), and provide confirmation on the displayed pop-up. Only activated users can access the application.

To make a user inactive, click ![](<../.gitbook/assets/Inactive User.png>) .

To delete a user account, go to **User Management** > **Delete User**. Navigate to the user you wish to delete and click ![](<../.gitbook/assets/Delete User.png>). Then, click **Confirm** on the displayed pop-up.

<div align="left" data-with-frame="true"><figure><img src="../.gitbook/assets/Delete Users.png" alt=""><figcaption></figcaption></figure></div>

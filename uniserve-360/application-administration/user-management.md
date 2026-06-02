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

# User Management

This section explains how administrators manage **users**, **roles,** **groups**, **security**, and **organizations**. and control users' access to different modules.

To access, go to **Admin** > **User Configuration**. Alternatively, press <kbd><mark style="color:$primary;">Alt+U<mark style="color:$primary;"></kbd> The **User Manager** module opens in a separate tab.&#x20;

The default user is **Administrator.**

Before creating a user, create organizations, roles, roles-to-modules, so you can map them to the user while creating.

### Organizations

To create an organization,

* Select **Organizations** from the menu and select **Create Organization.**&#x20;
* Enter a unique name and brief description. Then, select **Save**.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/Create organization.png" alt="" width="499"><figcaption></figcaption></figure></div>

The organization gets created and appears in the Organizations list with the status "Active".&#x20;

To activate/deactivate an organization, select **Edit** (![](<../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png>)), change the status and select **Save**.&#x20;

### Roles

To create a role,

* Select **Roles** from the menu and select **Create Role.**&#x20;
* Enter a unique name and brief description. Then, select **Save**.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/Create Roles.png" alt="" width="498"><figcaption></figcaption></figure></div>

The role gets created and appears in the Roles list with the status "Active".&#x20;

To change a role's status to active/inactive, select **Edit** (![](<../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png>)), change the status and select **Save**.&#x20;

### Set Access Permissions to Role

To set access permissions to a role,

* Select **RoleToModule** from the menu and select **Create Role To Module.**&#x20;
* Select the role, then choose the module(s) to grant access to users assigned that role.

Then, select **Save**.

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/Create RoleToModule.png" alt="" width="500"><figcaption></figcaption></figure></div>

### Create Users

To create a user,

* Select **Users** module from the menu and select **Create User**.
* Provide the following details:
  * **Username**: Enter the user's email id
  * **Password**: Set a password for the user to log in
  * **Organisation**:  Select the organization from the list
  * **Role**: Select the user's role from the list

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1).png" alt="" width="548"><figcaption></figcaption></figure></div>

Then, select **Save**. This creates the user and appears in the users list with the status "Active".

To view the created user's details, click ![](<../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1).png>).

To edit the user details, click ![](<../../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1).png>). Make necessary changes and then select **Save**.

To deactivate a user, click ![](<../../.gitbook/assets/image (3) (1) (1) (1) (1).png>), and select **Yes** on the displayed confirmation dialog.

### Groups

To create a group,

* Select **Groups** module from the menu and select **Create Group**
* Enter a unique name and description

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (4) (1) (1) (1).png" alt="" width="501"><figcaption></figcaption></figure></div>

Then, select **Save**. This creates a group and is listed in the Groups list with the default status "Active".

### GroupsToUsers

To add users to groups,

* Select **GroupsToUsers** module from the menu.
* Select a group from the displayed list of groups. Then, select the user(s) to be grouped.&#x20;

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (41).png" alt="" width="497"><figcaption></figcaption></figure></div>

If user(s) are to be a part of more than one group, you can select the required groups at a time and add users.

### Register Database

To use or connect to a database, you need to register it.

To register a database,

* Select **Register database** in the menu and select **Create Database**
* Enter the following database details to let UniServe connect to it:
  * Connection Name
  * Address
  * Database Type
  * Schema
  * Username & Password

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (42).png" alt="" width="512"><figcaption></figcaption></figure></div>

Then, select **Save**. The database gets registered and is displayed in the DB list.

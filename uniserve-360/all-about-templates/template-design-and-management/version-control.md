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

# Version Control

Version History helps teams understand what changed, when it changed, and why. \
In UniServe 360, every update is tracked, allowing teams to collaborate safely, avoid overwrites, and maintain a clear audit trail of template changes.

With Version Control, you can:

* Store locally created templates on the server
* Save edits as new versions
* Fetch the most recent version from the server
* Continue work without server connectivity
* Review earlier versions and restore them when required

> **Note:** You can make one or more versions active at a time.

### Checking in a Single Template

When a template is ready, you can add it to Version Control.

To add a template to version contro&#x6C;**,**&#x20;

1. Save the template locally.
2. Go to **Version Control > Check In**. Alternatively, press <kbd><mark style="color:$primary;">Alt+I<mark style="color:$primary;"></kbd>
3. Add comments describing the changes for clarity and traceability. \
   E.g., "Initial commit," "Updated UI," or "Fixed bug #123."
4. Mark this version as the active one (optional).
5. Then, click **Check In** to complete the action.

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/image (36).png" alt="" width="318"><figcaption></figcaption></figure></div>

Each check-in automatically creates a new version of the template. Once added, the template is stored on the server and becomes available for controlled access.

### Bulk Check-in

Check in multiple templates at once.

Instead of opening and checking in templates individually, you can select multiple templates and perform a single check-in operation.

For bulk check-in,

*   Select **check-in** button and select the templates.<br>

    <div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Bulk checkin - Select templates.png" alt="" width="461"><figcaption></figcaption></figure></div>
*   Next, select the server, and add a check-in comment.<br>

    <div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Bulk checkin - Server selection.png" alt="" width="461"><figcaption></figcaption></figure></div>

Then, select **Check-in \<n> Templates**

This feature is particularly useful after template updates, migration activities, or bulk development changes where several templates need to be committed together.

#### Admin-controlled Bulk Check-in

This allows users with 'Administrator' or 'Super Administrator' permissions to check in multiple templates at once without opening each template individually.

This feature helps organizations streamline release activities by centralizing template check-in while allowing template designers to focus on development.

> **Note**: Administrators can perform bulk check-in operations but cannot modify the design or content of templates unless they have been granted the required design permissions.

### View Version History

Every checked-in update is stored as a separate version. You can view the version history of the currently opened template. To view the version history of a template, open it in the editor and go to **Version Control** > **Show History**. It displays the version number, checked-in date, status, comments, and actions to read or make it active.

Alternatively, press <kbd><mark style="color:$primary;">Alt+E<mark style="color:$primary;"></kbd>

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/version history.png" alt=""><figcaption></figcaption></figure></div>

#### Setting a Version Active

If multiple versions exist, you can explicitly choose which one should be used for processing.

Select the required version and click **Set Active** to make it active. To view, use **Get.**

> If changes are detected, the platform prompts you to either check-in the changes or overwrite them with the selected version. Overwriting will discard all your changes.

{% hint style="info" %}
To quickly get a latest version of a template when working collaboratively, open it in the editor and use the short key (<kbd>Alt + V</kbd>), else, go to **Version Control** > **Get Latest Version**
{% endhint %}

#### Rolling Back to an Earlier Version

If a newer change needs to be undone, you can restore an older version.&#x20;

When you roll back to an older version,&#x20;

* The selected version becomes the working version.
* You can continue editing and check in again as a new version.

This is useful when correcting errors or reverting unintended changes.

### Working Offline

UniServe 360 allows you to edit templates without server access.

**Offline mode behavior:**

* Changes are saved only on your local system.
* Server versions remain unchanged until you check in.

This is helpful when working with limited connectivity or during isolated testing.

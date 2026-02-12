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

#### Adding a Template to Version Control

When a template is ready, you can add it to Version Control.

To add a template to version contro&#x6C;**,**&#x20;

1. Save the template locally.
2. Go to **Version Control > Check In**.
3. Add comments describing the changes for clarity and traceability. \
   E.g., "Initial commit," "Updated UI," or "Fixed bug #123."
4. Mark this version as the active one (optional).
5. Then, click **Check In** to complete the action.

<mark style="color:green;">**<\<IMAGE>>**</mark>

Each check-in automatically creates a new version of the template. Once added, the template is stored on the server and becomes available for controlled access.

### Viewing Version History

Every checked-in update is stored as a separate version. You can view the version history of the currently opened template. To view the version history of a template, open it in the editor and go to **Version Control** > **Show History**. It displays the version number, checked-in date, status, comments, and actions to read or make it active.

<mark style="color:green;">**<\<IMAGE>>**</mark>

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

<mark style="color:orange;">**Queries:**</mark>

1. <mark style="color:orange;">Can we lock/check out a template to restrict editing?</mark>
2. <mark style="color:orange;">When we roll back to an earlier version and make changes and commit, how does it impact the versions available next to the restored version?</mark> \ <mark style="color:orange;">(E.g., rolling back to v 5.0—make changes and check in. What version does it become, and how does it impact the versions from v 1.0 to v 4.0? Will those be overwritten?)</mark>

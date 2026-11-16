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
    visible: false
  anchors:
    visible: true
---

# Website Scanner

The **Website Scanner** enables administrators to register organizational domains and run manual or automated scans to detect active cookies and third-party tracking scripts before classifying them for consent management.

The summary metrics displays the real-time posture of all registered websites.

* **Total Websites**: The total number of domains configured for scanning.
* **Cookies Discovered**: The cumulative count of cookies detected across all scanned sites.
* **Unclassified Cookies**: The number of discovered cookies pending category assignment.
* **Last Scan Date**: The date and timestamp of the most recently completed scan.

<div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Website Scanner.png" alt=""><figcaption></figcaption></figure></div>

### Registering a Website

* Select **+ Add Website**
*   In the **Add Website** dialog, enter the following details of the website to be registered:

    * Display name for the website
    * Website URL
    * Scan Frequency: Choose how often the platform should automatically scan the website (Manual, Daily, Weekly, or Monthly).
    * Status: Active or Inactive.

    Then, select **Create Website**. The platform registers the webiste and prompts for the confirmation whether to launch an initial scan immediately or skip to run it later from the website card. <br>

    <div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Website Scanner - Add website.png" alt=""><figcaption></figcaption></figure></div>

Registered websites appear as cards (or rows in List view) showing their active state, configured scan frequency, last scan timestamp, and last scan status (COMPLETED or FAILED).&#x20;

### Scan and View Results

Locate the website card and select **Start Scan**. The platform starts the scan and displays the progress. Once a scan finishes, the **Scan completed** modal displays a summary of findings for that website:

* **Cookies discovered**: Total cookies identified during the scan.
* **Scripts discovered**: Total tracking scripts detected.
*   **Discovered scripts table**: Lists each detected script's Provider, Category (defaulting to _Unclassified_ until mapped), and URL / Snippet.<br>

    <div align="left" data-with-frame="true"><figure><img src="../../../../.gitbook/assets/Website Scanner - Scan website.png" alt=""><figcaption></figcaption></figure></div>

Select **View in Cookie Inventory** to inspect and classify the newly discovered items in the \
Cookie Inventory.

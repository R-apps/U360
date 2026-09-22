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
  anchors:
    visible: true
---

# Privacy Risk Dashboard

The **Privacy Risk** dashboard provides a consolidated view of privacy risks identified across the organization's privacy-related activities and configurations. The dashboard highlights the areas where privacy risks may exist, require review, or need remediation.

This dashboard helps you understand the&#x20;

* organization's current privacy risk level, identify critical risks,&#x20;
* review high-risk data processing activities and vendors,&#x20;
* track pending assessments, and
* monitor risk reduction over time.&#x20;

The dashboard also provides AI-assisted recommendations to help prioritize actions based on the current privacy posture.

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Privacy Risk Dashboard.png" alt=""><figcaption></figcaption></figure></div>

Let's understand how each insight helps:

* **Risk Snapshot**—This section helps you quickly understand the factors contributing to the current privacy risk level such as high-risk activities, pending DPIAs, visible and hidden sharing partners, and changes in risk areas.
* **Priority Gaps**—This section lists unresolved risk areas that require attention. Each gap includes a priority level, such as Critical, High, or Medium.
* **Risk Heatmap**—This heatmap provides a visual view of privacy risk across business processes and risk areas, such as Data, Consent, Vendor, DPIA, Retention, and Incident. \
  The color of each indicator represents the relative risk level for the corresponding area.

> **Note:** The risk levels shown by the colors are based on the risk scale configured for the platform.

* **Risk Trend**—This chart shows how the overall privacy risk score changes over the selected period.
* **High-Risk Assets**—This section lists sensitive data processing activities that may require additional risk assessment or controls. It can include activities involving personal or sensitive information, such as identity-related data, payment information, or customer information.
* **Pending DPIAs**—A DPIA (Data Protection Impact Assessment) is an assessment used to identify and evaluate privacy risks associated with a data processing activity. The **Pending DPIAs** section lists assessments that are ready to be started or are awaiting completion.
* **Consent Risk**—This section provides a view of consent-related risk based on the current consent configuration. It shows the distribution of consent settings, such as active and visible options, hidden or inactive options, and default settings.
* **Vendor Risk**—This section provides an overview of the privacy risk associated with third-party vendors or sharing partners.
* **Incident Trend**—This chart depicts the number of privacy-related incidents recorded over the selected period.
* **Mitigation Progress**—This chart helps you monitor progress in addressing privacy risks and identify items that remain open. It compares completed and open mitigation activities over time.

Use the filters at the top of the dashboard to focus the displayed information on a specific scope. Select **Reset** to clear the selected filters and return to the default view.

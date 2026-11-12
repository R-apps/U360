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

# Trust Graph

Trust Graph™ provides a visual representation of how privacy-related records are interconnected across your organization. It helps you trace personal data flows, understand dependencies, and assess the potential impact of changes to privacy configurations.

It maps relationships between privacy entities, including Records of Processing Activities (RoPA), consent categories, data fields, purposes, system integrations, sharing partners, notices, policies, and risk assessments.

To access Trust Graph,&#x20;

* Go to **Privacy Foundation** > **Trust Graph** in the left menu.&#x20;
*   It displays the total tracked records across entity types, and the number of records under each privacy area.&#x20;

    <div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Trust Graph.png" alt=""><figcaption></figcaption></figure></div>
* Select an entity, such as **RoPA**, **Consent Category**, **Data Field**, or **System Integration**.
*   Select **Stats** to view the connected nodes, relationships, associated policies, systems, third-party integrations, and consent categories.<br>

    <div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Trust Graph - stats.png" alt=""><figcaption></figcaption></figure></div>
* Select a record to open its relationship. The selected record becomes the central node of the graph. Its connected records appear as branches, showing how different privacy entities relate to one another.
*   To view record details, select any node. Its details are displayed in side panel such as its status, reference ID, owner, retention period, purpose, and linked records.<br>

    <div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Trust Graph - record level analysis.png" alt=""><figcaption></figcaption></figure></div>

### Graph Actions

* **Diagram View**: Displays relationships as a visual graph.
* **List View**: Displays connected records in a structured list for easier review.
* **Group Connectors**: Groups relationships of the same type to simplify the graph.
* **Search Graph**: Searches for records and highlights matching nodes.
* **Options**: Provides graph display and filtering options, including entity visibility and connector grouping.
* **Refresh**: Reloads the graph data to display the latest available relationships.

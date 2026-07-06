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

# QC Module

The QC (Quality Control) Module adds an approval layer to the communication lifecycle in UniServe 360. It enables designated reviewers and approvers to validate communications before they are delivered to customers.

The module is particularly useful for organizations operating in regulated industries such as insurance, banking, financial services, telecommunications, and utilities, where communications often require business, compliance, legal, or regulatory approval before distribution.

The QC Module is provided as a separate web application and can be integrated into the UniServe 360 communication workflow. It supports role-based access control (RBAC), allowing organizations to define who can view, review, approve, reject, or manage communication records.

#### Key Benefits

* Helps ensure regulatory and compliance adherence.
* Prevents unauthorized or incorrect communications from reaching customers.
* Supports controlled access through user roles and permissions.
* Enables faster review through bulk operations.
* Provides visibility into approval and rejection status.

## QC Process Overview

When UniServe 360 generates a communication request, the communication can either be sent directly for delivery or routed through the QC approval process, depending on the configuration.

The QC Module acts as an approval checkpoint between communication generation and communication delivery.

When UniServe 360 generates a communication request, the communication can either be sent directly for delivery or routed through the QC approval process, depending on the configuration.

When configuring a template,

* **If QC is enabled**, the communication waits for approval before being delivered. Once approved, the communication proceeds to the configured delivery channel.
* **If QC is not enabled**, the communication is processed immediately after generation.

## Roles and Access Control

A role defines the actions a user can perform within the QC Module. It controls access to features, records, and approval activities based on the user's responsibilities.

Permissions are assigned to roles, and users are mapped to one or more roles to determine their level of access within the application.

Permissions can be configured to control:

* Access to letters
* Record visibility
* Approval rights
* Rejection rights
* Bulk operations

## Understanding QC Terminology

The QC Module uses the following terminology:

<table><thead><tr><th width="199.55548095703125">Term</th><th width="449.55560302734375">Description</th></tr></thead><tbody><tr><td>Letter</td><td>A communication template or communication type that requires review and approval.</td></tr><tr><td>Record</td><td>An individual communication request generated for processing under a specific letter.</td></tr><tr><td>Reviewer / Approver</td><td>A user authorized to validate and approve or reject communications.</td></tr><tr><td>Approval Status</td><td>Indicates whether a communication record is Pending, Approved, or Rejected.</td></tr></tbody></table>

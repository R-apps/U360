# On-Demand Document Generation

UniServe 360 allows users to generate documents instantly for a single customer or transaction, exactly when it is needed. It helps generate documents in real time using the same approved templates and rules.

Use on-demand generation for time-sensitive or customer-initiated documents, such as instant account statements, policy documents, premium payment receipts, and more.

**Example**: When a customer logs in to net banking and clicks “Download Mini Statement,” UniServe 360 helps generate the statement instantly using live account data.

#### Generating an On-Demand Document

Let us understand this with an example—when a customer requests a loan repayment schedule from online banking, UniServe 360 pulls the customer’s loan data, applies the approved template, and generates the document instantly.

Here's how it works:

* A customer action or a system call triggers the request. UniServe 360 fetches the real-time data for the specific customer or transaction from the connected data source.
* Applies business rules and conditions, if any.
* Then, the system generates the document instantly using the active template and retrieved data.
* The final document is delivered in the required format (such as PDF) and made available to the user or the calling system.

{% hint style="info" %}
Make sure the template is checked in and set as the active version.
{% endhint %}

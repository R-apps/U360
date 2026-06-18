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
    visible: true
  pagination:
    visible: true
  metadata:
    visible: false
  tags:
    visible: true
  actions:
    visible: true
---

# Custom Parameter Configuration

Organizations often require business-specific information such as policy numbers, customer identifiers, application references, or source system details as custom parameters.

Custom Parameter Configuration allows administrators to define the maximum number of custom parameters that businesses can include in CPaaS API requests. Configuring a limit helps standardize API requests while still allowing businesses to personalize communications and maintain relevant tracking information.

The configured limit applies to SMS, email, and WhatsApp communications.

### Set Custom Parameter Limit

* Sign in as a Super Admin.
* Navigate to the CPaaS configuration settings.
* Specify the maximum number of custom parameters allowed per API request.
* Save the configuration.

<div align="left"><figure><img src="../.gitbook/assets/image (127).png" alt="" width="446"><figcaption></figcaption></figure></div>

The configured limit applies across all supported CPaaS communication channels.

### Configure Custom Parameters

Businesses can configure the required custom parameters as follows:

* Log in to the UniServe Reach application.
*   Go to **Settings** and select **CPaaS Custom Params**.

    <div align="left"><figure><img src="../.gitbook/assets/image (129).png" alt=""><figcaption></figcaption></figure></div>
*   Select **Add Custom Column** (![](<../.gitbook/assets/image (131).png>)) and specify the following:

    * **Column Name**: Enter the custom parameter name.
    * **Data Type**: Select the data type.
    * **Validation**: Specify whether this column needs validation. If it does, select the validation.
    * **Search**: Select this option to make this parameter available as a search criterion in the detailed report.
    * **Comments**: Add any additional information about this parameter, if required.

    Then select **Save**.

    <div align="left"><figure><img src="../.gitbook/assets/image (132).png" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
Businesses should add custom parameters carefully, as they cannot edit or delete them once they are added.
{% endhint %}

### API Payload with Custom Parameters

Here is a sample CPaaS API payload structure with custom parameters:

```json
{
  "to": "9876543210",
  "channel": "SMS",
  "message": "Dear <user_name>, renew your policy at a lower cost with 0% GST! Policy 12345 was due for renewal on 2026-05-30. Pay Rs.100 at link to keep your life cover active & bonus benefits intact. T&C Apply. XYZ Ltd.",
  "msg_category": "TR",
  "regional": {
    "template_id": "111222333444555666",
    "pe_id": "1010101010101010199",
    "header": "XYZ",
    "country": "91"
  },
  "short_link": "Y",
  "reach_template": "N",
  "custom_params": {
    "service_request": "XYZ12345",
    "policy_number": "123456789",
    "application_number": "XYZ12345",
    "client_id": "57645675",
    "name": "John",
    "department": "Renewal"
  }
}
```

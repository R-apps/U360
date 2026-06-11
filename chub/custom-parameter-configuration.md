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

Custom Parameters Configuration allows administrators to define the maximum number of custom parameters that businesses can include in CPaaS API requests. Configuring a limit helps standardize API requests while still allowing businesses to personalize communications and maintain relevant tracking information.

The configured limit applies to SMS, Email, and WhatsApp communications.

### Set Custom Parameter Limit

* Sign in as a Super Admin.
* Navigate to CPaaS configuration settings.
* Specify the maximum number of custom parameters allowed per API request.

Then, save the configuration.

<div align="left"><figure><img src="../.gitbook/assets/image (127).png" alt="" width="446"><figcaption></figcaption></figure></div>

The configured limit is applied across all supported CPaaS communication channels.&#x20;

### Configuring Custom Parameters

Businesses, to configure the necessary custom parameters,

* Log in to UniServe Reach application
*   Go to **Settings** and select **CPAAS Custom Params**

    <div align="left"><figure><img src="../.gitbook/assets/image (129).png" alt=""><figcaption></figcaption></figure></div>
*   Select **Add Custom Column** (![](<../.gitbook/assets/image (131).png>)) and specify the following:

    * **Column Name**: Enter the custom param name
    * **Data Type**: Select its data type
    * **Validation**: Specify if this column needs validation. If yes, select the validation.
    * **Search**: Check this option to make this parameter available as a search criterion in the detailed report.
    * **Comments**: Add any information about this param, if required.

    Then, select **Save**.&#x20;

    <div align="left"><figure><img src="../.gitbook/assets/image (132).png" alt=""><figcaption></figcaption></figure></div>

{% hint style="info" %}
Businesses should make sure they add custom params carefully as they cannot edit or delete once added.&#x20;
{% endhint %}

### API Payload with Custom Params

Here's the sample structure of CPaaS API payload with custom params:

<pre class="language-json"><code class="lang-json">{
"to": "9876543210",
"channel": "SMS",
"message":"Dear &#x3C;user_name>, renew your policy at a lower cost with 0% GST!
Policy 12345 was due for renewal on 2026-05-30.
Pay Rs.100 at link to keep your life cover active &#x26; bonus benefits intact.
T&#x26;C Apply.
XYZ Ltd.",
"msg_category": "TR",
"regional": {
"template_id": "111222333444555666",
"pe_id": "1010101010101010199",
"header": "XYZ",
"country": "91"
},
"short_link": "Y",
"reach_template": "N",
<strong>"custom_params":{
</strong><strong>  "service_request":"XYZ12345",
</strong>  "policy_number":"123456789",
<strong>  "application_number":"XYZ12345",
</strong>  "client_id":"57645675",
  "name":"John",
  "department":"Renewal"
}
}
</code></pre>


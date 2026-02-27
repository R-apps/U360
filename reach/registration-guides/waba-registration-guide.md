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
---

# WABA Registration Guide

Here are the steps to register your WhatsApp Business Account (WABA).

### Creating a WhatsApp Business Account

To create a WhatsApp Business account (WABA), be handy the following information:

* Facebook Business Manager ID
* Business Name
* Company logo (min 640x640 pixels, PNG/JPG via Publicly Hosted URL)
* Company description
* Company website, address, contact email
* A phone number to associate with the WhatsApp Account (Standard Long Number), this number identifies the account on the WhatsApp platform and is used as the sender Identity and as a reference for inbound conversations. Make sure the phone number meets the following criteria:
  * The phone number must be in the standard international format.
  * As part of the onboarding process for your new WhatsApp Business API, this number will be validated to ensure number ownership by SMS or Voice call – make sure it is not in DND or fight mode.
  * The phone number must not be associated with a WhatsApp Account. If it is, it will require disassociation first.

{% hint style="info" %}
Note: If your business is not yet Facebook verified, starting the registration process will walk you through the necessary steps.
{% endhint %}

### WABA Validation

Following steps are involved in WhatsApp business account validation:

{% stepper %}
{% step %}
### Business Manager ID verification

Performed using the Facebook Business ID provided by you.

* WhatsApp validates industry vertical with the commerce policy ([https://www.whatsapp.com/legal/commerce-policy/](https://www.whatsapp.com/legal/commerce-policy/%20))
* Meta approves the **Message on Behalf of Authority** notification, which arrives in your Facebook Business Manager console.
{% endstep %}

{% step %}
### Phone number validation

At the time of onboarding, Meta validates your phone number. As a part of this validation, WhatsApp sends 2FA request to your WhatsApp registered phone number. You will receive it via SMS or voice, and it will be valid only for 10minutes.
{% endstep %}
{% endstepper %}

You can locate your Facebook Business Manager ID in the **Business Settings > Business info** section in the Facebook Business Manager console: [https://business.facebook.com/settings/info](https://business.facebook.com/settings/info)

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/WABA Registration Guide.png" alt=""><figcaption></figcaption></figure></div>

For further information on Business Verification refer to:

[https://www.facebook.com/business/help/2058515294227817](https://www.facebook.com/business/help/2058515294227817)

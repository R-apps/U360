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

# DLT Registration Guide

This step-by-step guide assists you in DLT registration process for Entity, Header, and SMS Template registration. This document contains all of the necessary information to register your Entity, Header, and SMS Templates on the DLT platform. Please read it carefully.

According to the latest guidelines from TRAI (Telecom Regulatory Authority of India) and Operators, you must register your Entity, Header, and Templates on the Operators' DLT platform before sending enterprise messages, whether Transactional or Promotional. Once registered, you can seamlessly integrate these (Header/Templates) into your 24x7SMS account to send messages to your customers.

Please follow these steps carefully to ensure smooth registration and compliance with regulatory requirements.

{% stepper %}
{% step %}
#### Entity (Company/Enterprise/Others) Registration

The first step is Entity registration. Visit any of the operators' DLT links and follow these steps:

* Sign up as an Enterprise by providing details such as PAN, GST, Company Name, Address, etc.
* Upload the required documents and make the payment for registration fees, if applicable.
* Upon approval, you will receive a unique Entity ID.

**DLT Links**

JIO: \[[https://trueconnect.jio.com/#/entity-registration;role=PE](https://trueconnect.jio.com/%23/entity-registration;role=PE)]

Airtel: \[[https://www.airtel.in/business/commercial-communication/home](https://www.airtel.in/business/commercial-communication/home)]

Vodafone: \[[https://www.vilpower.in/\]](https://www.vilpower.in/]%20)

Videocon: \[[https://smartping.live/entity/register-with](https://smartping.live/entity/register-with)]

Tata Tele: \[[https://telemarketer.tatateleservices.com:8082/#/entity-registration;role=PE](https://telemarketer.tatateleservices.com:8082/%23/entity-registration;role=PE)]

BSNL: \[[https://www.ucc-bsnl.co.in/\]](https://www.ucc-bsnl.co.in/]%20)

{% hint style="info" %}
**Note**: Registration on any one portal will automatically sync across all other portals.
{% endhint %}

**Documents required for registration**

* PAN/GST/TAN
* Letter of Authorization
* Registration fees, if applicable.
{% endstep %}

{% step %}
#### Header (Sender ID) Registration

After registering your Entity on any operator portal, proceed to register your header by following the steps available on the respective operator's DLT portal.

Make sure to follow the below formats for transactional and promotional headers:

* Transactional Headers should consist of 6-alpha characters only and they are case sensitive.
* Promotional Headers should begin with a number corresponding to the category (as per DND Preferences).
{% endstep %}

{% step %}
#### Template (SMS Content) Registration

**Guidelines for SMS Template rules on all Operators' DLT Platforms**:

* The template content should only have one space between words.
* For any variable, use either the Insert Variable option or type {#var#}.
* Each variable can hold a maximum of 20 characters.
* Variable fields can contain special characters.
* Variables should be used to replace customized values such as name, amount, date, OTP, and URL.
* Variable fields are required for Transactional/Service SMS templates, with a maximum of four variables allowed.
* SMS templates in the Promotional category can contain static content or up to two variables.

**Steps to upload Transactional/Service Implicit templates for approval at all Operators DLT Platform:**

* Log into the operator’s DLT portal and navigate to TEMPLATE section.
* Select the Template Type (Transactional & Service Implicit).
* Provide the Header (Sender ID) to which you want to link the template.
* Provide a unique Template Name for easy reference.
* Select the Template message type (Text or Unicode).
* Provide the template content and save it for approval by the DLT Registrar.

**Steps to upload Promotional/Service Explicit templates for approval at all Operators DLT Platform:**

* Log in to the operator’s DLT portal and navigate to CONSENT TEMPLATE section.
* Upload the consent template. Then, save and send it to the DLT Registrar for approval.
* Once approved, navigate to the TEMPLATE section, select Template Type, Headers, and provide the Template Name and content.
* Provide the template content and save it for approval by the DLT Registrar.
{% endstep %}
{% endstepper %}

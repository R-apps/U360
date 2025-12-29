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
---

# Defining Data Sources and Process Levels

Let's understand the processing levels for different data source types.

<details>

<summary>Text Files</summary>

**Step 1**: Select the Process Data Source Type as "Text Files". &#x20;

**Step 2**:  Click <mark style="color:green;">\<icon></mark> to define the data source. In the **Text Extractor** wizard, expand the Text Extractor to locate the entity.&#x20;

Example: A bank has a large text file containing all credit card statements for the month.

```yml
===============================
Customer account details
===============================

--------------------------------
MAIN ACCOUNT SUMMARY
--------------------------------
Customer Name      : Mr. R. Kumar
Customer ID        : 78912345
Card Number        : XXXX XXXX XXXX 4567
Statement Month    : November 2025
Credit Limit       : ₹ 2,00,000
Available Limit    : ₹ 1,57,800
Total Due          : ₹ 42,200
Minimum Amount Due : ₹ 4,220
Due Date           : 10-Dec-2025

--------------------------------
TRANSACTION HISTORY
--------------------------------

# Transaction 1
Date        : 04-Nov-2025
Merchant    : Amazon India
Description : Online Purchase - Electronics
Amount      : ₹ 15,500
Status      : Posted

# Transaction 2
Date        : 10-Nov-2025
Merchant    : Apollo Pharmacy
Description : Medical Purchase
Amount      : ₹ 1,245
Status      : Posted
```

This file has information in two levels:

1. Main Account (Customer summary)
2. Sub Accounts / Transaction history

To extract this data correctly, the system needs to know where each part begins and end&#x73;**.**\
This is what **Entities** help with.&#x20;

Entity One is the default entity. It represents Parent Account Information. Click it and specify the identifier and other properties to tell the system how to identify and extract the data from a text file.&#x20;

**Defining the Entity Properties**:

Select the **Type** to specify the beginning of an entity (Identifier / Line Count)\
Use:\
&#x20;    **Identifier**, when you can locate the section by a specific word or phrase.\
&#x20;    **Line Count**, when the section always begins after a fixed number of lines, with no unique \
&#x20;    text to search for.

Here's a quick reference to understand what Type to select and when to enable Match Case/Match word:

<table><thead><tr><th width="214" valign="top">Type</th><th valign="top">When to Use</th><th valign="top">Example</th></tr></thead><tbody><tr><td valign="top">Identifier</td><td valign="top">When a section contains a unique text pattern that can be searched</td><td valign="top">Parent account details always begin with the label “CUSTOMER ACCOUNT DETAILS”.</td></tr><tr><td valign="top">Identifier + <br>Match Case/Match Word</td><td valign="top">When the system should only match exact text</td><td valign="top">Transaction rows contain <strong>“DEBIT”</strong> in uppercase. Using Match Case ensures the system doesn’t pick <strong>“Debit”</strong> or <strong>“debit”</strong>.</td></tr><tr><td valign="top">Line Count</td><td valign="top">When the file uses a fixed layout, and the next section always begins after a set number of lines.</td><td valign="top">A sub-account record always begins <strong>5 lines below</strong> the parent record. Set Line Count = 5 to capture the sub-account details.</td></tr></tbody></table>

**Adding additional entities**: Let's understand where and why do we require additional entities. \
For example, if the bank wants to extract additional information such as Reward points summary, EMI details, etc., add more entities by clicking '+' in the parent entity.&#x20;

```yaml
--------------------------------
REWARD POINTS SUMMARY
--------------------------------
Total Reward Points Earned This Month : 1,250
Total Reward Points Available         : 8,940
Equivalent Cashback Value             : ₹ 894

Recent Earned Points:
  • Amazon Purchase (₹ 15,500)  →  775 Points
  • Fuel (₹ 1,800)              →  180 Points
  • Others                      →  295 Points

Redemption Options Available:
  - Cashback
  - Flight Miles
  - Gift Vouchers
  - Utility Bill Payments

--------------------------------
EMI DETAILS
--------------------------------
EMI #1
  Description       : Mobile Phone Purchase (Flipkart)
  Purchase Amount   : ₹ 36,000
  EMI Amount        : ₹ 3,000 / month
  Tenure            : 12 Months
  Remaining Months  : 6
  Interest Rate     : 14%
```

Each added entity helps the system separate sections like this:\
&#x20;\
Entity One --> Account summary\
Entity Two --> Transactions\
Entity Three --> Rewards details\
Entity Four --> EMI details

<mark style="color:green;">**<\<IMAGE - Adding a new entity>>**</mark>

As you add entity, they are created in a hierarchical model acting as Parent & Sub accounts. &#x20;

Once created, define the properties for each entity and click **OK** to continue.

{% hint style="info" %}
* You cannot rename the entity once created.
* You can delete the unused entities.&#x20;
{% endhint %}

**Step 3**: Define process levels. To define, select the default (Level1) and select its value in the Properties.\
<mark style="color:green;">**<\<IMAGE - Level 1 Processing>>**</mark>\
If your data source has another level inside it, click '+' to add another level for processing and specify its properties.  \
<mark style="color:green;">**<\<IMAGE - Level 2 Processing>>**</mark>\
Follow the same process to define all the levels.

</details>

<details>

<summary>XML</summary>

Select the Process Data Source Type as "XML" and follow the same process as specified for [Text Files](defining-data-sources-and-process-levels.md#text-files) data source.&#x20;

Here's the sample XML structure:

```xml
<CustomerAccountDetails>

  <CustomerSummary>
    <CustomerName>Mr. R. Kumar</CustomerName>
    <CustomerID>78912345</CustomerID>
    <CardNumber>XXXX XXXX XXXX 4567</CardNumber>
    <StatementMonth>November 2025</StatementMonth>
    <CreditLimit>200000</CreditLimit>
    <AvailableLimit>157800</AvailableLimit>
    <TotalDue>42200</TotalDue>
    <MinimumAmountDue>4220</MinimumAmountDue>
    <DueDate>10-Dec-2025</DueDate>
  </CustomerSummary>

  <Transactions>
    <Transaction>
      <Date>04-Nov-2025</Date>
      <Merchant>Amazon India</Merchant>
      <Description>Online Purchase - Electronics</Description>
      <Amount>15500</Amount>
      <Status>Posted</Status>
    </Transaction>

    <Transaction>
      <Date>10-Nov-2025</Date>
      <Merchant>Apollo Pharmacy</Merchant>
      <Description>Medical Purchase</Description>
      <Amount>1245</Amount>
      <Status>Posted</Status>
    </Transaction>

    <Transaction>
      <Date>22-Nov-2025</Date>
      <Merchant>Big Bazaar</Merchant>
      <Description>Grocery & Household</Description>
      <Amount>5600</Amount>
      <Status>Posted</Status>
    </Transaction>
  </Transactions>

  <RewardPoints>
    <EarnedThisMonth>1250</EarnedThisMonth>
    <Available>8940</Available>
    <CashbackValue>894</CashbackValue>
  </RewardPoints>

  <EMIDetails>
    <EMI>
      <Description>Mobile Phone Purchase (Flipkart)</Description>
      <PurchaseAmount>36000</PurchaseAmount>
      <EMIAmount>3000</EMIAmount>
      <RemainingMonths>6</RemainingMonths>
      <InterestRate>14%</InterestRate>
    </EMI>
 </EMIDetails>
 
</CustomerAccountDetails>
```

</details>

<details>

<summary>JSON</summary>

**Step 1**: Select the Process Data Source Type as "JSON", when the input is structured JSON.

**Step 2**:  Click <mark style="color:green;">\<icon></mark> to define the data source. In the **JSON Extractor** wizard, expand the \
JSON Extractor to locate the entity.&#x20;

Example: A bank's JSON feed containing Customer Information, Monthly Account Summary, and Transactions.

```json
{
  "customer": {
    "name": "John",
    "accountNumber": "1234567890",
    "statementMonth": "November 2025"
  },
  "summary": {
    "openingBalance": 20000,
    "closingBalance": 25000
  },
  "transactions": [
    {
      "date": "2025-01-03",
      "description": "POS PURCHASE",
      "amount": 1500
    },
    {
      "date": "2025-01-11",
      "description": "ATM WITHDRAWAL",
      "amount": 2000
    }
  ]
}
```

**Defining the Entity Properties**:

Select the **Type** as "Identifier" to specify the beginning of an entity. \
For JSON files, '{' becomes the identifier or you can specify the line count.

**Step 3**: Define process levels.&#x20;

To define, select the default (Level1) and select its value in the Properties.\
<mark style="color:green;">**<\<IMAGE - Level 1 Processing>>**</mark>

</details>

<details>

<summary>Database</summary>



</details>

Enable "**Content Authoring**" only when you want to let your users change the content at text /image level without working with the template directly.  --> <mark style="color:orange;">Check with</mark> <mark style="color:orange;">Karu</mark>

If enabled, specify the design workflow and select the server for batch processing.&#x20;

To manage batch configurations, click <mark style="color:green;">**\<icon>**</mark>. [Click here](../../output-generation/batch-configurations.md) to know more about batch configurations.

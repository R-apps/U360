# Client (Output Format) Settings

**Client Settings** control how runtime metadata is captured and stored in the UniServe database during document processing. When the job is executed, this information is saved automatically in the database and helps track who received what, how, and when.&#x20;

This helps you track processing status, output details, and distribution behavior across channels.

A job schema is created for each registered client. These job schemas are updated in real time as the document moves through different processing stages.

#### Accessing client settings

* Expand **Client Settings**.
* Select a client from the list:
  * **Primary Client** – Process Client
  * **Dependent Clients** – Print, Mail, SMS, WhatsApp, Hybrid (SMS & Email) and others\
    ![](<../../../.gitbook/assets/Primary and Secondary Clients (1).png>)
* Expand the selected client to configure mappings at different levels (File level, Level 1, Level 2). For each level, three configuration settings are available:
  * **Reserved:** Lists system-defined fields and are automatically populated during processing. \
    No manual mapping is required. Values are stored in the corresponding job table or entity.
  * **File:** Use to control output behavior per channel by specifying when the FGT should be applied.\
    \- Preprocessing\
    \- Processing\
    \- Post-processing
  * **Custom:** Displays user-defined fields where you can map global data variables based on the data type and business need. These fields help capture delivery details and status. If a delivery fails or incorrect data is sent, these mappings make it easier to identify and troubleshoot the issue.

This allows precise control over how metadata is captured and stored for each client and processing level.&#x20;

Let's see how to configure each client:

<br>

# Setting up the environment

**Batch Configurations** help you define how and where UniServe 360 should connect when running batch jobs. Here's where you control server access, database connectivity, and processing behavior for large-volume document generation.&#x20;

Batch configurations include server (to run batch jobs reliably, securely, and at scale) and database configurations (to fetch data). Set this up once per environment (QA, UAT, production, or client-specific) and reuse it across batch processes.

To set up an environment, navigate to **Settings** > **Batch Configurations**

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Batch Configurations.png" alt="" width="563"><figcaption></figcaption></figure></div>

### Server Configuration

This configuration defines how UniServe 360 connects to a processing server.

To configure a new server, click '+' and enter these details:

* **Profile Name:** a unique name to identify the environment (E.g., QA Server)&#x20;
* **Active:** set this to "true" to keep this configuration active
* **Organization:** organization name under which the batch process is executed
* **Username and Password:** credentials to securely authenticate with this server
* **Host and Port:** server IP address and Port number where the UniServe services are running
* **PMS Token Wait Time:** the maximum time (in seconds) the system should wait to receive an authentication token from the PMS service
* **Cloud Organization ID:** the cloud organization identifier, required for cloud servers
* **Connection Pool Size:** specify how many batch requests can be processed simultaneously
* **Timeout:** specify the maximum time (in seconds) the system should wait for a server response before stopping the request
* **Idle Connection Timeout:** specify the duration (in seconds) to wait before disconnecting
* **File Path:** the directory location used to read batch input files or store generated output files

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Batch Configurations - Server (1).png" alt="" width="563"><figcaption></figcaption></figure></div>

### Database Configuration

This database configuration helps UniServe 360 fetch data efficiently during batch processing.

To configure,

* **URL:** the database connection URL, to establish communication with the data source
* **Driver Name:** the database driver class name required to connect to the selected database
* **User & Password:** the database user account credentials, to access data during batch execution
* **Database in Use:** the specific database instance from which batch data is read

<div align="left" data-with-frame="true"><figure><img src="../../../.gitbook/assets/Batch Configurations - Database.png" alt="" width="563"><figcaption></figcaption></figure></div>

Click **Test Connection** to check the setup works correctly.

Alternatively, you can choose to upload these configurations in JSON format.&#x20;

To upload, click <img src="../../../.gitbook/assets/Batch Configurations - Import Icon.png" alt="" data-size="original"> and upload the JSON file.

### Manage Environments

To edit an existing configuration, click ![](<../../../.gitbook/assets/Batch Configurations - Edit Icon.png>). Make necessary changes and update.

To delete an existing configuration, click ![](<../../../.gitbook/assets/Batch Configurations - Delete Icon.png>).&#x20;

To export the configuration settings, click ![](<../../../.gitbook/assets/Batch Configurations - Export Icon.png>). The configurations are exported in JSON format.

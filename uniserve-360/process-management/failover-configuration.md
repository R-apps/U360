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

# Failover Configuration

UniServe supports failover mechanism to ensure uninterrupted operations when the primary server becomes unavailable.

When failover is configured, processing initially begins on the **primary server**. If the primary server stops responding, the system automatically transfers processing to the **secondary server**, avoiding manual intervention.

For failover to work correctly:

* The same MPT must exist on both servers.
* The secondary server must be mapped to the corresponding template in the failover configuration.

To assign a secondary server,

*   Right-click the **IP address** of the active server and select **Configure**. \
    The **Process Configuration** dialog box appears.<br>

    <div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure></div>
* Expand **Failover Management** and select the MPT for which the secondary server to be assigned. In the right pane,
  * select the secondary server IP address and MP template
  * Right-click the template under **Failover Management** in the left pane and click **Save.**

<div align="left" data-with-frame="true"><figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure></div>

Then, click **Upload**. A confirmation message appears.

This completes the failover server configuration for the template to be processed uninterruptedly.

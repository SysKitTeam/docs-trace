---
title: Configure SysKit Trace
description: >-
  This article explains how to configure SysKit Trace.
author: Vinko Bedek
date: 1/20/2020
---

# Configure SysKit Trace

Once the installation is completed, by default, **SysKit Trace Configuration Wizard** starts automatically. Alternatively, you can start it manually at any time by searching for it from the windows start menu.

## Prerequisites

In the Configuration Wizard, you will need to provide the following information:

* **Local service account**
* **Office 365 Global admin account**

{% hint style="info" %}
For a detailed overview of the **SysKit Trace system and permission requirements**, [navigate to the Requirements section](../requirements/).
{% endhint %}


## Configuration Steps

### Office 365 Connection

Click the **Connect** button to connect SysKit Trace to your Office 365 tenant. **You need to provide the Office 365 global admin account.** This [account](../requirements/permission-requirements.md#global-administrator) will be used to configure the [tenant connection](./office-365-connection-details.md).  

Once the login process has finished you will need to provide some additional info for the connection to work. 
This is also the place where you can configure automatic snapshots and notifications.

### Service Settings

Provide local service account that will be used for running the automatic actions performed by SysKit Trace such as scheduled data collection.

Supported service account formats:

* `machine_name\username`
* `domain_name\username`

After you've entered the credentials click the **Validate Account** button. If the account has all [proper privileges](../requirements/permission-requirements.md#service-account), a Success window appears with the message:

`This account can be used to run SysKit Trace!`

Click **OK** to close the Success window, and **Next &gt;** to continue to the next step.


### Finish

The last step shows the status of all operations that are done before you can access SysKit Trace. If the configuration was successful, all steps are marked with green checkmarks.

Click the **Finish** button to open SysKit Trace.
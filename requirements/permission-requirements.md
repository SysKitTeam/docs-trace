---
title: Requirements
description: >-
  This article lists the requirements needed to run and use SysKit Trace
author: Vinko Bedek
date: 4/14/2020
---

## Installation
To install and use SysKit Trace, you need to have **Local Administrator** privileges on the target installation computer.

## Service Account

**Service Settings** page in Configuration Wizard requires appropriate [service account](https://docs.microsoft.com/en-us/windows/security/identity-protection/access-control/service-accounts) details.

A service account is a user account that is created explicitly to provide a security context for services running on Windows Server operating systems. The security context determined the service’s ability to access local and network resources. The Windows operating systems rely on services to run various features. These services can be configured through the applications, the Services snap-in, or Task Manager, or by using Windows PowerShell.

**The service account needs to have the following privileges** to be able to run the service, [collect Office 365 data](../how-to/collect-office-365-data.md) and run other associated jobs:

* **local administrator** privileges on the installation computer with UAC control disabled so we can verify your credentials
* **log on as Service** rights configured

## Office 365

### Global Administrator

**When connecting to an Office 365 tenant** during the [configuration](../installation-and-configuration/configure-syskit-point.md#office-365-connection) process, **you need to connect with a Global Administrator account.**

**The first time you connect to your Office 365 tenant, you will be prompted to give consent** to a set of permissions that SysKit Trace requires to function correctly. Additional prompts may show up in the future when installing a newer version of SysKit Point because of new functionality, and in consequence, potentially new required permissions.  

The consented permissions will be used to perform the [tenant connection](./office-365-connection-details.md) configuration.
It will also be used for collecting data for some workloads that do not support an application identity.
For this reason, the account needs to have a **product license** assigned. Exchange and Teams need to be included in the selected product license.    
Once the tenant connection has been established the global admin role can be removed from the account. 
If you choose to do so you will need to assign some roles to the user because as mentioned in the [tenant connection](./office-365-connection-details.md) article, some workloads cannot be read by the Azure Application and must be retrieved with the identity of a user.

A combination of:
- Exchange admin
- Teams admin
- PowerApps admin
- Compliance admin 

roles will load most of the data.
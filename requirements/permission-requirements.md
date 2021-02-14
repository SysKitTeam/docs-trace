---
title: Permission Requirements
description: >-
  This article discusses permission requirements that are necessary to
  successfully install and use SysKit Trace.
author: Vinko Bedek
date: 4/14/2020
---

# Permission Requirements

## Installation

To install and use SysKit Trace, you need to have **Local Administrator** privileges on the target installation computer.

## Service Account

**Service Settings** page in the Configuration Wizard requires appropriate [service account](https://docs.microsoft.com/en-us/windows/security/identity-protection/access-control/service-accounts) details.

A service account is a user account that is created explicitly to provide a security context for services running on Windows Server operating systems. The security context determined the service’s ability to access local and network resources. The Windows operating systems rely on services to run various features. These services can be configured through the applications, the Services snap-in, or Task Manager, or by using Windows PowerShell.

**The service account needs to have the following privileges** to be able to run the service, collect Office 365 data and run other associated jobs:

* **local administrator** privileges on the installation computer with UAC control disabled so we can verify your credentials
* **log on as Service** rights configured

## Office 365

### Global Administrator

**When connecting to an Office 365 tenant** during the [configuration](../installation-and-configuration/configure-syskit-trace.md#office-365-connection) process, **you need to connect with a Global Administrator account.**

**The first time you connect to your Office 365 tenant, you will be prompted to give consent** to a set of permissions that SysKit Trace requires to function correctly. Additional prompts may show up in the future when installing a newer version of SysKit Trace because of new functionality, and in consequence, potentially new required permissions.

The consented permissions will be used to perform the [tenant connection](../installation-and-configuration/office-365-connection-details.md) configuration. It will also be used for collecting data for some workloads that do not support an application identity. For this reason, the account needs to have a **product license** assigned. Exchange and Teams need to be included in the selected product license.

#### Avoiding Global Admin permissions

Once the tenant connection has been established and the Configuration Wizard finishes, the global admin role can be removed from the account. If you choose to do so you will need to assign some roles to the user because as mentioned in the [tenant connection](../installation-and-configuration/office-365-connection-details.md) article, some workloads cannot be read by the Azure Application and must be retrieved with the identity of a user.

A combination of:

* Exchange admin
* Teams admin
* PowerApps admin
* Compliance admin 

roles will load most of the data.

Note that this use case is not supported 100% yet and you may run into some issues because of cached access tokens. Also, each time that you run the Configuration Wizard you will need to add the global admin permissions back to the user so that the wizard can finish successfully. Our current recommendation is to continue using a global admin account but we do acknowledge that this may not be possible in your environment. Please don't hesitate to [contact us](https://www.syskit.com/company/contact-us) if you run into any issues setting this up.

### SysKit Trace App Permissions

{% hint style="warning" %}
**Please note!**  
Permissions described bellow are automatically granted to SysKit Trace by giving consent during the configuration process.
{% endhint %}

SysKit Trace will create an Azure AD Application when establishing a [connection](../installation-and-configuration/office-365-connection-details.md) to your tenant.  
SysKit Trace requires permissions to access several Microsoft APIs. There are two types of required permissions:

* **Application permissions** - define what SysKit Trace can do without a signed in user.
* **Delegated permissions** - define what SysKit Trace can do in the name of the signed in user.

The following permissions are required for the SysKit Trace Azure AD Application:

**Microsoft Graph**

| Permissions | Type | Reason |
| :--- | :--- | :--- |
| Read all administrative units | Application | Allows SysKit Trace to read administrative units and administrative unit membership. |
| Read directory data | Application | Allows SysKit Trace to read directory data. |
| Read all groups | Application | Allows SysKit Trace to read group properties. |
| Read all groups | Delegated | Allows SysKit Trace to read group properties as signed in user. Required for Planner. |
| Read all group memberships | Application | Allows SysKit Trace to read group memberships. |
| Send mail as any user | Application | Allows SysKit Point to send emails so you can be notified ie. when a snapshot finishes. |
| Have full control of all site collections | Application | Allows SysKit Trace to collect data from SharePoint. Unfortunately full control is required and it will not work with read permissions. |
| Sign users in | Delegated | Allows SysKit Trace to collect data from your environment as signed in user. |
| Read all users' full profiles | Delegated | Allows SysKit Trace to read your users profiles and show you reports based on that data. |

**Azure Active Directory Graph**

| Permissions | Type | Reason |
| :--- | :--- | :--- |
| Read directory data | Application | Allows SysKit Trace to read data in your company or school directory, such as users, groups, and apps. |
| Read all hidden memberships | Application | Allows SysKit Trace to read the memberships of hidden groups and administrative units. |

**SharePoint**

| Permissions | Type | Reason |
| :--- | :--- | :--- |
| Have full control of all site collections | Application | Allows SysKit Trace to collect data from SharePoint. Unfortunately full control is required and it will not work with read permissions. |
| Read user profiles | Application | Allows SysKit Trace to read user profile properties. |

**Teams and Skype for Business Administration**

| Permissions | Type | Reason |
| :--- | :--- | :--- |
| Have full access to the Skype Remote Powershell Azure services | Delegated | Allow SysKit Trace to collect Skype for Business data on behalf of the signed-in user. |

**PowerApps Service**

| Permissions | Type | Reason |
| :--- | :--- | :--- |
| Access the PowerApps Service API | Delegated | Allows SysKit Trace to access the PowerApps Service API on behalf  of the signed-in user. |

**Azure Service Management**

| Permissions | Type | Reason |
| :--- | :--- | :--- |
| Access Azure Service Management as organization users | Delegated | Allows SysKit Trace to collect data about PowerApps. |


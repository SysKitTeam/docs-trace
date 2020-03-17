---
title: Requirements
description: >-
  This article lists the requirements needed to run and use SysKit Trace
author: Vinko Bedek
date: 1/20/2020
---

# Requirements

In order to prepare for the SysKit Trace deployment, the following requirements need to be met:

## Hardware Requirements

* CPU – any Windows 7, Windows 8 or Windows 10 capable CPU 
* Memory 
  * up to 200 MB RAM while idle 
  * upward of 500 MB RAM when performing or reading a snapshot 
* Disk – 100 MB disk space 

## Software Requirements

* Windows 10 or Windows Server 2016 or above 
* PowerShell 5.1 or above 
* .NET Framework 4.7.2 or above

SysKit Trace will also install additional PowerShell modules once the first snapshot attempt has been made. The modules are as follows: 

* ReverseDSC 
* MSOnline 
* SharePointPnPPowerShellOnline 
* Microsoft.Online.SharePoint.PowerShell 
* MicrosoftTeams 
* AzureAD 
* MSCloudLoginAssistant 
* Microsoft.PowerApps.Administration.PowerShell 

You do not need to install any of the modules manually. These modules are listed here for informational purposes only. You may want to install SysKit Trace on another machine if you are dependant on a specific version of any of these modules.

## User Permission Requirements 

* **Local administrator** to install and run the application 
* A windows service account with **Local administrator** rights that will be used for the SysKit Trace windows service
* An Office 365 account with the **Global admin role** to perform the tenant snapshot.  
  The account needs to have a **product license** assigned. SharePoint, Exchange, Teams and OneDrive need to be included in the selected product license.  
  Otherwise, SysKit Trace will fail to create snapshots.
* Alternatively, a combination of Exchange admin, SharePoint admin, Teams admin, User admin, Compliance admin roles will load most of the data. Nonetheless, the Global Admin role is recommended.
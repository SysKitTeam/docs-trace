---
title: Requirements
description: >-
  This article list the requirements needed to run and use SysKit Trace
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

SysKit Trace will also install additional PowerShell modules once the first snapshot attempt has been made. The modules are as follows: 

* ReverseDSC 
* MSOnline 
* SharePointPnPPowerShellOnline 
* Microsoft.Online.SharePoint.PowerShell 
* MicrosoftTeams 
* AzureAD 
* MSCloudLoginAssistant 
* Microsoft.PowerApps.Administration.PowerShell 

## User Permission Requirements 

* **Local administrator** to install and run the application 
* An Office 365 account with the **Global admin role** to perform the tenant snapshot
* Alternatively, a combination of Exchange admin, SharePoint admin, Teams admin, User admin, Compliance admin roles will load most of the data. Nonetheless, the Global Admin role is recommended. 

{% hint style="info" %}
Please note that MFA is currently not supported . We are working on improving this experience and will keep you updated as we release next versions of the tool.
{% endhint %}


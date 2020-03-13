---
description: >-
  This article explains how to configure WinRm authentication on
  your machine to successfully run snapshots.
---

# Configure Windows Remote Management (WinRM)

In order to successfully collect data, **SysKit Trace** will create a **remote PowerShell session** to the Security & Compliance Center.

To make sure that collection can work properly, Windows Remote Management (WinRM) on your computer needs to allow **Basic authentication** (it's enabled by default). 

### Enabling Basic Authentication

**1.** To verify that Basic authentication is enabled, run this command in a **Command Prompt**:

`winrm get winrm/config/client/auth`

**2.** If you don't see the value `Basic = true`, you need to run this command to enable Basic authentication for WinRM:

`winrm set winrm/config/client/auth @{Basic="true"}`

If Basic authentication is disabled, you'll get this error when creating a snapshot and collecting data for specific reports (Security & Compliance, Exchange Online, Teams etc.): 

*The WinRM client cannot process the request. Basic authentication is currently disabled in the client configuration. Change the client configuration and try the request again.*



For more information about creating PowerShell remote sessions, please visit: [https://docs.microsoft.com/en-us/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps]
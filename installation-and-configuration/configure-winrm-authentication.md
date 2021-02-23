---
description: This article explains how to configure WinRm authentication on your machine to successfully run snapshots.
---

# Configure WinRM Authentication

In order to successfully collect data when creating a snapshot, **SysKit Trace** will use a **remote PowerShell session** to connect to Office 365. This is required to collect the data for Security & Compliance, Exchange Online and some Teams reports.

To make sure that collection can work properly, Windows Remote Management \(WinRM\) on your computer needs to allow **Basic authentication** \(it's enabled by default\).

**Multi-Factor Authentication**

Even when using MFA, the WinRM Basic authentication needs to be enabled, because the Basic authentication header is still required to transport the session's OAuth token, since the client-side WinRM implementation has no support for OAuth.

## Enabling Basic Authentication

{% hint style="warning" %}
To enable executing commands from following steps, make sure that _Windows Remote Management_ service is running.
{% endhint %}

**1.** To verify that Basic authentication is enabled, run this command in a **Command Prompt**:

`winrm get winrm/config/client/auth`

**2.** If you don't see the value `Basic = true`, you need to run this command to enable Basic authentication for WinRM:

`winrm set winrm/config/client/auth @{Basic="true"}`

If Basic authentication is disabled, you'll get this error when creating a snapshot and collecting data for specific reports \(Security & Compliance, Exchange Online, Teams\):

_The WinRM client cannot process the request. Basic authentication is currently disabled in the client configuration. Change the client configuration and try the request again._

For more information about creating PowerShell remote sessions, please visit: [connect-to-scc-powershell](https://docs.microsoft.com/en-us/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).


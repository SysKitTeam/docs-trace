---
title: Install SysKit Trace
description: >-
  This article explains how to install SysKit Trace.
author: Vinko Bedek
date: 1/20/2020
---

# Install SysKit Trace

**SysKit Trace** is a desktop application, meaning that you need to install it on a Windows machine or server in your environment. Azure virtual machines are supported as well.

{% hint style="warning" %}
Check the exact [hardware and software requirements here](../requirements/system-requirements.md).
{% endhint %}

### Installation Steps

1. Download the SysKit Trace setup file.
2. Unpack and run the setup file - **SysKitTraceSetup.exe**. The wizard will guide you through the installation steps.
3. Check the **I Accept the terms of the license agreement** option to accept the [EULA](https://www.syskit.com/eula/) and click **Next &gt;** to proceed.
4. By default, the installation folder is set to **C:\Program Files\SysKit\Trace**. You can modify it by clicking the **Change** button. Once selected, click **Next &gt;** to proceed. 
5. Let the installation wizard finish
6. The configuration wizard should start automatically after the installation

### Configuration Steps
1. Connect to the tenant that you wish to collect data for.
2. Enter the windows service account for the SysKit Trace windows service. The SysKit Trace windows service is used to perform background tasks such as scheduled data collection.
3. Let the configuration wizard finish setting up the [tenant connection](./office-365-connection-details.md). 
4. The application should start automatically after the configuration

To continue with the configuration of the application, proceed to the [next article](./configure-syskit-trace.md).



---
description: >-
  This article explains how to easily create documentation of Office 365
  configuration settings using SysKit Trace.
---

# Manual Snapshots

This section describes how to use Snapshot wizard to collect  Office 365 configuration settings.

1. Navigate to the Actions Screen and click the Take Snapshot button.
2. If you are running the Snapshot Wizard for the first time please **enter the global admin credentials** for Office 365 tenant that you wish to document. The entered credentials will be stored for future data collection \(multiple tenants supported\).
3. Select the snapshot mode you wish the application to execute. There are three choices:
   1. **Default** – predefined set of configuration setttings will be loaded.
   2. **Custom** – allows the user to specify exactly what configuration setting should be loaded. 

      It can be the fastest load option if the user wishes to have access only to specific data, and is aware what data he is interested in. This mode is recommended for more advanced users who are looking to generate specific reports.   
      **Please note!** What you choose to take a snapshot of, within the Custom mode, applies only to the current load.

   3. **Full** –  collects all available information where possible. This is the recommended load mode if you don’t mind waiting and want to be sure you have all the data once the load finishes.
4. Click Next and the loading will start. Wait for the  wizard to finish, and start exploring the reports using Office 365 Explorer.


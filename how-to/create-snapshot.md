---
title: Create Snapshot
description: >-
  This article explains how to easily create a snapshot of Office 365
  configuration settings using SysKit Trace.
author: Vinko Bedek
date: 1/17/2020
---

# Create Snapshot

A snapshot in the context of SysKit Trace is a collection of all the Office 365 configuration settings taken at a specific point in time. There are two ways to create a snapshot in SysKit Trace:

## Take Snapshot Wizard

This section describes how to use the Take Snapshot wizard to create a snapshot.

1. Navigate to the **Home Screen** and click the Take Snapshot button.
2. If you are running the Snapshot Wizard for the first time please **enter the global admin credentials** for Office 365 tenant that you wish to document. The entered credentials will be stored for future data collection \(multiple tenants supported\).
3. Select the snapshot mode you wish the application to execute. There are three choices:
   1. **Default** – predefined set of configuration setttings will be loaded. The default selection can be modified in the [snapshot options](../get-to-know-syskit-trace/options-wizard.md#snapshot-options).
   2. **Custom** – allows the user to specify exactly what configuration setting should be loaded.

      It can be the fastest load option if the user wishes to have access only to specific data, and is aware what data he is interested in. This mode is recommended for more advanced users who are looking to generate specific reports.

   3. **Full** –  collects all available information where possible. This is the recommended load mode if you don’t mind waiting and want to be sure you have all the data once the load finishes.
4. Click Next and the loading will start. Wait for the  wizard to finish, and start exploring the reports using Office 365 Explorer.

## SysKit Trace Service

This section describes how to use the SysKit Trace service to create a snapshot.

The service can take a snapshot in one of two ways:

1. When adding the Office 365 tenant connection a schedule can be setup to collect the data periodically from your tenant. The snapshots taken by the SysKit Trace service will be available from the [snapshots screen](../get-to-know-syskit-trace/snapshots-screen.md). 

   To change the schedule for the snapshot you will need to run the Configuration Wizard again and modify the tenant connection.

2. By using the **Take Snapshot With Service button** on the [snapshots screen](../get-to-know-syskit-trace/snapshots-screen.md). The button is located in the dropdown part of the **Take Snapshot** button.

The configuration settings that the SysKit Service will collect can be modified in the [snapshot options](../get-to-know-syskit-trace/options-wizard.md#snapshot-options).


---
title: Compare Wizard
description: >-
  This article describes the SysKit Trace Compare Wizard and available
  comparison types. Track changes in your settings, compare different O365
  tenants.
author: Vinko Bedek
date: 1/16/2020
---

# Compare Settings

SysKit Trace allows to compare snapshots by using the Compare Wizard.  
The Compare Wizard provides the possibility to track Office 365 tenant changes and compare specific settings either on the same tenant or between different tenants. With a couple of easy steps you can view the desired differences and export the result.  
Before you can use the Compare Wizard you are required to have at least two snapshots [created](create-snapshot.md). To use the Compare Wizard click the **Compare Wizard** button on the [Home Screen](../get-to-know-syskit-trace/home-screen.md).

## Compare Tenant With a Previous Snapshot

1. Select **Compare tenant with a previous snapshot**
2. Select two snapshots from same tenant for the source and target.

   You can import additional snapshots by using the **Import** button.

   Importing snapshots is a one-time action, so the next time you run the Compare Wizard you will have to repeat the process.

   If you would like to import these snapshots permanently, click the **Import** button on the [Snapshots screen](../get-to-know-syskit-trace/snapshots-screen.md).

3. Click Next to see the settings compare results.

## Compare Two Diffent Tenants

1. Select **Compare two different tenants**
2. Select two snapshots from different tenants for the source and target.

   You can import additional snapshots by using the **Import** button.

   Importing snapshots is a one-time action, so the next time you run the Compare Wizard you will have to repeat the process.

   If you would like to import these snapshots permanently, click the **Import** button on the [Snapshots screen](../get-to-know-syskit-trace/snapshots-screen.md).

3. Select what you wish to ignore in the compare process. Not everything makes sense to compare when dealing with settings from different tenants.
4. Different tenants have different domains associated with them. Map the domains to each other as best as you can to get better compare results.
5. Click Next to see the compare results.

The Results window shows the differences between the two tenants. Object changes are marked by a different colors. The upper part of the window shows all the objects in a hierarchical structure, while the bottom half displays the differences between currently selected objects in the upper half. The compare process uses the [Compare template](../get-to-know-syskit-trace/options-wizard.md#compare) when displaying changes between snapshots. If you would like to change which objects are compared, use the cog button on the left-hand side. Deselected objects will not be used in future comparisons.


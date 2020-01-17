---
title: Snapshots Screen
description: >-
  This article states how to use Snapshots Screen and track changes made to your
  SharePoint farm during its lifetime.
author: Vinko Bedek
date: 6/23/2020
---

# Snapshots Screen

The **Snapshots Screen** allows administrators to track changes made to Office 365 during its lifetime. The snapshots contain information about all the [settings SysKit Trace can retrieve](../how-to/create-snapshot.md).

This screen will display snapshots found in the snapshots folder on the disk and group them by Office 365 tenants. The snapshots folder can be changed in the [options](../get-to-know-syskit-trace/options-wizard.md) if you desire to do so.

The following commands are available on this screen:

* **Open** – open currently selected snapshot.
* **Delete**– this button will delete the currently selected snapshot from previously defined snapshot locations.
* **Import** – use this button to add a snapshot to this list from any other location. Once that the snapshot is imported, it remains here until the user removes it.
* **Export**– use this button to snapshot file which can be transferred to any other location. 
* **Show Changes** – shows differences between the currently selected snapshot and an older snapshot \(if one exists\).
* **Compare Wizard**– starts Compare Wizard for more complex comparisons.
* **Compare to Local** – compares a snapshot with the currently loaded local farm.
* **Compare Selected**  – if two snapshots are selected, this button compares SharePoint settings stored in these two.
* **Mark Configuration as Good** – use this button to mark which snapshot captured your Office 365 tenant with all the settings configured in a best possible way.


---
title:  BigMemory Max 4.0.0 Release Notes  
lang: en
layout: page
keywords:
space: archive
sidebar: lb2_sidebar
permalink: /display/archive/BigMemory+Max+4.0.0+Release+Notes.html
summary:
---

BigMemory Max 4.0 introduces new and improved In-memory Data Management platform with following core capabilities:

##### **Simple & Predictable Scaling**

The BigMemory platform has been enhanced to scale to even higher data limits while providing greater resilience to failures.  The new, highly simplified, Resource Management provides capabilities to easily manage your data in-memory at scale with minimal to no tuning.  The new release includes improved management platform that provides tools such as Terracotta Management Console ("TMC") to effectively monitor, manage, and administer deployments.  Various other enhancements include improved support for rejoin and non-stop.

##### **Continuous Uptime**

The enhanced platform provides continuous availability of data with zero downtime with improvements in the areas of restart-ability and recoverability, including the new purpose-built Fast Restartable Store ("FRS").  The new FRS provides ability to take live backup and snapshots of in-memory data.  Various other enhancements include features for achieving extreme resilience to failures by configuring multiple redundant copies thereby avoiding any single point of failure in the deployment.

##### **Enhanced Interfaces & Integrations**

BigMemory Max 4.0 introduces support for Toolkit 2.0 -- an updated set of tools, helper classes, data structures, and APIs to help build scaled, distributed applications. This release also includes support for an early access of BigMemory-Hadoop connector to enable use cases to derive better value from data by using BigMemory and Hadoop in complementary ways.

##### **Support for Java 7**

BigMemory Max is Java 7 compliant.  Please refer to the Platform Support page for additional details.

##### Simplified Configuration File

If you are upgrading from an earlier version of Terracotta configuration, note that tc-config.xml has extensive changes:

*   The <mirror-group> element can now wrap <server> configuration blocks, eliminating the need to repeat the setup of <server> information.
*   <dso-port> is renamed to <tsa-port>, and <l2-group-port> is renamed to <tsa-group-port>.
*   <client-reconnect-window>, <garbage-collection> (DGC), and <restartable> settings are now global for all servers.  
    
*   The <data> element specifies where to store data files used for the fast-restartable feature.
*   The <clients> section now has one setting, <logs>.
*   <security> is a new configuration block for setting up authorization/authentication and SSL.
*    <offheap>, which used to be part a <persistence> configuration block, is now an independent element directly under <server>.
*   <dso>, <system>, <statistics>, <persistence>, and <ha> (and, unless otherwise noted, any sub-elements) have been removed.

See the [TSA Configuration Reference](http://terracotta.org/documentation/4.0/terracotta-server-array/config-reference) for a complete listing and definitions of configuration elements.

#### BigMemory Max 4.0.0 Known Issues

**Resource Management**

*   DEV-8998 - Known issue during active-mirror sync operation
*   DEV-9179 - Known performance issue during start of active-passive sync
*   DEV-8626 - Live objects may exceed maxEntriesInCache by many folds when a low threshold value for maxEntriesInCache is configured
*   DEV-8959 - Clients may timeout and exit while waiting for server to recover.  Workaround: Set a high value for "tc.config.total.timeout" for large data sizes 
*   DEV-9180 - Setting maxEntriesInCache to -1 dynamically doesn't work

**TMC**

*   DEV-8952 - Local Cluster config not shown until both active and passive servers are started
*   DEV-8953 - Fails to start up if logs directory removed 
*   DEV-9031 - Stale information shown when restarting cluster; Workaround: Refresh browser 
*   DEV-9046 - Unsecured REST agents accept TMS connection with secure parameters
*   DEV-9075 - Intermittent issue: "There are no CacheManagers" message shown in TMC's Application Tab
*   DEV-9090 - TMC becomes unresponsive after running for a extended period of time
*   DEV-9198 - No error message when creating a clustered cache and unclustered cache with the same name on different nodes
*   DEV-9216 - Issue configuring ini-based security; Workaround: create a dummy keychain file.  e.g. on unix execute "touch ~/.tc/mgmt/keychain", prior to restarting the TMS after enabling security

**Miscellaneous**

*   DEV-9132 - debug-tool script throws a benign exception when server is in "RECOVERING" status

C  

  

  

  

  



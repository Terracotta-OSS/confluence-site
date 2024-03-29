---
title:  Terracotta 3.6.0 Beta Release Notes  
lang: en
layout: page
keywords:
space: archive
sidebar: lb2_sidebar
permalink: /display/archive/Terracotta+3.6.0+Beta+Release+Notes.html
summary:
---

* TOC
{:toc}

Release Notes for Terracotta 3.6.0 Beta
=======================================

Overview
--------

*   Enterprise Ehcache 2.5.0
*   Quartz Scheduler 2.1.1
*   Terracotta Enterprise Suite 3.6.0

Summary of Changes
------------------

#### Ehcache 2.5.0

The major new capability of Ehcache 2.5 is enhanced cache resource management, specifically the ability to set the maximum size in bytes of a Cache or CacheManager. This offers the following additional benefits to Ehcache users:

*   Ease of use. Tuning cache sizes is now as simple as setting the maximum number of bytes. No more setting maximum entry counts and juggling eviction parameters to approximate the maximum amount of system memory your cache can use.
*   Greater efficiency. Ehcache now efficiently manages caches based on their memory footprint and can dynamically balance their resource use based on runtime size information.

For detailed documentation on how to use the new configuration settings available in Ehcache 2.5 please refer to:  
[http://ehcache.org/documentation/beta/configuration](http://ehcache.org/documentation/beta/configuration)

Also the Ehcache API has been extended with new batch methods (getAll, putAll and removeAll) that are performance optimized for use with Terracotta clustered caches.

#### Quartz Scheduler 2.1.0

This is a bug fix release for Quartz Scheduler. The list of fixes can be found [here](https://jira.terracotta.org/jira/secure/ReleaseNote.jspa?projectId=10282&version=10981)

#### Terracotta 3.6.0

*   BigMemory enhancements - L1 BigMemory support in clustered configurations, for significant performance improvements in large data set read-mostly use cases
*   Eventual consistency is now the default mode
*   Tomcat 7 support for express WebSessions
*   Many dev-console enhancements
    *   Ehcache statistics display can now show all available stats
    *   Both the Ehcache statistics data displayed in tabular form and charts shown are now user customizable
    *   A new tab that shows cache sizing

### Beta3 Notes

General

*   The implementation is not performance tuned. There are some known issues with performance although there are improvements over Beta.
*   6282 - Pinning in clustered cache to be implemented after Beta3

##### Resolved in Beta3

*   The Developer Console Sizing Panel allows edits which may throw exceptions
*   The sizing panel is Feature Complete
*   New naming for properties in ehcache.xml is incomplete.
*   Rejoin and Reconnect improvements
*   [EHC-857](https://jira.terracotta.org/jira/browse/EHC-857) - Write-behind IllegalMonitorStateException when last client terminates
*   6075 - cache.calculateInMemorySize() isn't correct for a clustered cache
*   6109 - Need to protect users from rogue sizeOf calls

##### Known Issues and Limitations

[https://jira.terracotta.org/jira/browse/DEV-6410](https://jira.terracotta.org/jira/browse/DEV-6410) - SVT update - need to figure out what to do in short term need to remove from documentation

*   6132 - Storage Engine and Eviction Failed on a small clustered cache filled above capacity
*   5939 - Date range queries are slower than other queries
*   [EHC-739](https://jira.terracotta.org/jira/browse/EHC-739) - OSGI headers in the MANIFEST

Please email any questions you have regarding the beta to pm <at> terracotta.org



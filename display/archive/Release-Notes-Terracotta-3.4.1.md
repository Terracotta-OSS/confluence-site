---
title:  Release Notes Terracotta 3.4.1  
lang: en
layout: page
keywords:
space: archive
sidebar: lb2_sidebar
permalink: /display/archive/Release+Notes+Terracotta+3.4.1.html
summary:
---

Release Notes for Terracotta 3.4.1
==================================

Terracotta 3.4.1 is a bug fix release. The kit includes [Ehcache 2.3.2](Release+Notes+Ehcache+2.3.2) and Quartz 1.8.4

*   5207 - Fix deadlock in server map eviction
*   5123 - Fix to Developer Console cacheable region reporting error in Hibernate panel
*   5053 - Updated MBean tunneling to stop unnecessary JMX communication from Client to Server
*   5113 - Fix to issue with Active/Passive Server setup. GC thread could get stuck on Passive Server causing OffHeap to fill up, disk to fill up and crash Passive
*   5105 - Fix to recover correctly from split-brain in Passive during restart, causing incomplete transactions
*   5077 - Fix to OOME during DGC immediately after Eviction

* * *

Release Notes for Terracotta 3.4.0
==================================

### New Feature

##### BigMemory for the Terracotta Server Array (L2)

BigMemory is an add-on product for Enterprise Ehcache and the Terracotta Server Array. It provides an off-heap cache that is not subject to Garbage Collection (GC). By avoiding performance-killing GC pauses, BigMemory allows Java applications to use as much memory as required. It works everywhere Ehcache works — for stand-alone and distributed caches — with no changes to application code and no special JVM or operating system requirements. It is available in two forms:

### Additional Improvements

*   Developer console improvements
*   Platform Updates
    *   Certification on JDK 1.6.0\_22

### Expected Updates and Scheduled Bug Fixes

in the Terracotta 3.4.0 Server Array and Kit [CDV Jira Project](https://jira.terracotta.org/jira/browse/CDV#selectedTab=com.atlassian.jira.plugin.system.project%3Achangelog-panel)

If You Are Upgrading: Terracotta Integration Modules in the Terracotta Toolkit

Users upgrading from a version earlier than 3.3.0 should note that the following Terracotta Integration Modules (TIMs) are now part of the Terracotta Toolkit JAR:

*   tim-concurrent-collections
*   tim-distributed-cache
*   tim-annotations
*   tim-async-processing

Product installation does not require specifying these TIMs. See the [product documentation](http://terracotta.org/documentation) for more information on installing Terracotta products with the Terracotta Toolkit JAR.

##### Known Issues

*   DEV-4875: Clustered Offheap statistics show allocated offheap space rather than offheap occupied in Terracotta Developer Console Graphs. This is as designed but should be noted as it may cause confusion.



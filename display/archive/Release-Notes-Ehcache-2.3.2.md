---
title:  Release Notes Ehcache 2.3.2  
lang: en
layout: page
keywords:
space: archive
sidebar: lb2_sidebar
permalink: /display/archive/Release+Notes+Ehcache+2.3.2.html
summary:
---

Release Notes for Ehcache 2.3.2
===============================

Ehcache 2.3.2 is included in the Terracotta 3.4.1 kit

Ehcache 2.3.2 is a bug fix and enhancement release. The following issue is addressed in this release.

*   [EHC-805](https://jira.terracotta.org/jira/browse/EHC-805) - Blocking cache can create several StripedReadWriteLockSync

* * *

Release Notes for Ehcache 2.3.1
===============================

Ehcache 2.3.1 is included in the Terracotta 3.4.0\_1 kit

Ehcache 2.3.1 is a bug fix and enhancement release. The following issues are addressed in this release.

*   [EHC-808](https://jira.terracotta.org/jira/browse/EHC-808) - Memory leak and thread-safety issue in CacheManager & Configuration
*   [EHC-810](https://jira.terracotta.org/jira/browse/EHC-810) - Changes in ManagementService method signature in 2.3.0 broke backward compatibility
*   CopyOnRead is now honored when used with the OffHeap setting
*   RMI bootstrapping Replication now working with BigMemory
*   Puts in onHeap fronted offHeap caches will now end up in the onHeap, unless onHeap is full
*   BigMemory no longer faults elements out on update



---
title:  Terracotta 11.1 Release Notes  
lang: en
layout: page
keywords:
space: current
sidebar: lb2_sidebar
permalink: /display/release/Terracotta+11.1+Release+Notes.html
summary:
---

Terracotta provides distributed in-memory operational data storage and caching for highly concurrent use cases requiring low and predictable latency.

The Terracotta 11.1.x Enterprise Edition offering includes the following:

   *  Distributed Caching capabilities via Java's most widely used cache, Ehcache 3.11.1.x API 
   *  Distributed In-Memory Operational Data Storage capabilities via the TCStore API
   *  Distributed In-Memory Data Management with fault-tolerance, and both horizontal and vertial scaling via Terracotta Server
   *  In memory off-heap storage - take advantage of all the RAM in your server and your client applications without GC pauses
   *  Terracotta Management Console for monitoring and managing your Terracotta cluster, and the workload that you've thrown at it

------

<br>

Document Contents

* TOC
{:toc}

<br>

# Current Release
------------------
Terracotta 11.1 (September 2024) is the latest release. It includes Ehcache 3.11.1.

Fixes are cumulative from version to version.

<br>

# Feature Highlights
------------------
The Terracotta 11.1 release builds upon the enterprise readiness features and analytical capabilities of past releases, by improving operational usability and performance. Some of the notable features of Terracotta 11.1 include:

* Rebranding and copyright for IBM
* Support for Java 17
* Various bug fixes and security fixes

<br>

# Summary of Changes 11.1
-----------------------
### 11.1.0.1
* Release Date: 2024/09/13
* Resolved
  * [TDB-18984]	Potential Cross Site Scripting Vulnerability in 'management/tmc/src/login.html'
  * [TDB-18985]	Potential DoS Regexp Vulnerability in 'management/tmc/src/js/util/OffHeapDialog.js'
  * [TDB-18986]	Potential Path Relative Stylesheet Vulnerabilities
  * [TDB-18987]	Potential 'Target Blank' vulnerabilities in TMC
  * [TDB-18989]	Potential autocompletion on sensitive fields in 'management/tmc/src/login.html'
  * [TDB-18991]	Remove unused class org.terracotta.config.data_roots.XmlUtils
  * [TDB-18992]	Configure TransformerFactory to mitigate XXE
  * [TDB-19031]	Make cloneable implementations final
  * [TDB-19032]	Possible "Evil" Regex
  * [TDB-19048]	Terracotta And BigMemory Max - Cross Site Scripting (Stored)
* Security Updates to Third Party Libraries
  * none

<br>

# Notes
-------
* Terracotta BigMemory 4.4.1.x and Terracotta 11.1.x clients may be used simultaneously in the same application by ensuring ClassLoader isolation when initializing at least one of the clients.
<br>
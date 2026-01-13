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

### 11.1.0.2
* Release Date: 2024/11
* Resolved
  * none
* Security Updates to Third Party Libraries
  * [TDB-19100] Vulnerable 3rd party component Spring framework used

### 11.1.0.3
* Release Date: 2024/12
* Resolved
  * none
* Security Updates to Third Party Libraries
  * [TDB-19136] Vulnerable 3rd party component Spring-security-web used - upgraded to 6.3.5
  * [TDB-19153] Vulnerable 3rd party component Spring framework used - upgraded to 6.1.15
  * [TDB-19146] Vulnerable 3rdparty components found in TDB Container images[11.1.0.1.3] - upgraded undertow-core to 2.3.18.Final

### 11.1.0.4
* Release Date: 2025/06/20
* Resolved
  * none
* Security Updates to Third Party Libraries
  * k8s.io/apimachinery to v0.26.10
  * micrometer-registry-prometheus to 1.13.13
  * logback-classic to 1.5.18
  * logback-core to 1.5.18
  * hibernate-validator to 8.0.2.Final
  * slf4j-api to 2.0.17
  * Spring Boot to 3.3.11
  * Spring Security 6.3.9
  * Spring to 6.1.19

### 11.1.0.5
* Release Date: 2025/08/22
* Resolved
  * [TDB-19324] TDBLibrariesStore SUM bundle includes the jdbc related jars
  * [TDB-19324] TDBServer SUM bundle includes the client folder
* Security Updates to Third Party Libraries
  * commons-lang3 to 3.18.0
  * Spring boot to 3.3.12
  * Spring to 6.1.20

### 11.1.0.6
* Release Date: 2025/09/22
* Resolved
  * Update Ehcache to 3.11.1
* Security Updates to Third Party Libraries
  * none

### 11.1.0.7
* Release Date: 2024/10/17
* Resolved
  * Base image update
* Security Updates to Third Party Libraries
  * 3rd Party Library Updates:
    *   Parquet Avro 1.15.2 : Fixes CVE-2025-30065 & CVE-2025-46762
    *   jackson-annotations to 2.18.1
    *   jackson-core to 2.18.1
    *   jackson-databind to 2.18.1

### 11.1.0.8
* Release Date: 2024/11/03
* Resolved
  * Base image update
* Security Updates to Third Party Libraries
  * none

### 11.1.0.9
* Release Date: 2024/12/02
* Resolved
  * Base image update
* Security Updates to Third Party Libraries
  * 3rd Party Library Updates:
    *   CVE-2023-1370 - JSON Smart to 2.4.11 
    *   CVE-2025-9784 - Undertow to 2.3.20.Final
    *   CVE-2023-2976, CVE-2020-8908 - Guava to 32.0.0-jre
    *   CVE-2024-7254 - Protobuf to 3.25.8
    *   CVE-2024-47554 - Commons IO to 2.21.0

### 11.1.0.10
* Release Date: 2024/01/12
* Resolved
  * none
* Security Updates to Third Party Libraries
  * Update docker base image
  * logback-classic 1.5.18 to 1.5.21
  * logback-core 1.5.18 to 1.5.21
  * classmate 1.7.0 to 1.7.1
  * prometheus 1.2.1 to 1.3.10
  * snakeyaml 2.2 to 2.4
  * Spring Boot 3.3.13 to 3.5.8
  * Spring Security 6.3.10 to 6.5.7
  * Spring Framework 6.1.21 to 6.2.14


<!-- Next entrypoint --> 

<br>

# Notes
-------
* Terracotta BigMemory 4.4.1.x and Terracotta 11.1.x clients may be used simultaneously in the same application by ensuring ClassLoader isolation when initializing at least one of the clients.
<br>

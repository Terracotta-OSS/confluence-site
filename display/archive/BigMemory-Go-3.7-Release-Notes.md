---
title:  BigMemory Go 3.7 Release Notes  
lang: en
layout: page
keywords:
space: archive
sidebar: lb2_sidebar
permalink: /display/archive/BigMemory+Go+3.7+Release+Notes.html
summary:
---


* TOC
{:toc}

# Release Notes for BigMemory Go 3.7.6
====================================

BigMemory Go 3.7.6 is a bug fix release.

##### Resolved Issues

*   9463 – Support for HP-UX

# Release Notes for BigMemory Go 3.7.2
====================================

BigMemory Go 3.7.2 is a bug fix release.

##### Resolved Issues

*   8317 - Terracotta Management Console, Hit Ratio, Hit Rate value toggles between 0 and 1 and not seeing graph for Hit Ratio
*   7883 - Null Pointer Exception when searching with an undefined attribute
*   7702 - Ability for Terracotta Management Console users to enable/disable agent connections
    
*   EHC-973 -Failure while decoding key java.nio.HeapByteBuffer 
    

# Release Notes for BigMemory Go 3.7.1
====================================

BigMemory Go is a pluggable, in-memory data management solution with sizable storage capacity and includes search, fast restartability, and support for management, administration, and monitoring.

# Summary of Features
-------------------

*   **In-memory data storage** - BigMemory Go comes with 32GB of free storage capacity per JVM.
*   **Fast Search** - BigMemory Go provides powerful search APIs for searching in-memory data in a predictable manner with extremely low latencies.
*   **Fault-tolerant fast restartable store** - BigMemory Go supports full fault tolerance using fast restartable store. This allows for continuous accessibility of previously cached data after a planned or unplanned shutdown.
*   **Terracotta Management Console** - BigMemory Go includes new web-based management console for complete management, administration, and monitoring of BigMemory Go deployments.
*   **Ehcache interfaces (APIs)** - BigMemory Go includes Ehcache interfaces for in-memory data management.

# Platform Support
----------------

Please see the [Platform Support Page](Terracotta+3.7%2C+Ehcache+2.6%2C+Quartz+2.1+Platform+Support).

# How to get support
------------------

#### Known Issues and Limitations

*   To run the samples with Maven, you will need to add the Terracotta Maven repositories to your Maven settings.xml file. Add the following repository information to your settings.xml file:
    
    <repository>
        <id>terracotta-repository</id>
        <url>http://www.terracotta.org/download/reflector/releases</url>
        <releases>
            <enabled>true</enabled>
        </releases>
    </repository>
    
    For further information please see [http://terracotta.org/documentation/more/apache-maven](http://terracotta.org/documentation/more/apache-maven)
    

*   BigMemory Go code samples do not run on 32-bit Windows
*   BigMemory Go 3.7.1 should not be run with older versions of Ehcache (less than 2.6.1)
*   8255 - Terracotta Management Console does not parse connection names containing underscores
*   8214 - Terracotta Management Console does not currently show disk size statistics for Fast Restartable Store
*   8164 - Terracotta Management Console Overview panel shows config values as all lowercase
*   7883 - Null Pointer Exception when searching with an undefined attribute

For any feedback or questions you have regarding this release to pm <at> terracotta.org.



---
title:  BigMemory 4.0, Ehcache 2.7 Platform Support  
lang: en
layout: page
keywords:
space: archive
sidebar: lb2_sidebar
permalink: /display/archive/BigMemory+4.0%2C+Ehcache+2.7+Platform+Support.html
summary:
---


* TOC
{:toc}

Platform Support
----------------

The platforms listed on this page are currently certified for use with commercial Terracotta product editions. As a 100% Java solution, Terracotta should run without issues on Java platforms for which it is not certified as well. If you have any questions about a certified or non-certified platform, contact us in one of the following ways:  
  

*   Send email to [info@terracotta.org](mailto:info@terracotta.org)
*   Post a question on our community forums

Terracotta is comprised of two different components: the client that integrates with your application, and the server (the server array) that typically runs on a set of separate machines in production.  The client is designed to run on many platform/JDK/container combinations. The server runs directly as a Java process (without a container).  
  

Client JDKs
-----------

| JDK Version |
| --- |
| Oracle/Sun Hotspot 1.7.0\_7 |
| Oracle/Sun Hotspot 1.6.0\_30 |
| Oracle BEA JRockit 1.6.0\_26-b03 R28 |
| IBM JDK 1.6 |

Client Containers
-----------------

| Container Versions |
| --- |
| Apache Tomcat 7.0.34 |
| Apache Tomcat 6.0.36 |
| IBM WebSphere 7.0.0.9 |
| IBM WebSphere 8.0 |
| IBM WebSphere 8.5 |
| JBoss AS 6.1.0 |
| JBoss AS 7.1.1 |
| Jetty 8.1.10 |
| Jetty 9.0.2 |
| Oracle BEA Weblogic 10.3.6 |
| Oracle BEA WebLogic 12.1.1 |
| Glassfish V3.1.2.2 |
| Resin 4.0.35 |

Server Information
------------------

The Terracotta server is a process that runs directly in a JVM.  
It has been validated on the following OSes with Sun Hotspot JDK 1.6.0\_27 and JDK 1.7.0\_07  
  

*   Solaris 10(x86)
*   Solaris 11(x86)
*   RedHat ES5 (5.6)
*   RedHat EL6 (6.4)
*   SUSE ES 10.4 32 and 64 bit
    
*   SUSE ES 11
*   Windows Server 2003 R2
*   Windows XP (dev only)
*   Windows Server 2008R2
*   Windows Server 2012
*   CentOS 5.6

For other JVM/platform combinations not listed above, please contact [info@terracotta.org](mailto:info@terracotta.org) to confirm status.

Library to Server Compatibility Matrix
--------------------------------------

[Library to Server Compatibility Matrix 4.0](Library+to+Server+Compatibility+Matrix)

### If you are using Sun SPARC

You may be encountering a known issue with the Sun Hotspot JVM for SPARC. The problem is expected to occur with Hotspot 1.6.0\_08 and higher, but may have been fixed in a later version. For more information, see this [Sun bug report](http://bugs.sun.com/bugdatabase/view_bug.do?bug_id=6849574) and [this possible fix](http://hg.openjdk.java.net/jdk7/hotspot-comp/hotspot/rev/c6386080541b).

  
  



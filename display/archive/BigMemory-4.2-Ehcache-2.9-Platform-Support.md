---
title:  BigMemory 4.2, Ehcache 2.9 Platform Support  
lang: en
layout: page
keywords:
space: archive
sidebar: lb2_sidebar
permalink: /display/archive/BigMemory+4.2%2C+Ehcache+2.9+Platform+Support.html
summary:
---


* TOC
{:toc}

Platform Support
----------------

The platforms listed on this page are currently certified for use with commercial Terracotta product editions. As a 100% Java solution, Terracotta should run without issues on Java platforms for which it is not certified as well. If you have any questions about a certified or non-certified platform, contact us in one of the following ways:  
  

*   Send email to [info@terracotta.org](mailto:info@terracotta.org)
*   Post a question on our community forums

Terracotta is comprised of two different components: the client that integrates with your application, and the server (the server array) that typically runs on a set of separate machines in production.  The client is designed to run on many platform/JDK/container combinations. The server runs directly as a Java process (without a container).

If you are using our BigMemory Cross Language Clients, please see [BigMemory .NET Client](http://terracotta-org/documentation/4.1/cross-language/dotnet/dotnet-install) and [BigMemory C++ Client](Library+to+Server+Compatibility+Matrix) for platform requirements.  
  

Client JDKs
-----------

| JDK Version |
| --- |
| Oracle/Sun Hotspot 1.7.0\_51 |
| Oracle/Sun Hotspot 1.6.0\_45 |
| OpenJDK 1.7 (RHEL only) |
| Oracle BEA JRockit 1.6 (client only) |
| IBM JDK 1.6 (client only) |

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
| JBoss EAP 6.1 |
| Jetty 8.1.10 |
| Jetty 9.0.2 |
| Oracle BEA Weblogic 10.3.6 |
| Oracle BEA WebLogic 12.1.1 |
| Glassfish V3.1.2.2 |

Server Information
------------------

The Terracotta server is a process that runs directly in a JVM.  
It has been validated on the following OSes with Sun Hotspot JDK 1.6.0\_45 and JDK 1.7.0\_51, and OpenJDK 1.7 (RHEL only).  
  

*   Solaris 11(x86)
*   RedHat EL6 (6.4)
*   RedHat EL6 (6.5)
*   SUSE ES 11 (SP 3)
    
*   Windows Server 2008R2
*   Windows Server 2012
*   CentOS 6.4

For other JVM/platform combinations not listed above, please contact [info@terracotta.org](mailto:info@terracotta.org) to confirm status.

Browsers (TMC)
--------------

*   Firefox 20.0
*   Chrome 33.0.1750.152
*   IE 9.0.50  
      
    

Library to Server Compatibility Matrix
--------------------------------------

[Library to Server Compatibility Matrix](Library+to+Server+Compatibility+Matrix)



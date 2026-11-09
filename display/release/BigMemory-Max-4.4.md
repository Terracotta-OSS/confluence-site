---
title:  BigMemory Max 4.4 Release Notes and Notifications
lang: en
layout: page
keywords:
space: current
sidebar: lb2_sidebar
permalink: /display/release/BigMemory+Max+4.4.html
summary:
---

BigMemory Max delivers ultrafast access to hundreds of terabytes of in-memory data. BigMemory snaps into enterprise applications to deliver unmatched performance at any scale.

BigMemory Max supports a distributed in-memory data-storage topology, which enables the sharing of data among multiple caches and in-memory data stores in multiple JVMs. It uses a Terracotta Server Array to manage data that is shared by multiple application nodes in a cluster.

The Ehcache 2.x API can be used with BigMemory Max 4.x as a general-purpose cache/in-memory data store or a second-level cache for Hibernate. You can additionally integrate it with third-party products such as ColdFusion, Google App Engine, and Spring.

------

<br>

Document Contents

* TOC
{:toc}

<br>

## Release Details
------------------
BigMemory Max 4.4.0 (October 2022). It includes Ehcache 2.11.

Fixes are cumulative from version to version.

> Deprecation Notice:  As previously announced in February 2020, as of October 2021, the BigMemory WAN Replication module and Web Sessions products have been deprecated and are no longer distributed or updated as part of BigMemory products (any/all versions).

<br>

## Feature Highlights
-------------------
BigMemory Max 4.4.0 introduced the following new capabilities:

*  Support for Java 11
*  Support for RedHat EL9 (server)
*  Support for Windows Server 2022
*  Provide logs in JSON format for better searchability and performance
*  Docker images with Logging as a service (LaaS) support
*  Voter process now available with Docker image
*  Various bug fixes and security fixes
* Contains all features and functionality included in [BigMemory Max 4.3.x](https://confluence.terracotta.org/display/release/BigMemory+Max+4.3)

<br>

# Summary of Changes 4.4
-----------------------
### 4.4.0.1
* Release Date: 2022/11/04
* Resolved
  * none  
* Security Updates to Third Party Libraries
  * [TAB-8200] Reflected Cross-Site Scripting
  * [TAB-8202] Improper Error Handling
  * [TAB-8203] Banner Grabbing
  * [TAB-8204] Server-side request forgery
  * [TAB-8241] Vulnerable 3rd Party Component Shiro used
  * [TAB-8226] Vulnerable 3rd Party Component Jackson Databind used

### 4.4.0.2
* Release Date: 2022/12/30
* Resolved
  * [TAB-8263]TMC shows blank page after installing Terracotta upgrade
  * [TAB-8261] Ascending function not working in terracotta query while fetching data.  
* Security Updates to Third Party Libraries
  * none
  
### 4.4.0.3
* Release Date: 2023/02/10
* Resolved
  * none  
* Security Updates to Third Party Libraries
  * [TAB-8280] Vulnerable 3rd Party Component shiro-core and jackson-databind updated
  
### 4.4.0.4
* Release Date: 2023/07/12
* Resolved
  * Update file containing docker image 3rd party components
* Security Updates to Third Party Libraries
  * [TAB-8393] CVE updates of json-smart
  * [TAB-8384] Vulnerable 3rd party component Guava updated
  * [TAB-8363] Vulnerable 3rd party component Eclipse-Jetty updated
  * Multiple 3rd party library updates
    *   jetty 10.0.15
    *   jackson-databind 2.15.2
    *   jersey 2.39.1
    *   guava 32.0.1-jre
    *   csrfguard 4.3.0
    *   logback 1.2.12
    *   hamcrest 2.2
    *   commons-io 2.13.0
    *   jaxb-runtime 2.3.8
  
### 4.4.0.5
* Release Date: 2023/08/11
* Resolved
  * none  
* Security Updates to Third Party Libraries
  * [TAB-8435][TAB-8436] Vulnerable 3rd party component Shiro updated
  * Other 3rd party library updates
    *   guava
    *   commons-codec
    *   commons-lang3
    *   jersey
  
### 4.4.0.6
* Release Date: 2023/10/04
* Resolved
  * [TAB-8276] Fix ConcurrentModificationException at org.terracotta.offheapstore.disk.storage.FileBackedStorageEngine.getOccupiedMemory
* Security Updates to Third Party Libraries
  * [TAB-8485] Vulnerable 3rd party component Eclipse Jetty updated to 10.0.16
  
### 4.4.0.7
* Release Date: 2023/10/24
* Resolved
  * none  
* Security Updates to Third Party Libraries
  * Third-party library upgrades:
    *   jetty to 10.0.17
    *   jackson to 2.15.3
    *   guava to 32.1.3-jre
    *   commons-io to 2.14.0
    *   rest-assured to 5.3.2

### 4.4.0.8
* Release Date: 2023/12/22
  * [TAB-8521] Secure Setting on cookies from TMS
  * [TAB-8522] Disable additional set of ciphers in TMS that are now considered weak
  * [TAB-8523] Enforce more strict password policy for strong passwords
  * [TAB-8288] Disallow HTTP v 1.0 protocol to TMS

### 4.4.0.9
* Release Date: 2024/02/03
* Resolved
  * [TAB-8544] The behavior of server-stat has changed after installing 4.4.0 Fix7
* Security Updates to Third Party Libraries
  * [TAB-8524] Http Security headers missing
  * [TAB-8529] High severity vulnerablity in logback found in terracotta-toolkit-runtime-ee-4.4.0.7.7.jar
  * [TAB-8537] Vulnerable 3rd party component logback used
  * [TAB-8550] Vulnerable 3rd party component shiro used
  * [TAB-8556] Vulnerable 3rd party component logback-core used
  * Third-party library upgrades:
    *   bytebuddy 1.14.11
    *   byteman 4.0.22
    *   commons-cli 1.6.0
    *   commons-logging 1.3.0
    *   guava 33.0.0-jre
    *   jackson 2.16.1
    *   jaxb-runtime 2.3.9
    *   jersey 2.41
    *   jetty 10.0.19
    *   logback 1.2.13
    *   rest-assured 5.4.0
    *   shiro 1.13.0       

### 4.4.0.10
* Release Date: 2024/02/23
* Resolved
  * none
* Security Updates to Third Party Libraries
  * [TAB-8673] Vulnerable 3rd party component json-path used
  * Third-party library upgrades:
    *   json-path updated to 2.9.0

### 4.4.0.11
* Release Date: 2024/03/23
* Resolved
  * none
* Security Updates to Third Party Libraries
  * [TAB-8727] Vulnerable 3rd party component eclipse-jetty used
  * Third-party library upgrades:
    *   eclipse-jetty updated to 10.0.20

### 4.4.0.12
* Release Date: 2024/05/09
* Resolved
  * Update to generation of install instructions
* Security Updates to Third Party Libraries
  * none

### 4.4.0.13
* Release Date: 2024/06/07
* Resolved
  * Updates to manifest for java 17
* Security Updates to Third Party Libraries
  * none

### 4.4.0.14
* Release Date: 2024/07/11
* Resolved
  * none
* Security Updates to Third Party Libraries
  *   [TAB-9448] Allow user to configure secure cookie attribute
  *   Don't set cookies secure in an INI setup, Jetty handles that when SSL is enabled

### 4.4.0.15
* Release Date: 2024/11/11
* Resolved
  * none
* Security Updates to Third Party Libraries
  *   [TAB-9591] Update jetty to 10.0.24

### 4.4.0.16
* Release Date: 2024/12
* Resolved
  * [TAB-9603] Update tanuki license to IBM
* Security Updates to Third Party Libraries
  * none

### 4.4.0.17
* Release Date: 2025/03/27
* Resolved
  * none
* Security Updates to Third Party Libraries
  *  Update to jetty 12

### 4.4.0.18
* Release Date: 2025/06/23
* Resolved
  * none
* Security Updates to Third Party Libraries
  * [TAB-9653] Disable the secure flag on cookies by default
  * [TAB-9654] Mask sensitive data in log files
  * [TAB-9655] Mask sensitive query parameters in logged URIs
  * Third-party library upgrades
  * jackson-annotations to 2.19.0
  * jackson-core to 2.19.0
  * jackson-databind to 2.19.0
  * guava to 33.4.8-jre
  * commons-beanutils to 1.11.0
  * commons-codec to 1.18.0
  * commons-io to 2.19.0
  * commons-logging to 1.3.5
  * commons-collections4 to 4.5.0
  * jetty to 12.0.21
  * slf4j-api to 2.0.17

### 4.4.0.19
* Release Date: 2025/08/04
* Resolved
  * none
* Security Updates to Third Party Libraries
  * [TAB-9691] Vulnerable 3rdparty component commons-lang3 used
  * Third-party library upgrades
  * commons-lang to 3.18.0
  * Jetty update to 12.0.23

### 4.4.0.20
* Release Date: 2025/08/18
* Resolved
  * Internal maintenance release of automation build processes
* Security Updates to Third Party Libraries
  * none

### 4.4.0.21
* Release Date: 2025/08/28
* Resolved
  * Update base docker image version
* Security Updates to Third Party Libraries
  * none

### 4.4.0.22
* Release Date: 2025/09/15
* Resolved
  * none
* Security Updates to Third Party Libraries
  * [TAB-9724] Vulnerable 3rdparty component jetty-http2-common used
  * Third-party library upgrades
  * Update Jetty to 12.0.25

### 4.4.0.23
* Release Date: 2025/09/26
* Resolved
  * [TAB-9721] Update tanuki to latest version for 4.4.0, 4.4.1, 4.3.10
  * Update base docker image version
* Security Updates to Third Party Libraries
  * none

### 4.4.0.24
* Release Date: 2025/12/05
* Resolved
  * [TAB-9685] fix broken management scripts
  * Update base docker image version
* Security Updates to Third Party Libraries
  * none

### 4.4.0.25
* Release Date: 2025/12/22
* Resolved
  * [TAB-9630] disallow concurrent login main
  * [WF-34500] Implementing MFA using RFC-6238
* Security Updates to Third Party Libraries
  * none

### 4.4.0.26
* Release Date: 2025/12/22
* Resolved
  * none
* Security Updates to Third Party Libraries
  * Update base docker image version

### 4.4.0.27
* Release Date: 2026/05/25
* Resolved
  * Internal maintenance items.
  * [TAB-9934] Update README.txt file to include Shiro 2 INI password information
* Security Updates to Third Party Libraries
  * Update base docker image version 
  * [TAB-9624] Vulnerable 3rd party component logback used [ TAB-9622 Code-Rollin 4.4.0]
  * [TAB-9659] Logback is still vulnerable post fix installation
  * [TAB-9787] CLONE - TC - Vulnerable 3rdparty components found in docker image ibmwebmethods.azurecr.io/webmethods-microservicesruntime:10.15.0.22 (logback)
  * [TAB-9875] Vulnerable 3rdparty component logback-core used
  * [TAB-9911] Update vulnerable shiro-core-1.13.0-jakarta.jar, shiro-core-1.13.0.jar
  * [TAB-9915] Vulnerable 3rd party component shiro-core reported
  * [TAB-9924] Update logback to 1.5.32 [4.4.0, 4.5.0, 4.5.1]
  * [TAB-9977] Vulnerable 3rd party component jetty used [4.4.0]
  * Library Updates:
    * asm to 9.9.1
    * bcprov-jdk18on to 1.84    
    * commons-cli to 1.11.0
    * commons-codec to 1.21.0
    * commons-io to 2.21.0
    * commons-lang3 to 3.20.0
    * guava to 33.5.0-jre
    * jackson to 2.21.1
    * jaxb to 4.0.6
    * jersey to 3.1.11
    * jetty to 12.0.34
    * logback to 1.5.32
    * shiro to 2.1.0
    * slf4j to 2.0.17
   
### 4.4.0.28
* Release Date: 2026/06/22
* Resolved
  * Internal maintenance items.
* Security Updates to Third Party Libraries
  * Update base docker image version 
  * [TAB-10021] [4.4.0] Update logback to 1.5.34 due to CVE-2026-10532, CVE-2026-9828
  * [TAB-10031] Update shiro to 2.2.0 due to CVE-2026-43827, CVE-2026-43828, CVE-2026-44598, CVE-2026-48589

### 4.4.0.29
* Release Date: 2026/07/31
* Resolved
  * Internal maintenance items
* Security Updates to Third Party Libraries
  * Update base docker image version 
  * [TAB-10031] Update shiro to 2.2.1 due to CVE-2026-43827, CVE-2026-43828, CVE-2026-44598, CVE-2026-48589
  * [TAB-10051] Update jackson-databind due to CVE-2026-54512, CVE-2026-54513, CVE-2026-54514, CVE-2026-54515
  * [TAB-10099] Upgrade Jetty due to CVE-2026-6790, CVE-2026-8384
  * jetty to 12.0.37
  * shiro to 2.2.1
  * jackson-databind to 2.21.5

### 4.4.0.30
* Release Date: 2026/08/17
* Resolved
  * Internal maintenance items
* Security Updates to Third Party Libraries
  * Update base docker image version 
  * [TAB-10184] Update logback to 1.5.38  

### 4.4.0.31
* Release Date: 2026/08/28
* Resolved
  * Internal maintenance items
* Security Updates to Third Party Libraries
  * Update base docker image version 
  * [TAB-10193] Update bcprov-jdk18on to latest (1.85.2)
  * bcprov-jdk18on to 1.85.2
 
### 4.4.0.32
* Release Date: 2026/09/14
* Resolved
  * Internal maintenance items
* Security Updates to Third Party Libraries
  * Update docker base image

### 4.4.0.33
* Release Date: 2026/10/09
* Resolved
  * Internal maintenance items
* Security Updates to Third Party Libraries
  * Update base docker image version 
  * jackson to 2.21.7
  * Jetty to 12.0.39  

### 4.4.0.34
* Release Date: 2026/10/26
* Resolved
  * Internal maintenance items
  * [TAB-10255] BigMemory Max Fix 31 installed but facing slowness in TC querying  
  * [TAB-10242] IBM BigMemory Max Server Image entrypoint looks for a license  
* Security Updates to Third Party Libraries
  * [TAB-10252] Security Vulnerability- Big Memory Max 4.4.0.32
  * Update base docker image version 
  * bcprov-jdk18on to 1.68
  * logback to 1.6.5
  * guava to 33.7.2-jre  
  * Jetty to 12.0.40
  * slf4j to 2.0.20

### 4.4.0.35
* Release Date: 2026/11/08
* Resolved
  * Internal maintenance items
* Security Updates to Third Party Libraries
  * Update base docker image version 
  * logback to 1.6.6
  * jackson update to 2.21.8
  * json-smart to 2.4.11
  * shiro to 3.0.1

<!-- Next entrypoint -->  
<br>

# Notes
-------
* Terracotta BigMemory 4.x and Terracotta 10.x clients may be used simultaneously in the same application by ensuring ClassLoader isolation when initializing at least one of the clients.
<br>


# Important Upgrade Information
-------
The following information is contained in the readme.txt file included with each fix release and should be reviewed prior to applying any fix.
<br>
```
8.0 Installation

8.1 Shut down the server array. A safe shutdown procedure is as follows.

  a. Shut down the mirror servers using the stop-tc-server script.
      If you are using a wrapper solution to manage the mirror servers, execute the wrapper shut
      down command to shut down the mirror servers instead of using the stop-tc-server script.

  b. Shut down the clients. A terracotta client will shut down when you shut down your application.

  c. Shut down the active servers using the stop-tc-server script.
      If you are using a wrapper solution to manage the servers, execute the wrapper shut down
      command to shut down the servers instead of using the stop-tc-server script.

8.2 This fix overwrites server scripts,wrapper configuration files and default tc-config.xml. If
    you have any custom settings defined on those files (ex:MaxDirectMemorySize), then you need to
    restore those settings back after applying the fix.

8.3 Install using IBM webMethods Update Manager. For instructions, see the documentation at
    https://docs.webmethods.io/.

8.4 IMPORTANT: File-Based INI Security Configuration Changes

    IBM BigMemory Max has migrated from Apache Shiro 1 to Apache Shiro 2 due to security
    vulnerabilities (CVEs) in Shiro 1. Shiro 2 uses the industry-standard Argon2 password hashing
    algorithm, providing significantly improved security over legacy hashing methods.

    You are NOT affected if:
      * You use LDAP or Active Directory for authentication
      * This is a fresh installation with no existing users

    You ARE affected if:
      * You use file-based INI security configuration to manage users
      * You have existing security.ini files with user credentials

    REQUIRED ACTIONS IF YOU ARE AFFECTED
    ------------------------------------
    All existing passwords in file-based INI security configurations MUST be regenerated to use the
    Argon2 hashing algorithm. Passwords hashed with the old Shiro algorithms will NO longer work.

    MIGRATION OPTIONS
    -----------------
    There are two options to migrate the security configuration:

      Option 1: Update existing security.ini file (RECOMMENDED)
      Update your existing security.ini file using the usermanagement script.
      This approach preserves existing user roles and permissions.

      Option 2: Recreate the security.ini file
      Create a new security.ini file from scratch with new user accounts and passwords.

    STEP-BY-STEP MIGRATION PROCEDURE
    ---------------------------------
    To update an existing security.ini file:

    1. Backup your current security.ini file
       Linux/Unix: cp security.ini security.ini.backup
       Windows:    copy security.ini security.ini.backup

    2. Run the usermanagement script for each user
       Linux/Unix: ./usermanagement.sh -f /path/to/security.ini -u username
       Windows:     usermanagement.bat -f C:\path\to\security.ini -u username

    3. Enter the new password when prompted
       - The script will re-hash the password using Argon2
       - All existing roles associated with the user will be preserved

    4. Repeat steps 2-3 for ALL users in your security.ini file

    5. Test the updated configuration before deploying to production

    IMPORTANT WARNINGS
    ------------------
    ** BACKWARD COMPATIBILITY **
    Once you have updated your security.ini file with Argon2 hashes, it CANNOT be used with earlier
    versions of IBM BigMemory Max. Always maintain a backup of your original file.

    ** DEPLOYMENT PLANNING **
    Plan your migration carefully if you have multiple IBM BigMemory Max instances. All instances
    must be upgraded before deploying the updated security.ini file.

    SECURITY BENEFITS
    -----------------
    This migration provides:
      * Protection against modern password cracking techniques
      * Compliance with current security best practices
      * Resistance to GPU-based brute force attacks
      * Memory-hard algorithm that increases attack costs

    ADDITIONAL RESOURCES
    --------------------
    For detailed information on authentication and authorization setup, see:
    IBM Documentation: Setting up Authentication/Authorization
    https://www.ibm.com/docs/en/webmethods-integration/bigmemory-max/${sumProductVersion}?topic=security-setting-up-authenticationauthorization

8.5 The upgrade of the 3rd party library Shiro may create an issue for some users that will require
    a manual configuration change to the "shiro.ini" found in the ".tc/mgmt" directory of the
    user's home folder (the user that the TMS/TMC process runs as ~/.tc/mgmt/shiro.ini). Edit this
    file and restart the TMS/TMC.

      a. Blank browser page or a message from the browser indicating too many redirects, or similar.
       In [urls] section of file ~/.tc/mgmt/shiro.ini, locate the line in the that reads
       "/login.jsp = authc". Immediately above that line add the three following lines:

       /401.jsp = anon
       /403.jsp = anon
       /404.html = anon

       In the [main] section of file ~/.tc/mgmt/shiro.ini, add the following line:

       [main]
       shiro.filterOncePerRequest=true

    b. URLs containing semi-colon are blocked and 400 client error is thrown.
       In the [main] section of file ~/.tc/mgmt/shiro.ini, add the following two lines to the top
       of the section:

       [main]
       invalidRequest = org.apache.shiro.web.filter.InvalidRequestFilter
       invalidRequest.blockSemicolon = false

    c. Previously, secure cookies in TMS were enabled by default, working only with TLS-secured
       connections or localhost requests. Remote HTTP access required adding the following line to
       the ~/.tc/mgmt/shiro.ini file:

       [main]
       securityManager.sessionManager.sessionIdCookie.secure = false

       The default value for this setting is now set to false. A restart of the TMS for changes
       to take effect.

8.6 As part of the Apache Shiro upgrade to 2.2.1, Terracotta Management Server and Terracotta server now automatically
    escape RFC 2253 special characters in usernames when building LDAP or AD Distinguished Names.
    If your LDAP or AD usernames contain special characters and userDnTemplate is configured, those characters no longer
    need to be manually escaped at login or when configuring the username.
    The only exception is AD configurations that do not configure userDnTemplate and use a full Distinguished Name for login.

8.7 To help customers avoid a mistakenly insecure setup, Terracotta Management Server (TMS) is no longer shipped with an
    example keystore (dev-keystore.jks).

    To enable HTTPS in a new TMS setup:

    Remove the .disabled extension from both files under <kit_install>/tools/management-console/start.d/:
    i. ssl.ini.disabled
    ii. https.ini.disabled

    Edit ssl.ini and replace the template placeholders with your real keystore path and passwords.

    If you already have an existing HTTPS setup, back up your existing ssl.ini and https.ini before upgrading. Then
    re-enable HTTPS following the steps above, restoring your keystore paths and passwords into the ssl.ini

    A JKS keystore containing a private key and its corresponding TLS/SSL certificate can be generated using the JDK
    keytool utility. For more information on generating a JKS keystore, see
    https://www.ibm.com/docs/en/webmethods-integration/bigmemory-max/4.5.1?topic=security-creating-server-certificates

9.0 Uninstallation

Note: These instructions can only be used to uninstall the most recently installed fix. This action
will revert your installation to the previously installed fix. You cannot use these instructions to
uninstall the previously installed fix.

9.1 Shut down the server array. A safe shutdown procedure is as follows.

  a. Shut down the mirror servers using the stop-tc-server script.
      If you are using a wrapper solution to manage the mirror servers, execute the wrapper shut
      down command to shut down the mirror servers instead of using the stop-tc-server script.

  b. Shut down the clients. A Terracotta client will shut down when you shut down your application.

  c. Shut down the active servers using the stop-tc-server script.
      If you are using a wrapper solution to manage the servers, execute the wrapper shut down
      command to shut down the servers instead of using the stop-tc-server script.

9.2 Uninstall using IBM webMethods Update Manager. For instructions, see the documentation at
    https://docs.webmethods.io/.
```
	  
<br>

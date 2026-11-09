---
title:  BigMemory Max 4.5.1 Release Notes and Notifications
lang: en
layout: page
keywords:
space: current
sidebar: lb2_sidebar
permalink: /display/release/BigMemory+Max+4.5.1.html
summary:
---

BigMemory Max delivers ultrafast access to hundreds of terabytes of in-memory data. BigMemory snaps into enterprise applications to deliver unmatched performance at any scale.

BigMemory Max supports a distributed in-memory data-storage topology, which enables the sharing of data among multiple caches and in-memory data stores in multiple JVMs. It uses a Terracotta Server Array to manage data that is shared by multiple application nodes in a cluster.

The Ehcache 2.12.1.x API can be used with BigMemory Max 4.5.1.x as a general-purpose cache/in-memory data store or a second-level cache for Hibernate. You can additionally integrate it with third-party products such as Google App Engine, Spring, and others.

------

<br>

Document Contents

* TOC
{:toc}

<br>

## Current Release
------------------
BigMemory Max 4.5.1 (May 2026) is the latest release. It includes Ehcache 2.12.1.

Fixes are cumulative from version to version within the BigMemory Max 4.5.1 product line.

<br>

## Feature Highlights
-------------------
BigMemory Max 4.5.1 introduced the following new capabilities:

* Rebranding for IBM
* Support for Java 21
* Security enhancements and bug fixes
* Contains all features and functionality included in [BigMemory Max 4.4.x](https://confluence.terracotta.org/display/release/BigMemory+Max+4.4)

<br>

# Summary of Changes 4.5.1.1
-----------------------
### 4.5.1.1
* Release Date: 2026/06/22
* Resolved
  * Internal maintenance items
* Security Updates to Third Party Libraries
  * Update base docker image version 
  * [TAB-10019] [4.4.0] Update logback to 1.5.34 due to CVE-2026-10532, CVE-2026-9828  
  * [TAB-10031] Update shiro to 2.2.0 due to CVE-2026-43827, CVE-2026-43828, CVE-2026-44598, CVE-2026-48589

### 4.5.1.2
* Release Date: 2026/07/16
* Resolved
  * Internal maintenance items
* Security Updates to Third Party Libraries
  * Update base docker image version 
  * [TAB-10031] Update shiro to 2.2.1 due to CVE-2026-43827, CVE-2026-43828, CVE-2026-44598, CVE-2026-48589
  * [TAB-10051] Update jackson-databind due to CVE-2026-54512, CVE-2026-54513, CVE-2026-54514, CVE-2026-54515  
  * shiro to 2.2.1
  * jackson-databind to 2.21.5

### 4.5.1.3
* Release Date: 2026/07/31
* Resolved
  * Internal maintenance items
* Security Updates to Third Party Libraries
  * Update base docker image version 
  * [TAB-10099] Upgrade Jetty due to CVE-2026-6790, CVE-2026-8384
  * jetty to 12.0.37

### 4.5.1.4
* Release Date: 2026/08/13
* Resolved
  * Internal maintenance items
* Security Updates to Third Party Libraries
  * Update base docker image version 
  * [TAB-10184] Update logback to 1.5.38

### 4.5.1.5
* Release Date: 2026/08/28
* Resolved
  * Internal maintenance items
* Security Updates to Third Party Libraries
  * Update base docker image version 
  * [TAB-10193] Update bcprov-jdk18on to latest (1.85.2)
  * bcprov-jdk18on to 1.85.2

### 4.5.1.6
* Release Date: 2026/09/14
* Resolved
  * Internal maintenance items
* Security Updates to Third Party Libraries
  * Update base docker image version 

### 4.5.1.7
* Release Date: 2026/10/09
* Resolved
  * Internal maintenance items
* Security Updates to Third Party Libraries
  * Update base docker image version
  * jackson to 2.21.6
  * Jetty to 12.0.39

### 4.5.1.8
* Release Date: 2026/10/26
* Resolved
  * Internal maintenance items
  * [TAB-10255] BigMemory Max Fix 31 installed but facing slowness in TC querying
* Security Updates to Third Party Libraries
  * [TAB-10252] Security Vulnerability- Big Memory Max 4.4.0.32
  * [TAB-10242] IBM BigMemory Max Server Image entrypoint looks for a license
  * Update base docker image version 
  * bcprov-jdk18on to 1.68
  * logback to 1.6.5
  * jackson to 2.21.7
  * guava to 33.7.2-jre
  * Jetty to 12.0.40
  * slf4j to 2.0.20

### 4.5.1.9
* Release Date: 2026/11/10
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
* Terracotta BigMemory 4.5.1.x and Terracotta 12.1.x clients may be used simultaneously in the same application by ensuring ClassLoader isolation when initializing at least one of the clients.
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

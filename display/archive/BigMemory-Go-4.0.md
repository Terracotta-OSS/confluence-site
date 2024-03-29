---
title:  BigMemory Go 4.0  
lang: en
layout: page
keywords:
space: archive
sidebar: lb2_sidebar
permalink: /display/archive/BigMemory+Go+4.0.html
summary:
---

BigMemory Go 4.0 introduces various enhancements in management tools and restartability.  The new version of BigMemory Go includes various UX and functional enhancements in Terracotta Management Console (TMC).  The improved restartable store provides enhancements including ability to take live backup of in-memory data. BigMemory Go supports Java 7. 

* * *

#### BigMemory Go 4.0.2

##### Resolved Issues

*   9180 - Setting maxEntriesInCache to -1 dynamically doesn't work
*   8953 - Fails to start up if logs directory removed
*   9046 - Unsecured REST agents accept TMS connection with secure parameters
*   9075 - Intermittent issue: "There are no CacheManagers" message shown in TMC's Application Tab
*   9090 - TMC becomes unresponsive after running for a extended period of time
*   9216 - Issue configuring ini-based security; Workaround: create a dummy keychain file.  e.g. on unix execute "touch ~/.tc/mgmt/keychain", prior to restarting the TMS after enabling security

##### Known Issues

*   9535 - Large scale test, with numerous event messages cause TMC to be unresponsive to scroll
*   9910 - Must encode Cache name when injecting into HTML text  
      
    

#### BigMemory Go 4.0.0 Known Issues

*   9180 - Setting maxEntriesInCache to -1 dynamically doesn't work
*   8953 - Fails to start up if logs directory removed
*   9046 - Unsecured REST agents accept TMS connection with secure parameters
*   9075 - Intermittent issue: "There are no CacheManagers" message shown in TMC's Application Tab
*   9090 - TMC becomes unresponsive after running for a extended period of time
*   9216 - Issue configuring ini-based security; Workaround: create a dummy keychain file.  e.g. on unix execute "touch ~/.tc/mgmt/keychain", prior to restarting the TMS after enabling security



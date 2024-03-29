---
title:  BigMemory Go 4.0.0  
lang: en
layout: page
keywords:
space: archive
sidebar: lb2_sidebar
permalink: /display/archive/BigMemory+Go+4.0.0.html
summary:
---

BigMemory Go 4.0 introduces various enhancements in management tools and restartability.  The new version of BigMemory Go includes various UX and functional enhancements in Terracotta Management Console (TMC).  The improved restartable store provides enhancements including ability to take live backup of in-memory data. BigMemory Go supports Java 7. 

* * *

#### BigMemory Go 4.0.0 Known Issues

*   DEV-9180 - Setting maxEntriesInCache to -1 dynamically doesn't work
*   DEV-8953 - Fails to start up if logs directory removed 
*   DEV-9046 - Unsecured REST agents accept TMS connection with secure parameters
*   DEV-9075 - Intermittent issue: "There are no CacheManagers" message shown in TMC's Application Tab
*   DEV-9090 - TMC becomes unresponsive after running for a extended period of time
*   DEV-9216 - Issue configuring ini-based security; Workaround: create a dummy keychain file.  e.g. on unix execute "touch ~/.tc/mgmt/keychain", prior to restarting the TMS after enabling security



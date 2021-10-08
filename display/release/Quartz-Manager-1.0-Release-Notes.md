Product Information : Quartz Manager 1.0 Release Notes  

1.  [Product Information](index.html)
2.  [Home](Home.html)

Product Information : Quartz Manager 1.0 Release Notes
======================================================

Created by Fiona OShea, last modified on Jan 27, 2012

/\*<!\[CDATA\[\*/ div.rbtoc1633463967582 {padding: 0px;} div.rbtoc1633463967582 ul {list-style: disc;margin-left: 0px;} div.rbtoc1633463967582 li {margin-left: 0px;padding-left: 0px;} /\*\]\]>\*/

*   [Quartz Manager 1.0.2](#QuartzManager1.0ReleaseNotes-QuartzManager1.0.2)
    *   [Resolved Issues](#QuartzManager1.0ReleaseNotes-ResolvedIssues)
*   [Quartz Manager 1.0.1](#QuartzManager1.0ReleaseNotes-QuartzManager1.0.1)
    *   [Resolved Issues](#QuartzManager1.0ReleaseNotes-ResolvedIssues.1)
*   [Quartz Manager 1.0.0](#QuartzManager1.0ReleaseNotes-QuartzManager1.0.0)
    *   [Overview](#QuartzManager1.0ReleaseNotes-Overview)
    *   [Details](#QuartzManager1.0ReleaseNotes-Details)
*   [Known Open Issues](#QuartzManager1.0ReleaseNotes-KnownOpenIssues)

### Quartz Manager 1.0.2

Bug fix release

##### Resolved Issues

*   [QTZ-156](https://jira.terracotta.org/jira/browse/QTZ-156) - Do not save connections authentication data to connection-store.xml, use browser cookies instead
*   6148 - Quartz manager remember the latest username/password details

### Quartz Manager 1.0.1

Update the Quartz Manager to run with the 2.1.0 version of Quartz Scheduler.

##### Resolved Issues

*   5774/5926 - Successful or Failed Jobs List is not always consistent with the jobs that were triggered

### Quartz Manager 1.0.0

##### Overview

Quartz Manager provides enterprise-class monitoring and management capabilities for use in both development and production. It provides access to one or more Quartz Scheduler instances from a single web console. The application runs either as a Java web app in your own container (such as Tomcat), or as a standalone Java app with its own Jetty container. The app functions as a JMX client to the remote Quartz Schedulers. The web user interface is an Adobe Flex client application that runs in web browsers with an Adobe FlashPlayer plug-in.

##### Details

Features

*   Manage multiple Quartz Schedulers embedded within any remote JVM
*   Connect to remote Quartz Schedulers via JMX; support is included for JMX Authentication and SSL
*   View status and details, pause, resume and shutdown schedulers
*   Create, update, and monitor the jobs for a Quartz Scheduler
*   Schedule, pause, and remove triggers

Note: some features, such as the ability to schedule triggers, and to add and schedule job in a single step - as described in the product documentation packaged with the product - require Quartz 2.0

Deployment Options

*   As a standalone Jar (with it's own built-in Jetty contaner)
*   As a deployable War file - compatible with Apache Tomcat 5.5.23 or newer

Compatibility

*   Quartz 1.8.3 or newer (with JMX configured)
*   Java 1.6
*   A Flash-enabled browser: IE7, Firefox 3.x, Chrome 9, Safari 4, Opera 9 or newer

* * *

### Known Open Issues

*   QTM-45 - No way to persist job execution history
*   QTM-47 - Job completion status not shown
*   QTM-52 - Manager does not detect addition of new scheduler
*   QTM-56 - Current selections are not maintained after operations

Document generated by Confluence on Oct 05, 2021 15:59

[Atlassian](http://www.atlassian.com/)
---
title:  FAQ How to Become a Terracotta Contributor  
lang: en
layout: page
keywords:
space: current
sidebar: lb2_sidebar
permalink: /display/release/How+to+Become+a+Terracotta+Contributor
summary:
---

Become a Contributor
====================

Being a contributor means you get to work on the Terracotta source code. This is an excellent way to help us make the product even better, or to influence what types of features or bugs are worked on.

Read below to find out more about being a contributor.

How To Start
------------

The basic steps to becoming a contributor or committer to Terracotta are as follows:

*   Check out and get familiar with the source code:

*   *   [Source Repository](http://www.terracotta.org/community/source)

After that, there's a committer acceptance process that includes submitting the first few contributions as patches, then, based on those contributions, a community vote.

[Contact Us](mailto:info@terracotta.org?subject=Interested in Contributing to Terracotta) if you would like more information on becoming a Terracotta contributor.

Contributor / Committer Agreements
----------------------------------

After you get in touch with us, you'll be asked to sign and return one of:

*   [The Terracotta Contributor Agreement](/download/attachments/27918462/TerracottaIndividualContributorAgreementv4.pdf)
*   [The Terracotta Committer Agreement](/download/attachments/27918462/Committer Agreement.pdf)

Documentation
-------------

[User Documentation](http://www.terracotta.org/documentation/)  
[Developer Documentation](http://terracotta-org.terracotta.eur.ad.sag/community/)

Source Repository
-----------------

All information on accessing our source code is here:

*   [Source Repository](http://www.terracotta.org/community/source)

Contribute Patches
------------------

Create the patches using `svn` or `diff`. Make sure that you turn on the `-u` option and that you give the patch a meaningful name. Diffs should be run from the top-level directory.

For example:

`svn diff -x -u path/to/Foo.java > foo-fix.patch`

or

`diff -u Foo.java.orig path/to/Foo.java > foo-fix.patch`

Then create an issue on the JIRA issue tracking system, provide a detailed description about what the patch does and add the patch file to the issue as an attachment. If you did not run the diff from the top-level directory, please specify what subdirectory you ran it from so the patch can be properly applied.

Community Code of Conduct
-------------------------

**Principles:**

1.  Always treat people involved in the project with respect.
2.  If you are a committer you are expected to show excellent judgement and communicate appropriately with the other developers before making changes.
3.  We encourage committers to strive for quality.
4.  New committers are expected to ease themselves in with small commits to start, and greater free-will may be assumed later.
5.  Terracotta encourages people to be brief in email and to honor internet etiquette.

Attachments:
------------

![Bullet](images/icons/bullet_blue.gif) [Individual Contributor Agreement.pdf](/download/attachments/27918462/Individual Contributor Agreement.pdf) (application/pdf)  
![Bullet](images/icons/bullet_blue.gif) [Committer Agreement.pdf](/download/attachments/27918462/Committer Agreement.pdf) (application/pdf)  
![Bullet](images/icons/bullet_blue.gif) [Individual Contributor Agreement.pdf](/download/attachments/27918462/Individual Contributor Agreement.pdf) (application/pdf)  
![Bullet](images/icons/bullet_blue.gif) [Terracotta Individual Contributor Agreement v3.pdf](/download/attachments/27918462/Terracotta Individual Contributor Agreement v3.pdf) (application/pdf)  
![Bullet](images/icons/bullet_blue.gif) [Terracotta Individual Contributor Agreement v4.docx](/download/attachments/27918462/Terracotta Individual Contributor Agreement v4.docx) (application/vnd.openxmlformats-officedocument.wordprocessingml.document)  
![Bullet](images/icons/bullet_blue.gif) [TerracottaIndividualContributorAgreementv4.pdf](/download/attachments/27918462/TerracottaIndividualContributorAgreementv4.pdf) (application/pdf)  



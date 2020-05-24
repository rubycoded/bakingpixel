---
id: 2024
title: Asus routers allow strangers to access your files
date: 2014-02-19T00:13:10+00:00
author: Matt
layout: post
guid: http://bakingpixel.com/?p=2024
permalink: /2014/02/19/asus-routers-allow-strangers-to-access-your-files/
categories:
  - News
tags:
  - asus
  - networking
  - security
---
It&#8217;s 2014, so security issues are the norm rather than the exception, but the latest news that Asus [left the door wide open](http://arstechnica.com/security/2014/02/dear-asus-router-user-youve-been-pwned-thanks-to-easily-exploited-flaw/) on many of its routers is extremely disturbing.

The fact that anybody with your IP address will be able to login anonymously to your attached storage device is bad enough, it&#8217;s much worse that a [list of almost 13,000 IP addresses](http://pastebin.com/ASfYTWgw) of people who are using these vulnerable routers was published online. In simpler terms, that means your home address has been published online, and your front door isn&#8217;t locked.

> Going through the file listings of other IP addresses I see insanely personal items like whole backups of laptops, family photos, porn collections, and tax documents. Anyone that has the list of IP addresses can potentially download any of those files. I wrote some python to walk through the list of IP addresses and check to see if logging in anonymously is still possible. I’m not bothering to look at anything just see if ftp.login() works and recording the statistics. The numbers are not reassuring. The code is also on pastebin for those who want to run it and help report the numbers. 

So far the [incidents](http://blogs.law.harvard.edu/zeroday/2014/02/05/so-this-is-what-getting-pwned-is-like/) that have surfaced due to this security issue haven&#8217;t been too serious, but it could be a lot worse if someone decided that it&#8217;d be a good idea to create a script to access the files of the affected users and delete all the files, or insert some sort of malware.

To make things worse, it took Asus a long time to finally [release a patch](http://news.softpedia.com/news/ASUS-Fixes-Vulnerabilities-in-RT-N66U-RT-N66R-and-RT-N66W-Routers-426689.shtml). Patching the vulnerability is the first step, but the question is how many folks out there who own the affected routers are aware of the issue and know how to patch their routers?

Asus really botched this one badly.
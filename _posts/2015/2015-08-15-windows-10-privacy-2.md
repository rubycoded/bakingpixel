---
id: 2927
title: Even when told not to, Windows 10 just can’t stop talking to Microsoft
date: 2015-08-15T20:38:32+01:00
author: Jenxi
layout: post
guid: http://bakingpixel.com/?p=2927
permalink: /2015/08/15/windows-10-privacy-2/
categories:
  - News
tags:
  - microsoft
  - privacy
  - windows 10
---
Ars Technica reported on [Windows 10 talking to Microsoft even when told not to](http://arstechnica.co.uk/information-technology/2015/08/even-when-told-not-to-windows-10-just-cant-stop-talking-to-microsoft/).

> For example, even with Cortana and searching the Web from the Start menu disabled, opening Start and typing will send a request to www.bing.com to request a file called threshold.appcache which appears to contain some Cortana information, even though Cortana is disabled. The request for this file appears to contain a random machine ID that persists across reboots.
> 
> [&#8230;]
> 
> Some of the traffic looks harmless but feels like it shouldn&#8217;t be happening. For example, even with no Live tiles pinned to Start (and hence no obvious need to poll for new tile data), Windows 10 seems to download new tile info from MSN&#8217;s network from time to time, using unencrypted HTTP to do so. While again the requests contain no identifying information, it&#8217;s not clear why they&#8217;re occurring at all, given that they have no corresponding tile.
> 
> Other traffic looks a little more troublesome. Windows 10 will periodically send data to a Microsoft server named ssw.live.com. This server seems to be used for OneDrive and some other Microsoft services. Windows 10 seems to transmit information to the server even when OneDrive is disabled and logins are using a local account that isn&#8217;t connected to a Microsoft Account. The exact nature of the information being sent isn&#8217;t clear—it appears to be referencing telemetry settings—and again, it&#8217;s not clear why any data is being sent at all. We disabled telemetry on our test machine using group policies. 

When disabling services doesn&#8217;t really disable them.
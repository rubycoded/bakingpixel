---
id: 3114
title: New Android ransomware locks out victims by changing lock screen PIN
date: 2015-09-12T12:12:33+01:00
author: Jenxi
layout: post
guid: http://bakingpixel.com/?p=3114
permalink: /2015/09/12/android-ransomware/
categories:
  - News
tags:
  - android
  - security
---
Ars Technica reported on [a new Android ransomware that locks out victims by changing lock screen PIN](http://arstechnica.com/security/2015/09/new-android-ransomware-locks-out-victims-by-changing-lock-screen-pin/).

> Dubbed Android/Lockerpin.A, the app first tricks inexperienced users into granting it device administrator privileges. To achieve this, it overlays a bogus patch installation window on top of an activation notice. When targets click on the continue button, they really grant the malicious app elevated rights that allow it to make changes to the Android settings. From there, Lockerpin sets or resets the PIN that unlocks the screen lock, effectively requiring users to perform a factory reset to regain control over the device. By contrast, earlier forms of Android ransomware generally were thwarted, usually by deactivating administrator privileges and then uninstalling the app after the infected device is booted into safe mode.
> 
> &#8220;After clicking on the button, the user&#8217;s device is doomed,&#8221; Lukas Stefanko, a researcher with antivirus provider Eset, wrote in a blog post published Thursday. &#8220;The trojan app has obtained administrator rights silently and now can lock [the] device—and even worse, it set[s] a new PIN for the lock screen. Not long after, the user will be prompted to pay a $US500 ransom for allegedly viewing and harboring forbidden pornographic material.&#8221; 

Why would a developer be able overlay a notice?
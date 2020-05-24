---
id: 3219
title: Google’s own researchers challenge key Google PR on Android
date: 2015-09-26T17:58:37+01:00
author: Jenxi
layout: post
guid: http://bakingpixel.com/?p=3219
permalink: /2015/09/26/google-researcher-android/
categories:
  - News
tags:
  - android
  - google
---
Ars Technica reported on [Google’s own researchers challenging key Android security talking point](http://arstechnica.com/security/2015/09/googles-own-researchers-challenge-key-android-security-talking-point/).

> Throughout the resulting media storm, Google PR people have repeatedly held up the assurance that the raft of stagefright vulnerabilities is difficult to exploit in practice on phones running recent Android versions. The reason, they said: address space layout randomization, which came to maturity in Android 4.1, neutralizes such attacks. Generally speaking, ASLR does nothing to fix a buffer overflow or similar software bug that causes the vulnerability in the first place. Instead, the defense vastly decreases the chances that a remote-code-execution attack exploiting such bugs will succeed. ASLR does this by loading downloaded scripts in a different memory location each time the operating system is rebooted. If the attacker can&#8217;t locate the malicious code, the exploit results in a simple crash, rather than a game-over hack.
> 
> On Wednesday, Project Zero researchers tested a home-grown stagefright exploit on a Nexus 5 device running an Android 5.x version. The results showed that at best, ASLR will lower the chances their exploit will succeed. Meanwhile, Joshua Drake, the security researcher who first disclosed the critical vulnerabilities in the code library, said Android ASLR does even less to prevent a new custom exploit he has developed from working.
---
id: 2539
title: Android password manager vulnerability unpatched after almost two years
date: 2015-01-25T00:20:59+00:00
author: Jenxi
layout: post
guid: http://bakingpixel.com/?p=2539
permalink: /2015/01/25/android-password-manager/
categories:
  - News
tags:
  - android
  - password
  - security
---
Ars Technica reported on [Android password managers being wide open to sniffing attacks](ttp://arstechnica.com/security/2014/11/using-a-password-manager-on-android-it-may-be-wide-open-to-sniffing-attacks/).

> Almost two years later, the threat remains viable in at least some, if not all, of the apps originally analyzed. An app recently made available on Google Play, for instance, has no trouble divining the passwords managed by LastPass, one of the leading managers on the market, as well as the lesser-known KeePassDroid. With additional work, it&#8217;s likely that the proof-of-concept ClipCaster app would work seamlessly against many other managers, too, said Xiao Bao Clark, the Australia-based programmer who developed it. While ClipCaster does nothing more than display the plaintext of passwords that LastPass and KeePassDroid funnel through Android handsets, a malicious app with only network privileges could send the credentials to an attacker without the user having any idea what was happening. 

The vulnerability has been known since early 2013 but app developers are not keeping users informed of it:

> &#8220;Besides the insecurity of it, what annoyed me was that I was never told any of this while I was signing up or setting up the LastPass app,&#8221; Clark wrote in an e-mail. &#8220;Instead, I got the strong impression from LastPass that everything was very secure, and I needn&#8217;t worry about any of it. If they at least told users the security issues using these features brings, then the users themselves could decide on their own trade-off between usability and security. Not mentioning it at all strikes me as disingenuous.&#8221; 

The finger is pointed at Android for the source of this vulnerability:

> As already alluded, the threat stems from the use of the Android clipboard, which acts as a temporary cache for text that is being copied and pasted, either within the same app or from one app to another. Android has no official programming interface that secures the clipboard. By design, its contents are available to any app installed on the phone, from the highest privileged banking app to one with no privileges at all. (ClipCaster, for instance, requires no permissions.) Siegrist rightly noted that any password manager that makes use of the Android clipboard—and there are plenty, including LastPass—is vulnerable. 

Both the app developers and Android should be making users aware of such a vulnerability so that they can take measure to avoid having their passwords from being stolen.
---
id: 2252
title: 'New Android &#8216;Fake ID&#8217; flaw empowers stealthy new class of super-malware'
date: 2014-07-30T00:03:51+01:00
author: Jenxi
layout: post
guid: http://bakingpixel.com/?p=2252
permalink: /2014/07/30/android-fake-id-flaw/
categories:
  - News
tags:
  - android
  - malware
  - security
---
AppleInsider reported on [a new Android flaw that allows malware to gain extensive control over a user&#8217;s device](http://appleinsider.com/articles/14/07/29/new-android-fake-id-flaw-empowers-stealthy-new-class-of-super-malware-).

> This is particularly serious because Google has granted a variety of trusted apps in Android broad permissions; by pretending to be one of these trusted apps, malware can can fool users into thinking that they are installing an app that doesn&#8217;t need any special permissions, then trick the system into giving it essentially full control of the device, with access to the user&#8217;s financial data, contacts and other private information, even data stored in the cloud. 

Here are some possible apps for malwares to spoof.

Adobe Flash:

> While Google eventually gave up on Flash for Android, an Adobe Flash plugin privilege escalation flaw remained embedded in Android&#8217;s webview—the browser component that gets embedded into third party apps that present web content—until the release of Android 4.4 KitKat last fall.
> 
> With Flash so deeply integrated into Android&#8217;s webview component, any malware using Fake ID to pretend to be Flash can subsequently escape Android&#8217;s app sandbox and take control of other apps, including Salesforce and Microsoft OneDrive, grab data from those apps, sniff out all those apps&#8217; network traffic and gain any additional privileges held by those apps. 

The solution is simple: upgrade to Android 4.4 KitKat. However, not every Android user can upgrade even if they want to.

NFC:

> Using Fake ID, a malware app that asks the user for no special permissions at installation can subsequently pretend to be the Google Wallet app; Android will then provide the rogue app with all the permissions it gave its own NFC infrastructure, which includes users&#8217; financial data.
> 
> Because Wallet, 3LM and other apps do not depend on the Flash / Android webview flaw, these other vectors of attack weren&#8217;t fixed in KitKat. That means Fake ID affects all versions of Android, including the latest Android 4.4.4 and the upcoming &#8220;Android L&#8221; (aka Android 5.0 beta). 

This happens because Android apps are signed but not verified, unlike iOS apps.

> However, Bluebox discovered that &#8220;the Android package installer makes no attempt to verify the authenticity of a certificate chain; in other words, an identity can claim to be issued by another identity, and the Android cryptographic code will not verify the claim (normally done by verifying the issuer signature of the child certificate against the public certificate of the issuer).
> 
> &#8220;For example, an attacker can create a new digital identity certificate, forge a claim that the identity certificate was issued by Adobe Systems, and sign an application with a certificate chain that contains a malicious identity certificate and the Adobe Systems certificate.
> 
> &#8220;Upon installation, the Android package installer will not verify the claim of the malicious identity certificate, and create a package signature that contains the both certificates. This, in turn, tricks the certificate-checking code in the webview plugin manager (who explicitly checks the chain for the Adobe certificate) and allows the application to be granted the special webview plugin privilege given to Adobe Systems &#8211; leading to a sandbox escape and insertion of malicious code, in the form of a webview plugin, into other applications.&#8221; 

It is hard for you to know if you have been infected.

> On the other hand, Fake ID requires no user involvement, and can be used by malware posing as an innocent app or game that requests no special permissions. Once installed, the app can take over without the user having any knowledge of being infected. 

This underlines the shocking state of Android security.

> &#8220;The Android malware ecosystem is beginning to resemble to that which surrounds Windows,&#8221; the firm observed. By September, Duo Security stated that &#8220;more than half of Android devices are vulnerable to at least one of the known Android security flaws.&#8221;
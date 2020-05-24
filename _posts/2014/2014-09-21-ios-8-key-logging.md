---
id: 2305
title: Third party keyboard in iOS 8 key logging?
date: 2014-09-21T22:00:03+01:00
author: Jenxi
layout: post
guid: http://bakingpixel.com/?p=2305
permalink: /2014/09/21/ios-8-key-logging/
categories:
  - News
tags:
  - apple
  - ios 8
  - keyboard
---
Gabe Weatherhead wrote about [his concerns about iOS 8 key logging](http://www.macdrifter.com/2014/09/ios-8s-new-key-logger.html).

> This is what I found (quoted from the documentation):
> 
>   * All capabilities of a nonnetworked custom keyboard
>   * Keyboard can access Location Services and Address Book, with user permission
>   * Keyboard and containing app can employ a shared container
>   * Keyboard can send keystrokes and other input events for server-side processing
>   * Containing app can provide editing interface for keyboard’s custom autocorrect lexicon
>   * Via containing app, keyboard can employ iCloud to ensure settings and autocorrect lexicon are up to date on all devices
>   * Via containing app, keyboard can participate in Game Center and In-App Purchase
>   * If keyboard supports mobile device management (MDM), it can work with managed apps
> 
> My interpretation of the documentation is that a keyboard extension can enable network access if it is for the purpose of improving the application. What improvements warrant this, is up to the app developer. 

It is a concern I share as well. Why would a keyboard need to send keystrokes?
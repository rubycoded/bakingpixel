---
id: 6031
title: How to Restart the Touch Bar
date: 2020-05-11T15:00:03+01:00
author: Jenxi
layout: post
guid: https://bakingpixel.com/?p=6031
permalink: /2020/05/11/how-to-restart-the-touch-bar/
categories:
  - News
tags:
  - apple
  - macbook pro
  - macOS
  - touchbar
---
[Michael Tsai](https://mjtsai.com/blog/2020/04/21/how-to-restart-the-touch-bar/):

<blockquote class="wp-block-quote">
  <p>
    The Terminal commands are:
  </p>
  
  <p>
    <code>sudo pkill TouchBarServer</code><br /><code>sudo killall ControlStrip</code>
  </p>
</blockquote>

Useful commands. I killed TouchBarServer and ControlStrip via Activity Monitor.

I had issues when I first used my MacBook Pro. Three times in the past five months, though they seem to have disappeared after a recent macOS update.
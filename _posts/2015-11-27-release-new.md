---
layout: post
title: "Version 0.9.2 is released"
author: jeff_pei
modified:
excerpt: "Version 0.9.2 is released with fix for logback config."
tags: []
---

#### Version 0.9.2 is released


_2015-11-27_

* Build/Maven/Logback: exclude logback.xml in the built jar, thanks to [xmpp](http://stackoverflow.com/users/5178636/xmpp) for raising the [issue](http://stackoverflow.com/questions/33897196/how-to-disable-inherited-logback/33900287#33900287), close [#21](https://github.com/eBay/parallec/issues/21).
* Test: add sleep to make sure server starts first; should fix build issue related to [#7](https://github.com/eBay/parallec/issues/7)
* Test: add coverage: updateRequestByAddingReplaceVarPairNodeSpecific() check null, add some other minor coverage
* Test: fix TcpServerThread (tcp sample server) not closed in test, thus skip idle TCP tests. 

---
layout: post
title: 服务器的一些概念
date: Fri Jan 04 2019 14:24:26 GMT+0800 (中国标准时间)
---


#### 正向和反向代理
***正向代理***<br/>
通常指的是代理服务器vpn，特点就是隐藏了真实的请求客户端，服务端不知道真实的客户端是谁，客户端请求的服务都由代理服务器代替来请求。

举个例子，国内的用户想要访问 Google 时，会被阻挡。所以这个时候把请求发送到另外一个代理服务器（可以访问 Google 的服务器）上，由其代为转发请求和接收响应内容。

***反向代理***<br/>
反向代理和正向代理相反，但反向代理一般是负载均衡的一个原理。正向代理是一对一或者多对一，而反向代理一般是一对多或多对多。

反向代理隐藏了真实的服务端，当我们请求 http://www.baidu.com 的时候，就像拨打 QQ 客服热线一样，背后可能有成千上万台服务器为我们服务，但具体是哪一台，你不知道，也不需要知道，你只需要知道反向代理服务器是谁就好了，http://www.baidu.com 就是我们的反向代理服务器，反向代理服务器会帮我们把请求转发到真实的服务器那里去。

因此二者的区别在于代理的对象不一样，正向代理代理的对象是客户端，反向代理代理的对象是服务端。


[whatForwardProxyOrReverseUrl]: https://zhuanlan.zhihu.com/p/25707362



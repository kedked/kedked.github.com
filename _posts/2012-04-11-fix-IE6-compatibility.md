---
layout: post
title: 兼容性处理原则"
keyword: "IE兼容性,兼容性处理原则"
description: "兼容性处理原则"
category: code
tags: [兼容性,css,html,web标准,可用性]
---

这里主要讲我理解的兼容性处理通用原则。

在很多人之前的设计与理解中，重构就是做兼容性。当时我也有这样错误的为了表现而忽视分离的想法。其实重构的灵魂是[语义化，可用性及web标准]({{ site.url }}/blog/code/availability-and-web-standard.html "语义化，可用性及web标准").

所以在兼容性的处理上不能违背语义化，可用性和web标准。当然也要出于可维护性和性能方面的考虑。而一些要的功能或者效果存在兼容性问题，处理该兼容性的方法应该是这样的原则：

1.在处理兼容性的时候不应该引入无用，无语义化的标签及空白的图片，标准就为了避免如此，为何再加入呢 ？例如有些bug嵌套多层div来实现布局的bug，这种方法不是很明智。该标签是没有语义化的。
2.对于bug理解浏览器的特性会让你的觉得hack bugs也不是很麻烦，优先是通过浏览器的特性来处理，比如haslayout
3.为了可维护性，CSS hack分离出普通代码来进行管理
4.预防为主：我们要做到总结bug ，能够在bug未出现前就进行预防。和通常的处理事情的原则一致，预防为主。

一些参考：
IE bug集：[http://www.qianduan.net/ie-bug-resources.html](http://www.qianduan.net/ie-bug-resources.html)
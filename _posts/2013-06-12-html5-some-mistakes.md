---
layout: post
title: "html5易混淆的几个标签的理解"
keyword: "html5，标签"
description: "html5易混淆的几个标签的理解"
category: code
tags: [code,html5]
---

在实际使用中，html5新增的几个语义化标签让人抓急，该如何选择标签，是否正确使用。

###article与section

>setion:表示文档和应用的通用部分。在此上下文中，一节是一组专题内容，并通常有标题。
>article:表示文档页面自我包含的部门。原则上，是独立发布和重复使用的。
>

从上面的标准文档中。我们可以抓住关键词，setcion表示专题的，相关的。而article代表独立的部分。一个较好的实践方法是，联合测试，如何一段内容可以无需修改出现在其他页面或者网站上，那么就是用article，否则考虑section。而div 是无语义化的，联合测试在这个最后终止。例子和场景对于概念的理解十分有帮助，比如一篇文章，用户的评论等都是独立的，考虑article;而对于页尾的关于里面的简介及团队等部分，部分之间是关联的，但是每个都是专题的，考虑用section.

section与article都可以互相嵌套或者自己嵌套自己。

###header与footer
在一个页面中可以使用多个。header的语义需要注意，表示页面任意独立部分的前言或导航。

###hgrounp

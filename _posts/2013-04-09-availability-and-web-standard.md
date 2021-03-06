---
layout: post
title: "可用性、语义化、web标准的笔记"
keyword: "可用性,设计,html,web标准"
description: "可用性、语义化、web标准的笔记"
category: code
tags: [code,可用性,设计,html,web标准]
---

>web标准的灵魂是可用性。 ---《网站重构》

web标准和语义化的重点是结构和表现分离，以及可用性。最好的实践方式是在做一开始的制造中就渗入这种实践思想，而不是为了满足设计的表现思维。

##好处

1. 能使页面能够近可能的向后兼容及向前兼容。即使是在未来的浏览器中。
2. 结构简洁，可维护性好，扩展性好。
3. 在现今大数据的推动下，语义化和结构清晰的网页能更好地进行扩展及转换，更具可发现性。
4. 布局，排版更加精致。

##最佳实践
如何才能让页面满足标准，语义化及可用性呢？

1. 先做出页面的结构，并注意结构的主次顺序及重要性。再在结构上添加布局及表现，行为。
2. 用正确的结构化的标签来描述元素，避免无语义的标签及表现上的无用图片标签。
3. w3c验证。doctype等的正确，符合html5或其他标准的语法。
4. 添加可访问性属性及测试。

##可用性的一些细节

1. 正确的doctype,正确的字符集，正确的标准语法。
2. 逻辑性的结构，注意内容结构的次序。
3. 标签语义化。使用正确的标签。
4. 图片添加alt，并且是有意义的句子描述，而不是随意性的单词。表现类图片放在css背景中。运用图片替换技术。
5. 超链接及表单添加title.
6. 颜色：如果用颜色传达信息，最好使用一些其他的强调方法，比如下划线等。
7. 测试语义化与结构：无样式表 无脚本时是否还具有逻辑化。
8. 表单加label标签
9. 提供键盘的访问方法：accesskey及tabindex属性

对于脚本：
渐进增强，添加`<noscript>`及无干扰的脚本设计
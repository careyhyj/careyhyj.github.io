---
layout: page
title: About
description: 心中有码
keywords: Carey Huang, 欢乐马儿
comments: true
menu: 关于
permalink: /about/
---

对代码有研究的测试工程师一枚

相信「技术能够改变世界」

## 联系

{% for website in site.data.social %}
* {{ website.sitename }}：[@{{ website.name }}]({{ website.url }})
{% endfor %}

## Skill Keywords

{% for category in site.data.skills %}
### {{ category.name }}
<div class="btn-inline">
{% for keyword in category.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}

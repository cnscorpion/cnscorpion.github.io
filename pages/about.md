---
layout: page
title: About
description: D66分享网
keywords: d66
comments: true
menu: 关于
permalink: /about/
---

欢迎来到D66分享站，你的网络奇趣之旅！在这里，我们精选分享各类趣站、网络技术、好用软件等精彩资源，助你畅游互联网的海洋。发现新奇，了解技术，体验便捷，D66.cn陪你一起探索无尽的网络世界。立即加入我们，掌握最新潮的网络资讯，畅享数字时代的精彩旅程！

## 联系

<ul>
{% for website in site.data.social %}
<li>{{website.sitename }}：<a href="{{ website.url }}" target="_blank">@{{ website.name }}</a></li>
{% endfor %}
{% if site.url contains 'mazhuang.org' %}
<li>
微信公众号：<br />
<img style="height:192px;width:192px;border:1px solid lightgrey;" src="{{ site.url }}/assets/images/qrcode.jpg" alt="闷骚的程序员" />
</li>
{% endif %}
</ul>


## Skill Keywords

{% for skill in site.data.skills %}
### {{ skill.name }}
<div class="btn-inline">
{% for keyword in skill.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}

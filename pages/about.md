---
layout: page
title: About
description: 개발자 이명훈입니다.
keywords: Devhun, 명훈
comments: false
menu: About
permalink: /about/
---

계획을 세우고 이를 따라가는 것을 좋아하며,

조용한 집중력으로 세세한 부분까지 신경 쓰는 것을 즐깁니다.

## Contact

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

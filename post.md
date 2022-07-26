---
layout: page
permalink: /post.html
title: 블로그 포스트
image: assets/images/night_sky.jpg
---

<ul>
<hr>
{% for post in site.posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title }} <div style="float: right; font-size:70%">{{ post.last_modified_at }}</div></a>
    <hr>
  </li>
{% endfor %}
</ul>

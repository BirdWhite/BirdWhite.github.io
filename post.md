---
layout: page
permalink: /post
title: 블로그 포스트
image: assets/images/night_sky.jpg
---

<table>
  <tbody>
{% for post in site.posts %}
  <tr>
    <td style="width: 25%; vertical-align: middle">
      {% if post.image %}
        <span class="image fit">
          <a href="{{ post.url }}">
            <img src="{{ post.image | absolute_url }}" alt="" />
          </a>
        </span>
      {% else %}
        <a href="{{ post.url }}">
          <span class="image fit">
            <img src="{{ 'assets/images/circuit.jpg' | absolute_url }}" alt="" />
          </span>
        </a>
      {% endif %}
    </td>

    <td style="vertical-align:middle">
      <a href="{{ post.url }}">
        <h2>{{ post.title }}</h2>
        <h4 style="font-weight: normal">{{ post.subtitle }}</h4>
      </a>
    </td>

    <td style="vertical-align: bottom">
      <a href="{{ post.url }}">
        <h2><div style="float: right; font-size:50%">{{ post.last_modified_at }}</div></h2>
      </a>
    </td>
  </tr>
{% endfor %}
  </tbody>
</table>

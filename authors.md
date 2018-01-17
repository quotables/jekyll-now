---
layout: page2
title: "by author"
---

{% capture tags %}
  {% for tag in site.tags %}
    {{ tag[0] }}
  {% endfor %}
{% endcapture %}
{% assign sortedtags = tags | split:' ' | sort %}

{% for tag in sortedtags %}
<ul>
  <li><a href="#{{tag}}"> {{ tag }}</a></li>
</ul>
{% endfor %}
<br><br><br>

{% for tag in sortedtags %}
  <h1 id="{{ tag }}">{{ tag }}</h1>
  {% for post in site.tags[tag] %}

<article class="post2">
{{ post.content }}
<hr><a href="{{post.url}}">Added to diary {{ post.date | date_to_long_string }}</a>
</article>

{% endfor %}
{% endfor %}
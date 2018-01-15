---
layout: page2
title: ""
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
<h4>Added {{ post.date | date_to_long_string }}</h4>
{{ post.content }}
<hr><br><br><br>

{% endfor %}
<br><br><br><br><br><br><br><br><br>
{% endfor %}
---
layout: page2
title: "by date"
---


<!-- //first time -->
{% for post in site.posts  %}
{% capture this_year %}{{ post.date | date: "%Y" }}{% endcapture %}
{% capture this_month %}{{ post.date | date: "%B" }}{% endcapture %}
{% capture next_year %}{{ post.previous.date | date: "%Y" }}{% endcapture %}
{% capture next_month %}{{ post.previous.date | date: "%B" }}{% endcapture %}

{% if forloop.first %}
<ul>
<li><h2><a href="#{{ this_year }}-ref">{{this_year}}</a></h2></li>
<ul>
<li><h3><a href="#{{ this_year }}-{{ this_month }}-ref">{{ this_month }}</a></h3></li>
</ul>
</ul>

{% endif %}

<!-- <article class="post2">
{{ post.content }} <hr><a href="{{post.url}}">Added to diary {{ post.date | date_to_long_string }}</a></article> -->

{% if forloop.last %}

{% else %}
    {% if this_year != next_year %}
    <ul>
    <li><h2><a href="#{{ next_year }}-ref">{{next_year}}</a></h2><li>
    <ul>
        <li><h3><a href="#{{ next_year }}-{{ next_month }}-ref">{{ next_month }}</a></h3></li>
        </ul>
    <ul>
    {% else %}    
        {% if this_month != next_month %}
<ul><ul>
<li><h3><a href="#{{ this_year }}-{{ next_month }}-ref">{{ next_month }}</a></h3></li>
</ul></ul>
        {% endif %}
    {% endif %}
{% endif %}
{% endfor %}






<br>
<br>
<br>
<br>


<!-- //second time -->
{% for post in site.posts  %}
{% capture this_year %}{{ post.date | date: "%Y" }}{% endcapture %}
{% capture this_month %}{{ post.date | date: "%B" }}{% endcapture %}
{% capture next_year %}{{ post.previous.date | date: "%Y" }}{% endcapture %}
{% capture next_month %}{{ post.previous.date | date: "%B" }}{% endcapture %}

{% if forloop.first %}
<h2 id="{{ this_year }}-ref">{{this_year}}</h2>
<h3 id="{{ this_year }}-{{ this_month }}-ref">{{ this_month }}</h3>

{% endif %}

<article class="post2">
{{ post.content }} <hr><a href="{{post.url}}">Added to diary {{ post.date | date_to_long_string }}</a></article>

{% if forloop.last %}

{% else %}
    {% if this_year != next_year %}
    <h2 id="{{ next_year }}-ref">{{next_year}}</h2>
    <h3 id="{{ next_year }}-{{ next_month }}-ref">{{ next_month }}</h3>
    {% else %}    
        {% if this_month != next_month %}
<h3 id="{{ this_year }}-{{ next_month }}-ref">{{ next_month }}</h3>
        {% endif %}
    {% endif %}
{% endif %}
{% endfor %}
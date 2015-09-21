---
layout: page
title: Topics
description: Topics list from the blog
permalink: /tags/
---

<!-- https://blog.brandonparsons.me/2015-using-tags-in-a-jekyll-blog-on-github-pages/ -->
<!-- This is pasted verbatim, with two exceptions:
1) I removed all the styling classes 
2) Slight copy editing -->

{% assign tags_list = site.tags %}

<ul>
  {% if tags_list.first[0] == null %}
    {% for tag in tags_list %}
      <li>
        <a href="/tags#{{ tag | slugify }}-ref" >{{ tag | capitalize }}</a>
        <span>{{ site.tags[tag].size }}</span>
      </li>
    {% endfor %}
  {% else %}
    {% for tag in tags_list %}
      <li>
        <a href="/tags#{{ tag[0] | slugify }}-ref" >{{ tag[0] | capitalize }}</a>
        (<span>{{ tag[1].size }}</span>)
      </li>
    {% endfor %}
  {% endif %}
</ul>
{% assign tags_list = nil %}

<hr />

<h2>Relevant posts by topic</h2>

{% for tag in site.tags %}
  <h2 id="{{ tag[0] | slugify }}-ref">{{ tag[0] | capitalize }}</h2>
  <ul>
    {% assign pages_list = tag[1] %}

    {% for node in pages_list %}
      {% if node.title != null %}
        {% if group == null or group == node.group %}
          {% if page.url == node.url %}
          <li class="active"><a href="{{node.url}}" class="active">{{node.title}}</a></li>
          {% else %}
          <li><a href="{{node.url}}">{{node.title}}</a></li>
          {% endif %}
        {% endif %}
      {% endif %}
    {% endfor %}

    {% assign pages_list = nil %}
    {% assign group = nil %}
  </ul>
  {% endfor %}
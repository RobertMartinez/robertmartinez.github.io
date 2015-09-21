---
layout: page
title: Tags
description: Tag list from the blog
permalink: /tags/
---

<!-- https://blog.brandonparsons.me/2015-using-tags-in-a-jekyll-blog-on-github-pages/ -->
<!-- This is pasted verbatim, with the one exception that I removed all the styling classes -->

{% assign tags_list = site.tags %}

<h2>Tag List</h2>
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
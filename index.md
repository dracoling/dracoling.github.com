---
layout: page
title: "Index"
description: ""
---
{% include JB/setup %}

I suppose this should really be some kind of introduction to the site, but I don't feel like
doing that kind of thing right now.

Here's a list of crap published here.

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

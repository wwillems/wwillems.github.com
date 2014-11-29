---
layout: page
title: Coding
tagline: memorabilia
---
{% include JB/setup %}

  
## Latest Posts

This blog is a fine collection of various tech related posts.

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>


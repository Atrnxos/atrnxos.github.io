---
layout: default
title: 博客
nav_order: 4
has_children: true
---

# 博客

这里是所有博客文章的列表。

{% for post in site.posts %}
## [{{ post.title }}]({{ post.url }})
{{ post.date | date: "%Y年%m月%d日" }}

{{ post.excerpt | strip_html | truncate: 200 }}
{% endfor %}
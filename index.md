---
layout: index
title: It works
---
# 终于学会做网站了，哈哈哈哈哈

# Blog
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

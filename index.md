---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: index
title: Home
---

<h2>日志</h2>
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>  
      {% for tag in post.tags %}
        <code class="highlighter-rouge">{{tag}}</code>
      {% endfor %}
    </li>
  {% endfor %}
</ul>

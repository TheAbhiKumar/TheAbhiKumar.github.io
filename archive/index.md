---
layout: postnew
title: archive
<!-- in-nav: true -->
weight: 2
---

<ul id="archive">
  {% for post in site.posts %}
  <li>
    <span class="post-date">
    <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: '%d %b<span class="year"> %Y</span>' }}</time>
    </span>
  <div class="description"><a href="{{ post.url }}">{{ post.title }}</a></div>
  </li>
{% endfor %}
</ul>
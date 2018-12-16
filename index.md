---
layout: home
title: about
header_title: Abhishek Kumar's homepage
---

## Posts

  {% assign posts = site.posts | where:"type", "posts" %}

  <ul id="archive">
    {% for post in posts %}
    {% if post.hidden != true %}
    <li>
      <a href="{{ post.url }}">
      <div class="post-list">
        <div class="post-name">{{ post.title }}</div>
        <div class="post-time">{{ post.date | date: '%Y.%m.%d' }}</div>
      </div>
      </a>
    </li>
    {% endif %}
    {% endfor %}
  </ul>

## Links

[GitHub][link_github] &nbsp;/&nbsp;
abhishek at abkumar dot me

[link_github]: http://www.github.com/TheAbhiKumar/

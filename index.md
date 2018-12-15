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
      <span class="post-date">{{ post.date | date: '%d %b %Y' }} &raquo;</span>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
    {% endif %}
    {% endfor %}
  </ul>

## Links

[GitHub][link_github] &nbsp;/&nbsp;
abhishek at abkumar dot me

[link_github]: http://www.github.com/TheAbhiKumar/

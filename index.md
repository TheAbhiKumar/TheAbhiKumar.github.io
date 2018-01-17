---
layout: home
title: about
header_title: Abhishek Kumar's homepage
---

## About

I am an undergraduate student at UC San Diego studying computer science. My current research interests are natural language understanding and reinforcement learning.

<!-- [CV][link_cv] &nbsp;/&nbsp; -->
[Blog][link_blog] &nbsp;/&nbsp;
[GitHub][link_github] &nbsp;/&nbsp;
<!-- [Style Guide][link_styleguide] &nbsp;/&nbsp; -->
<!-- [Google Scholar][link_scholar] &nbsp;/&nbsp; -->
abkumar at ucsd dot edu

[link_cv]: cv/
[link_blog]: blog/
[link_styleguide]: styleguide/
[link_github]: http://www.github.com/TheAbhiKumar/
[link_scholar]: https://scholar.google.com/citations?hl=en&amp;user=1xw2vTsAAAAJ

## Research

<ul id="pubs">
{% for paper in site.data.pubs %}
  <li id="paper">
    <strong>{{ paper.title }}</strong>
    <br />
    {{ paper.authors }}
    <br />
    {% if paper.conf != defined %} {{ paper.conf }} <br /> {% endif %}
    <a href="https://arxiv.org/abs/{{ paper.arxiv }}">ArXiv</a>
    {% if paper.code != defined %} / <a href="{{ paper.code }}">Code</a> {% endif %}
    {% if paper.blog != defined %} / <a href="{{ paper.blog }}">Blog</a> {% endif %}
    {% if paper.video != defined %} / <a href="{{ paper.video }}">Video</a> {% endif %}
    <br />
  </li>
{% endfor %}
</ul>

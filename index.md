---
layout: postnew
title: about
header_title: Abhishek Kumar's homepage
---

Hi, I'm **Abhishek Kumar**. I'm an undergraduate student at UC San Diego studying computer science. I am interested in recurrent neural networks and reinforcement learning problems. I am on [Github][github] and [Twitter][twitter]. [Email me][email] if you want to get in touch.

[github]: https://github.com/TheAbhiKumar
[twitter]: https://twitter.com/_abkumar
[email]: &#109;&#097;&#105;&#108;&#116;&#111;:&#097;&#098;&#107;&#117;&#109;&#097;&#114;&#064;&#117;&#099;&#115;&#100;&#046;&#101;&#100;&#117;

## Latest Blog Post
{% for post in site.categories.blog limit:1 %}
  <ul id="archive">
    <li>
      <span class="post-date">
      <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: '%d %b<span class="year"> %Y</span>' }}</time>
      </span>
    <div class="description">
      <a href="{{ post.url }}">{{ post.title }}</a>
      <p class="excerpt">{{ post.excerpt }}</p>
    </div>
    </li>
  </ul>
{% endfor %}

---
layout: page
title: About
---
 
<p class="gamma promo"><mark>This site is still under development.</mark></p>

My [Github](https://github.com/TheAbhiKumar).

<!-- I'm an undergraduate computer science major at /*/. I like to code my [projects](/projects) in C++ and open source them on [Github](https://github.com/TheAbhiKumar). I enjoy competing in [hackathons](/hackathons) and [writing](/blog) about programming.

If you have questions or feedback, you can tweet me [@](https://twitter.com/) or email me at [example@gmail.com](mailto:example@gmail.com). -->

<div class="grid"> 
    <section class="small grid__col grid__col--3-of-6">
        <h2 class="latest">Latest Blog Post</h2>
        <ul class="unl posts__list">
        {% for post in site.posts %}
            {% if post.recent == true %}
          <li class="o--p">
            <a class="a--plain" href="{{ post.url }}">
              <span class="o--b beta o--z">{{ post.title }}</span>
              <span class="meta delta o--b">{{ post.date | pretty }}</span>
            </a>
          </li>
          {% endif %}
        {% endfor %}
        </ul>
    </section>

    <section class="small grid__col grid__col--3-of-6">
        <h2 class="latest">Featured Project</h2>
        <ul class="unl posts__list">
        {% for post in site.posts %}
            {% if post.categories contains 'projects'%}
                {% if post.feature == yes %}
          <li class="o--p">
            <a class="a--plain" href="{{ post.url }}">
              <span class="o--b beta o--z">{{ post.title }}</span>
              <span class="meta delta o--b">{{ post.language }}</span>
            </a>
          </li>
                {% endif %}
          {% endif %}
        {% endfor %}
        </ul>
    </section>
</div>

---
layout: page
title: About
---

<!-- Hey, I'm Abhishek Kumar, an undergraduate computer science major at the University of California, San Diego. I write about programming here and showcase my personal projects which can be found on [Github](https://github.com/TheAbhiKumar). -->

<div class="grid">
    <!-- <section class="small grid__col grid__col--3-of-6"> -->
    <!-- <section class="small grid__col grid__col--6-of-6"> -->
  <!-- <section class="grid__col  grid__col--2-of-6"> -->
  <!-- </section>     -->
    <!-- <section class="grid__col  grid__col--2-of-6"> -->
    <section class="grid__col">
        <h2 class="latest">Latest Blog Post</h2>
        <ul class="unl posts__list">
        {% for post in site.posts %}
            {% if post.recent == true %}
          <li class="o--p">
            <a class="a--plain" href="{{ post.url }}">
              <span class="o--b beta o--z">{{ post.title }}</span>
              <!-- <span class="meta delta o--b">{{ post.date | pretty }}</span> -->
              <span class="meta delta o--b">{{ post.date | date_to_string }}</span> 
            </a>
          </li>
          {% endif %}
        {% endfor %}
        </ul>
    </section>

  <!-- <section class="grid__col  grid__col--2-of-6"> -->
  <!-- </section>   -->
<!--     <section class="small grid__col grid__col--3-of-6">
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
    </section> -->
</div>

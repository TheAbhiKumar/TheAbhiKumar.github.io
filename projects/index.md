---
layout: page
title: Projects
in-nav: true
---

<p class="gamma promo"><mark>This site is still under development.</mark></p>

* * *

## Tempus Porttitor
[Nulla vitae]() elit libero, a pharetra augue. Maecenas sed diam eget risus varius blandit sit amet non magna. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Curabitur blandit tempus porttitor. Nullam quis risus eget urna mollis ornare vel eu leo. Donec id elit non mi porta gravida at eget metus. [Visit the site]()

## Quis Risus
[Cras mattis]() consectetur purus sit amet fermentum. Morbi leo risus, porta ac consectetur ac, vestibulum at eros. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed posuere consectetur est at lobortis. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. [Visit the Site]()

<section class="small grid__col grid__col--3-of-6">
        <h2 class="latest">Latest Project</h2>
        <ul class="unl posts__list">
        {% for post in site.posts %}
            {% if post.categories contains 'projects' %}
          <li class="o--p">
            <a class="a--plain" href="{{ post.url }}">
              <span class="o--b beta o--z">{{ post.title }}</span>
              <span class="meta delta o--b">{{ post.language }}</span>
            </a>
          </li>
          {% endif %}
        {% endfor %}
        </ul>
    </section>
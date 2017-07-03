---
layout: postnew
title: about
header_title: Abhishek Kumar's homepage
---

<!--   <table width="800" border="0" align="center" cellspacing="0" cellpadding="0">
    <tbody><tr>
    <td>
      <table width="100%" align="center" border="0" cellspacing="0" cellpadding="20">
      <tbody><tr>
        <td width="67%" valign="middle">
        <p align="center">
        <name>Chelsea Finn</name><br>
        cbfinn at eecs dot berkeley dot edu
        </p>
        <p>I am a PhD student in CS at <a href="https://eecs.berkeley.edu/">UC Berkeley</a>, where I work on machine learning for robotic perception and control. I am a part
        of <a href="http://bair.berkeley.edu">Berkeley AI Research Lab (BAIR)</a>, advised by <a href="http://people.eecs.berkeley.edu/~pabbeel/">Pieter Abbeel</a> and
        <a href="https://people.eecs.berkeley.edu/~svlevine/">Sergey Levine</a>.
        I recently spent time at <a href="http://research.google.com/teams/brain/">Google Brain</a>.
        </p>
        <p>
        Before graduate school, I received a Bachelors in EECS at <a href="http://mit.edu">MIT</a>, where I worked on several research projects, including an
        assistive technology project in <a href="http://csail.mit.edu">CSAIL</a> under <a href="http://people.csail.mit.edu/teller/">Seth Teller</a> and an animal biometrics
        project under Sai Ravela. I have also spent time at <a href="https://www.counsyl.com/technology">Counsyl</a>, <a href="https://www.google.com/intl/en/about/">Google</a>,
        and <a href="http://www.sandia.gov/">Sandia National Labs</a>.
        </p>
        <p align="center">
<a href="https://people.eecs.berkeley.edu/~cbfinn/_files/cv.pdf">CV</a> &nbsp;/&nbsp;
<a href="https://scholar.google.com/citations?hl=en&amp;user=1xw2vTsAAAAJ">Google Scholar</a> &nbsp;/&nbsp;
<a href="http://www.github.com/cbfinn/"> GitHub </a>
        </p>
        </td>
        <td width="33%">
        <img src="./_files/ChelseaFinn.jpg">
        </td>
      </tr>
  </tbody></table> -->

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

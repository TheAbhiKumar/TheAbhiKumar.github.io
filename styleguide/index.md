---
layout: page
title: Style&nbsp;Guide
---

This page demonstrates the various visual styles that comprise the design of this site.<!--  At the time of writing ({{ site.time | pretty }}), heading & body copy is set in Hoefler Text A, headlines are set in Requiem Display A, and captions are set in Whitney[^1]. -->


## Heading Level Two

Second level headings are used to split text into sections. First level headings are only used once per page, in the page or post title. [Hyperlinks](/styleguide) are underlined and coloured when hovered.

- Bulleted lists look like this[^2].
- Multi-leveled bulleted lists look like this:
    - This is an example of a second-level bullet
- Another bullet.

{% include image.html url="/assets/2014/05/2.jpg" caption="Picture 2" %}

### Heading Level Three
Third level headings are most often used to denote names rather than sections, so have a lower visual priority. Headings should avoid containing or being themselves hyperlinks, but when this rule is broken, heading hyperlinks do not differ in style from the heading itself.

1. This is a numbered list.
2. Numbered lists can also have multiple levels:
	1. This is a second-level numbered list item
3. Numbered lists, like bulleted lists, are not used particularly often on this site.


Images may take one of two forms; aligned (left), or centered (relative to the text column). Captions are encouraged, but not required.

Footnotes can also be used to source sites[^3].

***

## Language, Voice, and Persona

{% highlight html %}
<p class="gamma promo"><mark>Look both ways. “You can’t just stop.”</mark></p>
{% endhighlight %}

The last words in any given paragraph or other block-level elements are (automatically separated by a non-breaking space to prevent widows.

<p class="gamma promo"><mark>Look both ways. “You can’t just stop.”</mark></p>

Here’s an example of all these dashes in use:

> When grammar-checking, one must always remember one rule—do it often and do it well. However—and I say this with caution—this rule may be broken 3–5 times a year, in recognition of national holidays.

There are two sides to every story.

[^1]: Aenean lacinia [bibendum nulla](sed consectetur). Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia [odio sem](nec elit).
[^2]: *Italic* Footnotes
[^3]: Vivamus [*sagittis lacus*](vel augue) laoreet rutrum faucibus dolor auctor.

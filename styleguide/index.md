---
layout: postnew
title: styleguide
in-nav: false
weight: 4
---

<div class="byline">
  <div class="authors">
    <a class="name" href="{{ page.link }}">{{ page.author }} [arXiv]</a>
  </div>
  <div class="tag">
    <p>{{ page.url}}</p>
  </div>
</div>

This page demonstrates in <span class="equation-mimic">O(n)</span> time the various visual styles that comprise the design of this site. Headings are set in PT Serif and body is set in Open Sans[^1]. Here is some code `std::iostream` inside a paragraph.

## Heading Level Two

Second level headings are used to split text into sections. First level headings are only used once per page, in the page or post title. [Hyperlinks](/styleguide) are underlined and coloured when hovered.

- Bulleted lists look like this[^2].
- Multi-leveled bulleted lists look like this:
    - This is an example of a second-level bullet
- Another bullet.

{% include image.html url="/assets/2014/05/2.jpg" caption="Picture 2" %}{: .center-image }

### Heading Level Three
Third level headings are most often used to denote names rather than sections, so have a lower visual priority.

1. This is a numbered list.
2. Numbered lists can also have multiple levels:
	1. This is a second-level numbered list item
3. Numbered lists, like bulleted lists, are not used particularly often on this site.

Images may take one of two forms; aligned (left), or centered (relative to the text column). Captions are encouraged, but not required.

Footnotes can also be used to source sites[^3].

***

{% include image.html url="/assets/2014/05/1.jpg" caption="Picture 1" %}{: .center-image }

Here is some _italicized text_ and some **bold text**.

### Random Crap

<!-- Comment on inputs/outputs in figure? -->
{% include image.html url="/assets/ntm/rnn_basic_rnn.svg" %}

The basic RNN design struggles with longer sequences, but a special variant -- ["long short-term memory" networks][olah2015lstm] -- can even work with these. Such models have been found to be very powerful, achieving remarkable results in many tasks including translation, voice recognition, and image captioning. As a result, recurrent neural networks have become very widespread in the last few years.

<p>H<sub>2</sub>O</p>

#### Heading Level Four

As this has happened, we’ve seen a growing number of attempts to augment RNNs with new properties. Four directions stand out as particularly exciting:

* [*Neural Turing Machines*](#neural-turing-machines) have external memory that they can read and write to.
* [*Attentional Interfaces*](#attentional-interfaces) allow RNNs to focus on parts of their input.
* [*Adaptive Computation Time*](#adaptive-computation-time) allows for varying amounts of computation per step.
* [*Neural Programmers*](#neural-programmer) can call functions, building programs as they run.

[olah2015lstm]: http://colah.github.io/posts/2015-08-Understanding-LSTMs/

<ul id="archive">
  <li>
  <span class="post-date">
  <time datetime="2016-09-01">01 Sep<span class="year"> 2016</span></time>
  </span>
  <div class="description">
    <a href="#">Title of post</a>
    <p class="excerpt">Description</p>
  </div>
  </li>
</ul>

<div class="byline">
        <div class="author">
          <a class="name" href="https://arxiv.org/abs/1511.04834">Neelakantan, et al., 2015 [arXiv]</a>
        </div>
        <div class="date">
          <div class="month">January 22, 2016</div>
        </div>
      </div>
      
### Random crap ending

## Language, Voice, and Persona

{% highlight cpp %}
template <typename T>
var<T> activation<T>::hard_sigmoid(const var<T>& input) {
  auto output = var<T>::zeros_like(input);
  const T* input_data = input.cpu_data();
  T* output_data = output.mutable_cpu_data();
  for (int i = 0; i < output.count(); i++) {
    output_data[i] = std::max(0.0, std::min(1.0, 0.2*input_data[i] + 0.5));
  }
  return output;
}
{% endhighlight %}

{% highlight python %}
def sample(h, seed_ix, n):
  """ 
  sample a sequence of integers from the model 
  h is memory state, seed_ix is seed letter for first time step
  """
  x = np.zeros((vocab_size, 1))
  x[seed_ix] = 1
  ixes = []
  for t in xrange(n):
    h = np.tanh(np.dot(Wxh, x) + np.dot(Whh, h) + bh)
    y = np.dot(Why, h) + by
    p = np.exp(y) / np.sum(np.exp(y))
    ix = np.random.choice(range(vocab_size), p=p.ravel())
    x = np.zeros((vocab_size, 1))
    x[ix] = 1
    ixes.append(ix)
  return ixes
{% endhighlight %}

The last words in any given paragraph or other block-level elements are (automatically separated by a non-breaking space to prevent widows.

Here’s an example of all these dashes in use:

> When grammar-checking, one must always remember one rule—do it often and do it well. However—and I say this with caution—this rule may be broken 3–5 times a year, in recognition of national holidays.

There are two sides to every story.

<!-- Appendix -->
[^1]: [PT Serif/Open Sans](https://fonts.google.com/specimen/PT+Serif)
[^2]: *Italic* Footnotes
[^3]: Vivamus [*sagittis lacus*](vel augue) laoreet rutrum faucibus dolor auctor.

## Footnotes

* footnotes will be placed here
{:footnotes}

<!-- Appendix -->
<section class="appendix">
  <h3>Errors, Reuse, and Citation</h3>
  <p>If you see mistakes or want to suggest changes, please open an issue or submit a pull request on <a href="https://github.com/TheAbhiKumar/TheAbhiKumar.github.io">github</a>.</p>
  <h3>References</h3>
  <ul class="references">
    <li>Alemi, A. A., Chollet, F., Irving, G., Szegedy, C., & Urban, J. (2016). DeepMath-Deep Sequence Models for Premise Selection. arXiv preprint arXiv:1606.04442.</li>
    <li>Andrychowicz, M., & Kurach, K. (2016). Learning Efficient Algorithms with Hierarchical Attentive Memory. arXiv preprint arXiv:1602.03218.</li>
  </ul>
</section>
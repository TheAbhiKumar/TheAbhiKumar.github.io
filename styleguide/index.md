---
layout: postnew
title: Style Guide
in-nav: false
weight: 4
---


This page exists to demonstrate the visual styles of the various elements that comprise the design of this site. Headings are set in PT Serif and body is set in Open Sans[^1]. 

## Heading Level Two

Second level headings are used to split text into sections. First level headings are only used once per page, in the page or post title. [Hyperlinks](/styleguide) are underlined and coloured when hovered.

- Bulleted lists look like this.
- Multi-leveled bulleted lists look like this:
    - This is an example of a second-level bullet
- Lists tend not to be used very often on this site, but they exist nonetheless.

### Heading Level Three

Third level headings are most often used to denote names rather than sections, so have a lower visual priority. Headings should avoid containing or being themselves hyperlinks, but when this rule is broken, heading hyperlinks do not differ in style from the heading itself.

1. This is a numbered list.
2. Numbered lists can also have multiple levels:
  1. This is a second-level numbered list item
3. Numbered lists, like bulleted lists, are not used particularly often on this site.

<!-- {% include image.html alt="" url="https://placeimg.com/1000/300/arch" caption="This is an example image caption." %} -->
{% include image.html url="/assets/rnn.png" caption="This is an example image caption." %}

<!-- {% include image.html url="/assets/lstm.png" caption="This is an example image caption." %}{: .center-image } -->

Images are centered and captions are encouraged, but not required. Images are currently used only sparingly, but must flow with the content. Captions should be readable, but not distract from the main article. Like images themselves, they are supplements.

Horizontal rules should be used to separate content into sections, or draw a rule before adding editorial notes and footnotes.

***

## Styling

All paragraphs are justified and text can be _italicized_ and **bolded**. Footnotes can also be used as references [^2]. Subscripts and superscripts can also be used H<sub>2</sub>O. Pseudo math is typeset with italicized Georgia to mimic equations like <span class="equation-mimic">O(n)</span> and <span class="equation-mimic">Q* (s,a) = max E[Σ γr | s, a, π]</span>. Short pieces of code have an inline style `import skynet as sn` inside a paragraph [^3].

{% highlight python %}
# Actor critic model
class Actor:
    def __init__(self, sess, env, default_hparams):
        self.sess = sess
        self.env = env
        self.ARGS = default_hparams
        self.actor_lr = self.ARGS.actor_lr
        self.tau = self.ARGS.tau
        self.batch_size = self.ARGS.batch_size

        self.state_dim = env.observation_space.shape[0]
        self.action_dim = env.action_space.shape[0]
        self.action_bound = env.action_space.high
        # Action space should be symmetric
        assert (env.action_space.high == -env.action_space.low)
        with tf.variable_scope(f'Actor'):
            self.a, _, self.c = self.create_network()
            self.ta, _, self.tc = self.create_network(scope='target')

        self.normal_params = tf.trainable_variables(scope='Actor/normal_actor')
        self.target_params = tf.trainable_variables(scope='Actor/target_actor')

        self.update_target_net = [
            self.target_params[i].assign(
                tf.multiply(self.normal_params[i], self.tau) + \
                tf.multiply(self.target_params[i], 1.0 - self.tau)
            ) for i in range(len(self.target_params))
        ]

        self.sampled_gradient = tf.placeholder(tf.float32, shape=[None, self.action_dim], name='sampled_gradient')
        self.unnormalized_actor_gradients = tf.gradients(self.c, self.normal_params, -self.sampled_gradient)
        self.actor_gradients = list(map(lambda x: tf.div(x, self.batch_size), self.unnormalized_actor_gradients))
        self.optimize = tf.train.AdamOptimizer(self.actor_lr).apply_gradients(zip(self.actor_gradients, self.normal_params))
{% endhighlight %}

Inline code blocks can also be used for longer pieces of code.

> "Blockquotes are used to frame non-original and secondary quotes that run longer than a single line."

The visual style guide of this site is outlined above. It would only be fair to create a writing style guide. These guidelines are just that—guidelines—and may be broken where appropriate. They are a mix of my upbringing, lessons learned from doing things the wrong way, and a few resources—notably [The Elements of Typographic Style][typograhic_style], [The Chicago Manual of Style][chicago_manual], and [The Elements of Style][elements_style]. Happy writing.

[typograhic_style]: https://amazon.com/gp/product/0881792128/
[chicago_manual]: https://amazon.com/gp/product/0226104206/
[elements_style]: https://amazon.com/gp/product/0143112724/

<!-- Appendix -->
[^1]: [PT Serif/Open Sans](https://fonts.google.com/specimen/PT+Serif)
[^2]: Alemi, A. A., Chollet, F., Irving, G., Szegedy, C., & Urban, J. (2016). DeepMath-Deep Sequence Models for Premise Selection. arXiv preprint arXiv:1606.04442.
[^3]: Andrychowicz, M., & Kurach, K. (2016). Learning Efficient Algorithms with Hierarchical Attentive Memory. arXiv preprint arXiv:1602.03218.

***

## Footnotes/References

* footnotes will be placed here
{:footnotes}

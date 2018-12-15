---
layout: post
title: Variational Inference
category: blog
math: true
hidden: true
---

> This post is a work in progress

At ICLR 2016 there were a couple of papers on neural programmers. The architecture of these networks introduce with it many benefits. They have complex operations and have combinations of these operations while being able to successfully generalize over unknown input ranges. Both of these networks outperform sequence to sequence models in many tasks, particularly because of their ability to generalize well.

The first, the Neural Programmer ([Neelakantan, *et al.*, 2015])[^1], is one approach to this. The other, the Neural Programmer-Interpreter ([Reed & de Freitas, 2015])[^2], which won best paper at ICLR 2016, can accomplish a number of very interesting tasks, but requires supervision in the form of correct programs.

---

[Neelakantan, *et al.*, 2015]: http://arxiv.org/abs/1511.04834
[Reed & de Freitas, 2015]: https://arxiv.org/abs/1511.06279

<!-- Appendix -->
[^1]: Neelakantan, A., Le, Q. V., & Sutskever, I. (2015). Neural programmer: Inducing latent programs with gradient descent. [arXiv preprint arXiv:1511.04834][Neelakantan, *et al.*, 2015].
[^2]: Reed, S., & de Freitas, N. (2015). Neural programmer-interpreters. [arXiv preprint arXiv:1511.06279][Reed & de Freitas, 2015].

## Footnotes/References

* footnotes will be placed here
{:footnotes}

---
layout: post
title: A List of Reinforcement Learning Derivations
category: blog
excerpt: A List of Reinforcement Learning Derivations
math: true
hidden: true
---

### Log derivative trick

$$
\nabla_\theta \log p(x;\theta) = \frac{\nabla_\theta p(x;\theta)}{p(x;\theta)}
$$

$$
\begin{aligned}
\mathbb{E}_{p(x;\theta)}[\nabla_\theta \log p(x;\theta)] &= \mathbb{E} \left[ \frac{\nabla_\theta p(x;\theta)}{p(x;\theta)} \right] \\
&= \int p(x;\theta) \frac{\nabla_\theta p(x;\theta)}{p(x;\theta)} dx \\
&= \nabla_\theta \int p(x;\theta)dx = \nabla_\theta 1 = 0
\end{aligned}
$$
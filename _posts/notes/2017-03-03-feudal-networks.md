---
layout: post
title: FeUdal Networks for Hierarchical Reinforcement Learning
category: blog
---

> We introduce FeUdal Networks (FuNs): a novel architecture for hierarchical reinforcement learning. Our approach is inspired by the feudal reinforcement learning proposal of Dayan and Hinton, and gains power and efficacy by decoupling end-to-end learning across multiple levels -- allowing it to utilise different resolutions of time. Our framework employs a Manager module and a Worker module. The Manager operates at a lower temporal resolution and sets abstract goals which are conveyed to and enacted by the Worker. The Worker generates primitive actions at every tick of the environment. The decoupled structure of FuN conveys several benefits -- in addition to facilitating very long timescale credit assignment it also encourages the emergence of sub-policies associated with different goals set by the Manager. These properties allow FuN to dramatically outperform a strong baseline agent on tasks that involve long-term credit assignment or memorisation. We demonstrate the performance of our proposed system on a range of tasks from the ATARI suite and also from a 3D DeepMind Lab environment.

[https://arxiv.org/abs/1703.01161](https://arxiv.org/abs/1703.01161)

## What?
A framework in which a high level manager sets abstract goals for the worker which generates primitive actions in the environment.

## Why?
This decoupled structure aids in facilitating long timescale credit assignment and also encourages the emergence of sub policies associated with different goals set by the manager.

One of the issues with options is that they typically degenerate into one of two trivial solutions
1. only one active option that solves the whole task
2. a policy over options that changes options at every step

FeUdal Networks differ in that the top level produces a meaningful and explicit goal for the bottom level to achieve.

## How?

They proposed a novel approximate transition policy gradient update for training the manger.

## Model

The architecture is a fully differentiable network consisting of two modules, the worker and the manager. Gradients are not propagated between the worker and manager. Both the manager and worker are recurrent.

The manager takes a latent state representation as input and outputs a goal vector.
It receives its learning signal from the environment alone.

The worker produces actions conditioned on external observation, its own state, and the manager's goal.

## Evaluation
## But
## Comments
## Questions
## Resources
## References

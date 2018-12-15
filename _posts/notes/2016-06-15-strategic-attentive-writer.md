---
layout: post
title: Strategic Attentive Writer for Learning Macro-Actions
category: blog
---

> Abstract: We present a novel deep recurrent neural network architecture that learns to build implicit plans in an end-to-end manner by purely interacting with an environment in reinforcement learning setting. The network builds an internal plan, which is continuously updated upon observation of the next input from the environment. It can also partition this internal representation into contiguous sub- sequences by learning for how long the plan can be committed to - i.e. followed without re-planing. Combining these properties, the proposed model, dubbed STRategic Attentive Writer (STRAW) can learn high-level, temporally abstracted macro- actions of varying lengths that are solely learnt from data without any prior information. These macro-actions enable both structured exploration and economic computation. We experimentally demonstrate that STRAW delivers strong improvements on several ATARI games by employing temporally extended planning strategies (e.g. Ms. Pacman and Frostbite). It is at the same time a general algorithm that can be applied on any sequence data. To that end, we also show that when trained on text prediction task, STRAW naturally predicts frequent n-grams (instead of macro-actions), demonstrating the generality of the approach.

[https://arxiv.org/abs/1606.04695](https://arxiv.org/abs/1606.04695)

## What?

Proposes a new architecture that can learn macro-actions in a reinforcement learning setting and maintain a multi-step action plan.

## Why?

Hypothetically, agents can discover useful macro-actions on their own should be capable of more efficient exploration.

## How?

One of the way they encourage exploration is to introduce a noisy communication channel between the feature extract (CNN) and the planning module. The architecture allows for multiple outputs to be generated if a single observation is informative enough.

### Benefits
1. Facilitates structured exploration since the network learns meaningful action pattern to make longer exploratory steps.
2. Computationally efficient since it doesn't need to process observations while it is committed to a multi step action plan

## Model

A deep recurrent neural network with two modules
1. Translates environment observations into an action-plan
	- Follows action-plan for multiple steps without updating
2. Maintains commitment-plan, determines at which step the network terminates a macro-action and updates the action-plan

Plans are updated using the attentive writing technique (DRAW)

## Evaluation

Evaluated on Atari and on a text prediction task

## But
- Only works on discrete action spaces

## Comments
## Questions
- If the agent commits to a plan in an unseen environment that gets it "stuck" can it get out?
- How would experience replay work with a technique like this since not each observation is evaluated?

## Resources
## References

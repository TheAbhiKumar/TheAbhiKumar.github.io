---
layout: post
title: "Deep Dyna-Q: Integrating Planning for Task-Completion Dialogue Policy Learning"
category: blog
---

> Training a task-completion dialogue agent via reinforcement learning (RL) is costly because it requires many interactions with real users. One common alternative is to use a user simulator. However, a user simulator usually lacks the language complexity of human interlocutors and the biases in its design may tend to degrade the agent. To address these issues, we present Deep Dyna-Q, which to our knowledge is the first deep RL framework that integrates planning for task-completion dialogue policy learning. We incorporate into the dialogue agent a model of the environment, referred to as the world model, to mimic real user response and generate simulated experience. During dialogue policy learning, the world model is constantly updated with real user experience to approach real user behavior, and in turn, the dialogue agent is optimized using both real experience and simulated experience. The effectiveness of our approach is demonstrated on a movie-ticket booking task in both simulated and human-in-the-loop settings.

[https://arxiv.org/abs/1801.06176](https://arxiv.org/abs/1801.06176)

## What?
A deep RL framework that integrates planning by incorporating a model of the environment for task-completion dialogue policy learning allowing the for the agent to be optimized using real and simulated experience.

## Why?
Training a task-completion dialogue agent is hard for two many reasons.
If the environment is used are real users than training the policy online from scratch becomes expensive.
User simulators on the other hand lack conversational complexity and are affected by the biases of its design.

## How?
## Model
## Evaluation
## But
## Comments
## Questions
## Resources
## References
* [github](https://github.com/MiuLab/DDQ)
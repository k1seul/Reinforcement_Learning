# Reinforcement Learning
### Study Notes of Hanseul Kim about Reinforcement Learning: An Introduction by Richard S. Sutton and Andrew G. Barto

## Abstract

Since the age of [Alpha Go](https://deepmind.google/research/breakthroughs/alphago/), Reinforcement Learning(**RL**) was popularized with application to diverse learning system such as Reinforcement Learning from Human Feedback([RLHF](https://huggingface.co/blog/rlhf)) to real world robots and finace application. These Deep Reinforcement Learning application heavly rely on robust [functional approximation](https://arxiv.org/abs/1610.04161) of deep neural network and learning capability using larger, [scalable models](https://huggingface.co/docs/transformers/main/performance) and huge amounts of dataset for generalization. However, to make a true generalist intelligent agent with human-like inference capability, data and computational efficient learning/planning algorithms must be well studied. This page is dedicated for deeper understanding of baseline RL algoirthms using "*Reinforcement Learning: An Introduction*" by Richard S. Sutton and Andrew G. Barto.

## Introduction

Reinforcement Learning is interdisciplinary study of optimal control and machine learning designing a intelligent agent capable of take actions in a dynamical environment to maximize cumulative reward. To design and understand such intelligent agent, [a framework by David Marr](https://www.albany.edu/~ron/papers/marrlevl.html) can be used to see each component of intelligent information processing agent.

* **Marr's Three levels of Analysis**
  * Computational theory: What is the goal of the computiation, why is it appropriate, and what is the logic of strategy by which it can be carried out? [1] 
  * Representation and algorithm: How can this computational theory be implemented? In particular, what is the representation for the input and output, and what is the algorithm for the transformation? [1]
  * Hardware implementation: How can the representation and algorithm be realized physically? [Marr (1982), p. 25] [1]


For example, we can view the current reinforcement learning research based on following aspects. 1) The goal of a reinforcement learning agent is to maximize single scalar reward by optimizing it's policy $\pi(a|s)$. It does not compute the reasons and implication of doing such action which might lead to [risk taking hazardous actions](https://www.rand.org/pubs/research_reports/RRA1473-1.html) and [complicated sim to real transfer](https://arxiv.org/abs/2009.13303). To resolve these limitations research on [Risk-Averse RL](https://arxiv.org/abs/2205.05138) or [robotic RL reward design](https://arxiv.org/abs/2404.19173) is being done. 
 








---


1. [Marr's Three Levels: A Re-evaluation](https://www.albany.edu/~ron/papers/marrlevl.html)

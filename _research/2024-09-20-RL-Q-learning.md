---
title:  "Understanding Q-learning in Reinforcement Learning"
date:   2024-09-20
collection: research
permalink: /research/Q_learning
---
Q-learning is a foundational algorithm in reinforcement learning, designed to help agents discover the optimal strategy for maximizing cumulative rewards in an environment. 
<figure style="display: flex; flex-direction: column; align-items: center;">
  <img src="{{ "/assets/img/learning/Q-learning.jpeg"  | absolute_url }}" alt="mode_shape" class="post-pic" style="width: 70%;"/>
</figure>

It is a **model-free algorithm**, meaning it doesn’t need a model of the environment, and it is **off-policy**, allowing the agent to learn the optimal behavior regardless of how it explores during training. The essence of Q-learning lies in estimating the **Q-values** of state-action pairs, which represent the long-term reward the agent can expect from a given state by taking a particular action. These Q-values are updated iteratively using the Q-learning equation:


$$
Q(s, a) \leftarrow Q(s, a) + \alpha \left[ r + \gamma \max_{a'} Q(s', a') - Q(s, a) \right]
$$


Here I provided a detailed Python implementation of a grid world example, where an agent learns the optimal path in a 4x4 grid to reach a target goal with a reward. Through this, I demonstrate how Q-learning works step-by-step, helping you understand how the algorithm can be applied to real-world problems like robotic control, game-playing, and more.

[Click here to access my GitHub code](https://github.com/YaroKazakov/RL-phd/blob/main/rl_book/code/Q_learning.ipynb)
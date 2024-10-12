---
title:  "Monte-Carlo Control (Q-learning) - Chapter 5 - Sutton and Barto"
date:   2024-09-18
collection: research
permalink: /research/chapter5_SB
---
In this chapter I cover Monte Carlo methods, which estimate value functions using sample returns from episodes without needing full knowledge of the environment's dynamics. 
<figure style="display: flex; flex-direction: column; align-items: center;">
  <img src="{{ "/assets/img/learning/monte-carlo.jpg"  | absolute_url }}" alt="mode_shape" class="post-pic" style="width: 70%;"/>
</figure>

These methods work well for episodic environments where each episode has a clear terminal state. I learned two types of Monte Carlo prediction: first-visit MC, which averages returns from the first time a state is visited, and every-visit MC, which averages returns across all visits to a state. Both approaches estimate the value function, but every-visit MC introduces bias due to correlated samples within episodes. I also explored incremental Monte Carlo, where the value function is updated incrementally using a learning rate, helping to smooth out the estimation process. Finally, I studied model-free control through Monte Carlo, focusing on learning optimal action values for decision-making without needing to model the entire environment. The Monte-Carlo control is also known as Q-learning because the objective is to simulate state-action values either on-policy or off-policy.

[Click here to access my GitHub pdf](https://github.com/YaroKazakov/RL-phd/blob/main/rl_book/chapter_notes/Chapter5_Monte_Carlo_notes.pdf)
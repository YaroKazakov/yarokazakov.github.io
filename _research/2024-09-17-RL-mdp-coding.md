---
title:  "Dynamic Programming (Markov Processes) - Chapter 4 - Sutton and Barto"
date:   2024-09-17
collection: research
permalink: /research/chapter4_SB
---
In these exercises (Chapter 4), I dove into how changing the horizon impacts the best strategy in an MDP. 

<figure style="display: flex; flex-direction: column; align-items: center;">
  <img src="{{ "/assets/img/learning/swimming.gif"  | absolute_url }}" alt="mode_shape" class="post-pic" style="width: 70%;"/>
  <figcaption style="text-align: center;">Alice-Bob Optimal Strategy as Defined by a Human</figcaption>
</figure>

I looked into reward hacking and how discount factor and [poor reward specification can lead to unexpected results](https://openreview.net/pdf?id=JYtwGwIL7ye). I worked with the Bellman backup equation to calculate expected rewards for different choices at each state. Coding the Policy Improvement, Bellman Operator, Policy iteration and Value Iteration functions was tricky, especially making sure the policy actually converged as it should. The RiverSwim problem added some fun challenges with its changing currents—tweaking the discount factor really affected how the agent behaved. One of the biggest struggles was getting everything to compute accurately without slowing things down too much. The reward hacking example was a real eye-opener, showing how easy it is for a poorly designed reward to push the AI toward the wrong behavior.

[Click here to access my GitHub code](https://github.com/YaroKazakov/RL-phd/blob/main/stanford_cs234/assignments/code/vi_and_pi.py)
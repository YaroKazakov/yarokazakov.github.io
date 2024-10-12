---
title:  "Foundations of Robot Motion - Chapter 2 - Lynch and Parker"
date:   2024-09-11
collection: research
permalink: /research/chapter2_robo_LP
---
Here, in Chapter 2 of Modern Robotics, I explore the concept of a robot's configuration and degrees of freedom (DoF), crucial for understanding robot motion. 
<figure style="display: flex; flex-direction: column; align-items: center;">
  <img src="{{ "/assets/img/learning/coppelia_sim.png"  | absolute_url }}" alt="mode_shape" class="post-pic" style="width: 70%;"/>
</figure>

The configuration space (C-space) represents all possible configurations of a robot, and the minimum number of coordinates needed to describe the robot's state is its degrees of freedom. Different types of joints, such as revolute, prismatic, and spherical, impose constraints on motion and influence the total DoF of a robot system. Grubler’s formula provides a method to calculate the DoF, accounting for the number of links, joints, and constraints. I also completed various exercises to apply these principles, such as determining the DoF for specific mechanisms and understanding how constraints like keeping a tray horizontal reduce available freedoms in motion.

[Click here to access my GitHub code](https://github.com/YaroKazakov/RL-phd/blob/main/robotics_book/Chapter%202%20-%20C-space%20-%20Notes%20and%20Exercises.pdf)

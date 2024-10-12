---
title:  "Research Internship at Imperial Rocketry"
date:   2020-06-20
permalink: /posts/internship_ICR
---
 This internship provided an excellent introduction to high-performance computing (HPC) using Julia.
<figure style="display: flex; flex-direction: column; align-items: center;">
  <img src="{{ "/assets/img/work/spaceport.jpg"  | absolute_url }}" alt="mode_shape" class="post-pic" style="width: 70%;"/>
</figure>

The project was part of the annual Imperial College Rocketry Team's entry in the Spaceport America Cup. The main objective was to implement a Mesh Adaptive Direct Search (MADS) algorithm in Julia for trajectory estimation of a gas-propelled rocket. MADS is an optimization algorithm designed to solve nonlinear optimization problems, particularly those with non-smooth or non-differentiable objective functions. It adapts the search mesh size based on the local behavior of the objective function, improving efficiency in finding optimal solutions.

The control algorithm aimed to optimize in-flight fuel consumption to maximize the rocket's apogee (the highest point in its trajectory). The internship was a success: the algorithm's runtime was reduced threefold, largely due to the effective introduction of caching mechanisms.

[Click here to view the repo I worked on]({{ "https://github.com/ImperialCollegeLondon/DirectSearch.jl" | absolute_url }})
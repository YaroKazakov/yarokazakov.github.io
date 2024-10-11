---
title:  "Sulzer Internship - Machine Learning for Damage Inspection in Gas Turbines"
date:   2019-06-26
permalink: /posts/internship_Sulzer
---
<figure style="display: flex; flex-direction: column; align-items: center;">
  <img src="{{ "/assets/img/work/gas-turbine-gif.gif"  | absolute_url }}" alt="mode_shape" class="post-pic" style="width: 70%;"/>
  <figcaption style="text-align: center;">Picture by [Process Tech Academy](https://www.processtechacademy.com/the-prime-movers-drivers-known-as-gas-turbines-suck-squeeze-bang-blow/).</figcaption>
</figure>

The 2019 internship at Sulzer[^1] allowed me to apply my machine learning knowledge to the seemingly rigid field of industrial engineering. At first glance, someone working in the gas turbine or turbojet engine sector might think the industry is "low-tech." However, this assumption would be incorrect. The gas turbine maintenance industry is already leveraging advanced supervised learning techniques to save millions of dollars annually. My experience, described below, shows how a short-term internship project can meaningfully optimize business processes.

A gas turbine requires regular maintenance, which is costly, and only a few companies worldwide possess the expertise to do it well. Gas turbines are subjected to corrosion, extreme heat, axial stress loads, and numerous other factors that can hinder operations, potentially leading to severe financial losses for utility companies. Examples of wet corrosion and heat damage are illustrated below.

<figure style="display: flex; flex-direction: column; align-items: center;">
  <img src="{{ "/assets/img/work/Damage_blade.png" | absolute_url }}" alt="mode_shape" class="post-pic" style="width: 70%;"/>
  <figcaption style="text-align: center;">Alice-Bob Optimal Strategy as Defined by a Human</figcaption>
</figure>

<figure style="display: flex; flex-direction: column; align-items: center;">
  <img src="{{ "/assets/img/work/Wet_corrosion_damage.png" | absolute_url }}" alt="mode_shape" class="post-pic" style="width: 70%;"/>
  <figcaption style="text-align: center;">Alice-Bob Optimal Strategy as Defined by a Human</figcaption>
</figure>

Turbine blades, in particular, are designed to be durable and are manufactured under strict supervision to ensure that the lattice structure of the superalloy contains minimal impurities and achieves high lattice coherence. These blades are exposed to high pressure and temperatures reaching up to 1300°C and are usually coated with thick layers of thermal barrier coatings (TBCs), typically made from zirconium oxide, as well as a bond coat, as shown below.

<figure style="display: flex; flex-direction: column; align-items: center;">
  <img src="{{ "/assets/img/work/Thermal_stress_damage.png"  | absolute_url }}" alt="mode_shape" class="post-pic" style="width: 70%;"/>
  <figcaption style="text-align: center;">Alice-Bob Optimal Strategy as Defined by a Human</figcaption>
</figure>

Due to operational conditions and environmental factors, gas turbine blades can develop cracks, particularly from the interaction with high-pressure, high-velocity, and high-temperature gases from the combustion chamber. These cracks are notoriously difficult to detect without a procedure known as "coating stripping"—a laborious and time-consuming process that requires hours of work from an on-site engineer. This procedure can cost utility companies $10-15 million per year.

<figure style="display: flex; flex-direction: column; align-items: center;">
  <img src="{{ "/assets/img/work/TBC_coating.png"  | absolute_url }}" alt="mode_shape" class="post-pic" style="width: 70%;"/>
  <figcaption style="text-align: center;">Alice-Bob Optimal Strategy as Defined by a Human</figcaption>
</figure>

Currently, an engineer must strip the coating from the blade before using techniques such as X-ray scanning, ultrasound inspection, or magnetic particle inspection to identify cracks. All of these methods require the "coating stripping" stage.

<figure style="display: flex; flex-direction: column; align-items: center;">
  <img src="{{ "/assets/img/work/Ultrasonic_inspection.png" | absolute_url }}" alt="mode_shape" class="post-pic" style="width: 70%;"/>
  <figcaption style="text-align: center;">Alice-Bob Optimal Strategy as Defined by a Human</figcaption>
</figure>


Instead, machine learning techniques can be employed during the signal processing stage of ultrasound inspections, allowing the tests to be conducted directly on the coated component. In this approach, an engineer applies magnetic particle or ultrasound diagnostics to the blade and observes additional "peaks" in the data due to the interaction of the waves with the external coating material. For this project, we used a proprietary labeled dataset containing over 300 turbine blades and a validation set of 50 samples.

<figure style="display: flex; flex-direction: column; align-items: center;">
  <img src="{{ "/assets/img/work/Magnetic_particle_diagram.png" | absolute_url }}" alt="mode_shape" class="post-pic" style="width: 70%;"/>
  <figcaption style="text-align: center;">Alice-Bob Optimal Strategy as Defined by a Human</figcaption>
</figure>

<figure style="display: flex; flex-direction: column; align-items: center;">
  <img src="{{ "/assets/img/work/Ultrasound_inspection_diagram.png" | absolute_url }}" alt="mode_shape" class="post-pic" style="width: 70%;"/>
  <figcaption style="text-align: center;">Alice-Bob Optimal Strategy as Defined by a Human</figcaption>
</figure>

Both the time and frequency domains of the signal were analyzed using Fourier transforms, power spectral density, and various normalization techniques. For classification, we applied random forest, support vector machines, k-nearest neighbors (k-NN), and a 32-layer autoencoder neural network, which focused on reconstruction errors.Interestingly, both random forest and k-NN performed exceptionally well with frequency domain data. The model's recall rate was 99.5%, which was a significant achievement, considering the tremendous cost of false negatives in this field. If implemented correctly, the business can saves tens of millions of dollars a year on coating stripping.

##### FOOTNOTES
[^1]: Sulzer is one the largest gas turbine maintenance service providers in the world. 

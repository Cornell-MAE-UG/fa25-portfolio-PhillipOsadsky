---
layout: project
title: Heat Exchanger Analysis for MAE 2210
description: Class Lab
image: /assets/images/counterflow.png
---

<style>
.image-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 1.2rem;
  margin: 1.25rem 0 2rem 0;
}

.image-grid img,
.feature-image {
  width: 100%;
  border-radius: 12px;
  box-shadow: 0 4px 14px rgba(0,0,0,0.12);
}

.feature-image {
  max-width: 900px;
  display: block;
  margin: 1.5rem auto;
}

.caption {
  text-align: center;
  font-size: 0.95rem;
  margin-top: 0.4rem;
  color: #555;
}

.comparison-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 1.5rem;
  margin: 1.25rem 0 2rem 0;
}

.data-card {
  background: #fafafa;
  border: 1px solid #ddd;
  border-radius: 14px;
  padding: 1rem;
  box-shadow: 0 3px 10px rgba(0,0,0,0.08);
}

.data-card img {
  width: 100%;
  border-radius: 12px;
  margin-bottom: 0.75rem;
}

.equation-box {
  background: #fafafa;
  border-left: 4px solid #8b1e3f;
  border-radius: 10px;
  padding: 1rem 1.2rem;
  margin: 1rem 0;
}

@media (max-width: 700px) {
  .image-grid,
  .comparison-grid {
    grid-template-columns: 1fr;
  }
}
</style>

## Overview

For a class project, we selected a real world instance of a device that we have learned about in our Thermodynamics course (MAE 2210), explained how it works in detail, and then discussed how its performance would change under change in design or operating conditions. The device that my partner and I chose to analyze was the heat exchanger.

Heat exchangers are widely used in engineering systems to transfer thermal energy between fluids without mixing. A couple examples include radiators, power plants, and one of my personal favorites, spacecraft thermal control. Understanding how the process behind a heat exchanger performance is influenced by its design and the way it operates is very important for designing systems in the class. 

In this project, we analyzed a specific heat exchanger shown in images below operated using two electric pumps and external thermal reservoirs. The objective was to experimentally compare parallel flow and counterflow configurations and evaluate their performance using mass, energy, and entropy balances.

---

## Setup

<div class="image-grid">
  <img src="{{ '/assets/images/exchanger.png' | relative_url }}"
       alt="Heat exchanger used in the experiment">

  <img src="{{ '/assets/images/setup.png' | relative_url }}"
       alt="Experimental heat exchanger setup">

  <img src="{{ '/assets/images/cross-section-1.png' | relative_url }}"
       alt="Heat exchanger cross-section view 1">

  <img src="{{ '/assets/images/cross-section-2.png' | relative_url }}"
       alt="Heat exchanger cross-section view 2">
</div>

<p class="caption">
Experimental setup, heat exchanger body, and internal cross-section views.
</p>

The experimental supplies consisted of:
* A compact water-to-water heat exchanger
* Two submersible water pumps
* Four water reservoirs (in our case, buckets)
* An immersion heater (hot reservoir)
* Ice and insulation (cold reservoir)
* Thermometers and a thermocouple
* Food dye for flow visualization

The hot reservoir temperature was controlled using the immersion heater, while the cold reservoir temperature was lowered using ice and insulation. Each reservoir was initially filled completely to allow sufficient runtime for near steady-state operation.

The four ports of the heat exchanger were configured to allow operation in either parallel flow or counterflow, with no mixing between the hot and cold streams. Temperatures were measured at all inlets and outlets once steady operation was reached.

There were several assumptions that we made in this process. The heat exchanger was modeled as a steady-flow control volume enclosing both fluid streams.<br/>

**Assumptions**: 
* Steady-state operation 
* Incompressible liquid water 
* Constant specific heat capacity, c<sub>p</sub>= 4.182 kJ/(kg*K) 
* Negligible kinetic and potential energy changes 
* No shaft work interaction 
* Equal mass flow rates for hot and cold streams 
* Heat loss to ambient air at the exchanger surface 

These assumptions are reasonable given the low flow velocities, small elevation changes, and the experimental setup.

---

## Equations to analyze:

<div class="equation-box">

* Mass Balance, since there is no mixing and steady operation
  - m˙<sub>h,i​</sub>=m˙<sub>h,e</sub>​=m˙<sub>c,i</sub>​=m˙<sub>c,e</sub>​=m˙ 

* Energy Balance With no work interaction and negligible KE/PE changes
  - Q˙<sub>​lost</sub>​=m˙c<sub>p</sub>​((T<sub>c,e</sub>​−T<sub>c,i</sub>​)+(T<sub>h,e</sub>​−T<sub>h,i</sub>​))

* Entropy Balance
  - S˙<sub>gen</sub>​=m˙(c<sub>p</sub>​ln(T<sub>c,e</sub>/​T<sub>c,i</sub>​​)+c<sub>p</sub>​ln(T<sub>h,e</sub>/​T<sub>h,i</sub>​​))−​Q˙<sub>​lost</sub>/​T<sub>amb</sub>​ ​ ​ 

</div>

The calculations corresponding to these equations are shown in the image below.

We considered changing and monitoring the effect of the operation of the exchanger in parallel flow vs counter flow.

---

## Data

<div class="comparison-grid">

  <div class="data-card">
    <img src="{{ '/assets/images/Parallel.png' | relative_url }}"
         alt="Parallel flow heat exchanger setup">

    <h3>Parallel Flow</h3>

    <p><strong>Parallel</strong>:</p>
    <ul>
      <li>We found the initial temperature of the water in the cold reservoir to be <strong>6 °C</strong> and the warm reservoir to be <strong>40 °C</strong>.</li>
      <li>The initial temperature of the exchanger was <strong>20.7 °C</strong>.</li>
      <li>During the process, the exchanger was at <strong>20 °C</strong>.</li>
      <li>The temperature of the water from the cold reservoir after going through the exchanger was <strong>20.5 °C</strong> and the water from the warm reservoir was <strong>23.8 °C</strong>.</li>
    </ul>
  </div>

  <div class="data-card">
    <img src="{{ '/assets/images/counterflow.png' | relative_url }}"
         alt="Counterflow heat exchanger setup">

    <h3>Counterflow</h3>

    <p><strong>Counter-flow</strong>:</p>
    <ul>
      <li>We found the initial temperature of the water in the cold reservoir to be <strong>5 °C</strong> and the warm reservoir to be <strong>40 °C</strong>.</li>
      <li>The initial temperature of the exchanger was <strong>20.8 °C</strong>.</li>
      <li>During the process, the exchanger was at <strong>18 °C</strong>.</li>
      <li>The temperature of the water from the cold reservoir after going through the exchanger was <strong>25.7 °C</strong> and the water from the warm reservoir was <strong>18.8 °C</strong>.</li>
    </ul>
  </div>

</div>

---

## Analysis and Calculations

<img src="{{ '/assets/images/work3.png' | relative_url }}"
     alt="Written heat exchanger analysis and calculations"
     class="feature-image">

<p class="caption">
Written calculations using mass, energy, and entropy balances.
</p>

Our analysis and work is written out and shown in the picture above:

With the values that we got, we are able to make a couple of conclusions on the heat exchanger that we worked with. First, we can safely conclude that the counterflow setup outperformed the parallel flow. Cold fluid reached a much higher outlet temperature in counterflow (25.7 degrees Celsius vs 20.5 degrees Celsius) while the hot fluid cooled more (to 18.8 degrees Celsius vs 23.8 degrees Celsius). This behavior aligns with the heat exchanger theory that counterflow allows a larger effective temperature difference along the exchanger length. The advantage of the counterflow is that the cold fluid can approach the hot inlet temperature more closely. We can also see that the parallel setup lost more net energy to the ambient, or the surrounding air, than the counterflow setup, making the counterflow setup more desirable yet again. This also explains why the hot stream leaves colder than the cold stream leaves; heat is lost in the exchanger itself. If heat were not lost, our counterflow setup would have violated the second law of thermodynamics, but since that cannot happen, we can conclude that the heat exchanger does in fact have heat loss and that this is a non adiabatic system. Both values of entropy calculated show that reversibility is not possible, which is what we would expect with this type of device. 

---

## Conclusion and application

Our analysis can be applied to real world scenarios, where reducing entropy generation and heat loss improves efficiency, lowers operating costs, and enhances system reliability, which are considerations in engineering design. This project demonstrates how what we learn in our thermodynamics course can be applied to a real physical system. By combining experimental data with mass, energy, and entropy balances, we were able to show the advantages of counterflow heat exchanger operation.
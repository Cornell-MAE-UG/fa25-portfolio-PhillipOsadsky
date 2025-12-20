---
layout: project
title: Heat Exchanger Analysis for MAE 2210
description: Experimental thermodynamic analysis of a compact water-to-water heat exchanger
image: /assets/images/counterflow.png
---

*Completed in collaboration with Gabe Anagnoson (gaa72).*

## Overview

For this project in **MAE 2210: Thermodynamics**, we analyzed a **real, experimentally operated heat exchanger** to evaluate how its performance changes with operating configuration. Heat exchangers are fundamental components in many engineering systems, including radiators, power plants, and spacecraft thermal control systems.

Our objective was to experimentally compare **parallel-flow** and **counterflow** configurations using **mass, energy, and entropy balances**, and to interpret the results using thermodynamic theory.

---

## Experimental Setup

<div class="image-row">
  <img src="{{ '/assets/images/exchanger.png' | relative_url }}" alt="Heat exchanger">
  <img src="{{ '/assets/images/setup.png' | relative_url }}" alt="Experimental setup">
  <img src="{{ '/assets/images/cross-section-1.png' | relative_url }}" alt="Cross section 1">
  <img src="{{ '/assets/images/cross-section-2.png' | relative_url }}" alt="Cross section 2">
</div>

The experimental apparatus consisted of:
- A compact water-to-water heat exchanger  
- Two submersible electric water pumps  
- Four water reservoirs  
- An immersion heater (hot reservoir)  
- Ice and insulation (cold reservoir)  
- Thermometers and a thermocouple  
- Food dye for flow visualization  

The hot reservoir temperature was regulated using an immersion heater, while the cold reservoir was maintained using ice and insulation. Each reservoir was filled completely to ensure sufficient runtime for near steady-state operation.

The four ports of the heat exchanger allowed configuration in either **parallel flow** or **counterflow**, with no mixing between the hot and cold streams.

---

## Modeling Assumptions

The heat exchanger was modeled as a **steady-flow control volume** enclosing both fluid streams.

**Assumptions:**
- Steady-state operation  
- Incompressible liquid water  
- Constant specific heat capacity  
  - \( c_p = 4.182 \, \text{kJ/(kg·K)} \)  
- Negligible kinetic and potential energy changes  
- No shaft work interaction  
- Equal mass flow rates for hot and cold streams  
- Heat loss to ambient air  

These assumptions are reasonable given the low flow velocities, small elevation changes, and laboratory-scale setup.

---

## Governing Equations

**Mass Balance**
\[
\dot{m}_{h,i} = \dot{m}_{h,e} = \dot{m}_{c,i} = \dot{m}_{c,e} = \dot{m}
\]

**Energy Balance**
\[
\dot{Q}_{lost} = \dot{m} c_p \left[(T_{c,e} - T_{c,i}) + (T_{h,e} - T_{h,i})\right]
\]

**Entropy Balance**
\[
\dot{S}_{gen} =
\dot{m} c_p \left[\ln\left(\frac{T_{c,e}}{T_{c,i}}\right)
+ \ln\left(\frac{T_{h,e}}{T_{h,i}}\right)\right]
- \frac{\dot{Q}_{lost}}{T_{amb}}
\]

---

## Experimental Data

### Parallel Flow
- Cold reservoir inlet: **6 °C**
- Hot reservoir inlet: **40 °C**
- Cold outlet: **20.5 °C**
- Hot outlet: **23.8 °C**

![Parallel flow results]({{ "/assets/images/Parallel.png" | relative_url }}){: .inline-image-r}

### Counterflow
- Cold reservoir inlet: **5 °C**
- Hot reservoir inlet: **40 °C**
- Cold outlet: **25.7 °C**
- Hot outlet: **18.8 °C**

![Counterflow results]({{ "/assets/images/counterflow.png" | relative_url }}){: .inline-image-r}

---

## Analysis and Calculations

![Hand calculations]({{ "/assets/images/work3.png" | relative_url }}){: .inline-image-r}

The counterflow configuration consistently outperformed the parallel-flow configuration. The cold stream achieved a higher outlet temperature while the hot stream experienced greater cooling. This aligns with heat exchanger theory, as counterflow maintains a larger effective temperature difference along the exchanger length.

The results also indicate measurable heat loss to the ambient environment, explaining why the hot outlet temperature fell below the cold outlet temperature in the counterflow case. Without heat loss, this behavior would violate the second law of thermodynamics, confirming that the exchanger operates as a **non-adiabatic system**.

Entropy generation values were positive in both configurations, as expected for a real, irreversible device.

---

## Conclusion and Engineering Relevance

This project demonstrates how thermodynamic principles apply directly to real engineering systems. By combining experimental data with mass, energy, and entropy balances, we verified the superior performance of counterflow heat exchanger operation.

In practical applications, minimizing entropy generation and heat loss leads to higher efficiency, reduced operating costs, and improved system reliability. This analysis reflects the type of trade studies and performance evaluations commonly performed in thermal system design.

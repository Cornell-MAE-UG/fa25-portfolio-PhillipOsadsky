---
layout: project
title: Heat Exchanger
description: Class Lab
image: /assets/images/setup.png
---

# Heat Exchanger Analysis for MAE 2210

I worked on this assignment with my lab partner Gabe Anagnoson (gaa72).

## Overview

For a class project, we selected a real world instance of a device that we have learned about in our Thermodynamics course (MAE 2210), explained how it works in detail, and then discussed how its performance would change under change in design or operating conditions. The device that my partner and I chose to analyze was the heat exchanger.

Heat exchangers are widely used in engineering systems to transfer thermal energy between fluids without mixing. A couple examples include radiators, power plants, and one of my personal favorites, spacecraft thermal control. Understanding how the process behind a heat exchanger performance is influenced by its design and the way it operates is very important for designing systems in the class. 

 In this project, we analyzed a specific heat exchanger (shown in images below) operated using two electric pumps and external thermal reservoirs. The objective was to experimentally compare parallel flow and counterflow configurations and evaluate their performance using mass, energy, and entropy balances.

## Setup

The experimental supplies consisted of:
• A compact water-to-water heat exchanger
• Two submersible water pumps
• Four water reservoirs (in our case, buckets)
• An immersion heater (hot reservoir)
• Ice and insulation (cold reservoir)
• Thermometers and a thermocouple
• Food dye for flow visualization

The hot reservoir temperature was controlled using the immersion heater, while the cold reservoir temperature was lowered using ice and insulation. Each reservoir was initially filled completely to allow sufficient runtime for near steady-state operation.

The four ports of the heat exchanger were configured to allow operation in either parallel flow or counterflow, with no mixing between the hot and cold streams. Temperatures were measured at all inlets and outlets once steady operation was reached.

![Photo of solution]({{ "/assets/images/setup.png" | relative_url }}){: .inline-image-r}
![Photo of solution]({{ "/assets/images/exchanger.png" | relative_url }}){: .inline-image-r}

There were several assumptions that we made in this process. The heat exchanger was modeled as a steady-flow control volume enclosing both fluid streams. 
Assumptions: 
• Steady-state operation 
• Incompressible liquid water 
• Constant specific heat capacity, c<sub>p</sub>= 4.182 kJ/(kg*K) 
• Negligible kinetic and potential energy changes 
• No shaft work interaction 
• Equal mass flow rates for hot and cold streams 
• Heat loss to ambient air at the exchanger surface 
These assumptions are reasonable given the low flow velocities, small elevation changes, and the experimental setup.

## Equations to analyze:
**Mass Balance, since there is no mixing and steady operation**: m˙<sub>h,i​</sub>=m˙<sub>h,e</sub>​=m˙<sub>c,i</sub>​=m˙<sub>c,e</sub>​=m˙ **Energy Balance With no work interaction and negligible KE/PE changes**: Q˙<sub>​lost</sub>​=m˙c<sub>p</sub>​((T<sub>c,e</sub>​−T<sub>c,i</sub>​)+(T<sub>h,e</sub>​−T<sub>h,i</sub>​))
**Entropy Balance**: S˙<sub>gen</sub>​=m˙(c<sub>p</sub>​ln(T<sub>c,e</sub>/​T<sub>c,i</sub>​​)+c<sub>p</sub>​ln(T<sub>h,e</sub>/​T<sub>h,i</sub>​​))−​Q˙<sub>​lost</sub>/​T<sub>amb</sub>​ ​ ​ 

![Photo of solution]({{ "/assets/images/cross-section-1.png" | relative_url }}){: .inline-image-r}
![Photo of solution]({{ "/assets/images/cross-section-2.png" | relative_url }}){: .inline-image-r}

The calculations corresponding to these equations are shown in the image below.

We considered changing and monitoring the effect of the operation of the exchanger in parallel flow vs counter flow.
## Data
**Parallel**: We found the initial temperature of the water in the cold reservoir to be 6 degrees Celsius and the warm reservoir to be 40 degrees Celsius. The initial temperature of the exchanger was 20.7 degrees Celsius. During the process, the exchanger was at 20 degrees. The temperature of the water from the cold reservoir after going through the exchanger was 20.5 degrees and the water from the warm reservoir was 23.8 degrees.

**Counter-flow**: We found the initial temperature of the water in the cold reservoir to be 5 degrees Celsius and the warm reservoir to be 40 degrees Celsius. The initial temperature of the exchanger was 20.8 degrees Celsius. During the process, the exchanger was at 18 degrees. The temperature of the water from the cold reservoir after going through the exchanger was 25.7 degrees and the water from the warm reservoir was 18.8 degrees.

![Photo of solution]({{ "/assets/images/Parallel.png" | relative_url }}){: .inline-image-r}

![Photo of solution]({{ "/assets/images/counterflow.png" | relative_url }}){: .inline-image-r}
## Analysis and Calculations
Our analysis and work is written out and shown in the picture below:
![Photo of solution]({{ "/assets/images/work3.png" | relative_url }}){: .inline-image-l}
With the values that we got, we are able to make a couple of conclusions on the heat exchanger that we worked with. First, we can safely conclude that the counterflow setup outperformed the parallel flow. Cold fluid reached a much higher outlet temperature in counterflow (25.7 degrees Celsius vs 20.5 degrees Celsius) while the hot fluid cooled more (to 18.8 degrees Celsius vs 23.8 degrees Celsius). This behavior aligns with the heat exchanger theory that counterflow allows a larger effective temperature difference along the exchanger length. The advantage of the counterflow is that the cold fluid can approach the hot inlet temperature more closely. We can also see that the parallel setup lost more net energy to the ambient, or the surrounding air, than the counterflow setup, making the counterflow setup more desirable yet again. This also explains why the hot stream leaves colder than the cold stream leaves; heat is lost in the exchanger itself. If heat were not lost, our counterflow setup would have violated the second law of thermodynamics, but since that cannot happen, we can conclude that the heat exchanger does in fact have heat loss and that this is a non adiabatic system. Both values of entropy calculated show that reversibility is not possible, which is what we would expect with this type of device. 

## Conclusion and application

Our analysis can be applied to real world scenarios, where reducing entropy generation and heat loss improves efficiency, lowers operating costs, and enhances system reliability, which are considerations in engineering design. This project demonstrates how what we learn in our thermodynamics course can be applied to a real physical system. By combining experimental data with mass, energy, and entropy balances, we were able to show the advantages of counterflow heat exchanger operation.



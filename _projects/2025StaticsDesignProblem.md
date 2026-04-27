---
layout: project
title: 2025 Statics Design Problem
description: Designing a statics mechanism
technologies: 
image: /assets/images/radio-machine-cad.jpg
---

<style>
.project-image-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 1.2rem;
  margin: 1.5rem 0 2rem 0;
}

.project-image-card {
  background: #fafafa;
  border: 1px solid #ddd;
  border-radius: 14px;
  padding: 0.8rem;
  box-shadow: 0 3px 10px rgba(0,0,0,0.08);
}

.project-image-card img {
  width: 100%;
  border-radius: 10px;
  display: block;
}

.project-section {
  background: #fcfcfc;
  border-left: 4px solid #8b1e3f;
  border-radius: 12px;
  padding: 1rem 1.2rem;
  margin: 1.25rem 0;
}

@media (max-width: 700px) {
  .project-image-grid {
    grid-template-columns: 1fr;
  }
}
</style>

## Project Overview

<div style="display:flex; gap:1.5rem; flex-wrap:wrap; margin:1.5rem 0;">

  <img src="{{ '/assets/images/Adobe Scan Oct 10, 2025.png' | relative_url }}"
       alt="Statics mechanism sketch"
       style="width:48%; min-width:300px; border-radius:12px; box-shadow:0 4px 12px rgba(0,0,0,0.12);">

  <img src="{{ '/assets/images/Deflection.png' | relative_url }}"
       alt="Beam deflection analysis"
       style="width:48%; min-width:300px; border-radius:12px; box-shadow:0 4px 12px rgba(0,0,0,0.12);">

</div>

<div class="project-section">

For a class, we were asked to design and sketch a mechanism of dimensions 150cm x 50cm to lift a load of maximum weight and a maximum height. We are given a bar of a fixed length, 3 pin supports two of which are on the ground, and a linear actuator of our choice from an online catalog using the maximum force values. I ended up sketching a diagram and calculating the force using moment equilibrium and the respective angles with the top and bottom of the bar. Using geometric principles, I found the appropriate values in order to maximize weight and height of the bar. My solution was to use the bar to rotate the load at the maximum length with the actuator which had the highest load and the largest stroke strength.

</div>

## Beam Deflection Update

<div class="project-section">

Update December 8, 2025: In this step, the original rigid bar was replaced with a flexible beam, and its deflection under the transverse components of the actuator force and lifted weight was analyzed. Treating the beam of length 1.40 m with a 2240 N downward load at the tip and a 105 N upward actuator force applied 0.60 m from the root, I derived a general expression for tip deflection and evaluated the combined load effect as a single geometry constant. To keep the vertical deflection below 2% of the beam length (28 mm), I did a mass-efficient sizing and chose a carbon-fiber–reinforced polymer hollow tube—103 mm outer diameter, 2 mm wall thickness—which provides sufficient stiffness (I ≈ 8.0×10⁻⁷ m⁴) to limit deflection to approximately 27.8 mm while keeping the beam very lightweight (~1.4 kg). A final schematic of the chosen beam, actuator location, and loading configuration was produced to complete the design.

</div>
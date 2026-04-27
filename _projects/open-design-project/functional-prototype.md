---
layout: project
title: Functional Prototype
description: Retractable protective enclosure prototype for spotted lanternfly prevention in vineyards
technologies: Jekyll, Fusion 360, 3D Printer
image: /assets/images/FunctionalPrototypeHero.png
permalink: /projects/open-design-project/functional-prototype/
show_in_projects: false
---

<style>
.milestone-nav {
  display: grid;
  grid-template-columns: repeat(2, minmax(220px, 1fr));
  gap: 1rem;
  margin: 1rem 0 2rem 0;
}

.milestone-card {
  display: block;
  padding: 1rem 1.2rem;
  border: 2px solid #d9d9d9;
  border-radius: 14px;
  text-decoration: none;
  background: #fafafa;
  box-shadow: 0 2px 8px rgba(0,0,0,0.06);
  transition: transform 0.18s ease, box-shadow 0.18s ease, border-color 0.18s ease;
}

.milestone-card:hover {
  transform: translateY(-2px);
  box-shadow: 0 6px 14px rgba(0,0,0,0.10);
  border-color: #8b1e3f;
  text-decoration: none;
}

.milestone-card h3 {
  margin: 0 0 0.35rem 0;
}

.quick-facts {
  display: grid;
  grid-template-columns: repeat(3, minmax(160px, 1fr));
  gap: 0.8rem;
  margin: 1.25rem 0 2rem 0;
}

.fact-box {
  background: #f7f7f7;
  border-left: 4px solid #8b1e3f;
  border-radius: 10px;
  padding: 0.9rem 1rem;
}

.section-card {
  background: #fcfcfc;
  border: 1px solid #e4e4e4;
  border-radius: 14px;
  padding: 1.2rem;
  margin: 1.25rem 0;
}

img.clean-img {
  width: 100%;
  max-width: 850px;
  display: block;
  margin: 1rem auto;
  border-radius: 12px;
  box-shadow: 0 4px 14px rgba(0,0,0,0.12);
}

table.clean-table {
  width: 100%;
  border-collapse: collapse;
  margin: 1rem 0 1.5rem 0;
  font-size: 0.98rem;
}

table.clean-table th, table.clean-table td {
  border: 1px solid #d7d7d7;
  padding: 0.7rem;
  text-align: left;
  vertical-align: top;
}

table.clean-table th {
  background: #f2f2f2;
}

.jump-link {
  font-weight: 600;
}

@media (max-width: 700px) {
  .milestone-nav,
  .quick-facts {
    grid-template-columns: 1fr;
  }
}
</style>

# The Lanternfly Terminator

**Team Bug-anators**  
**Client(s):** Cornell CALS Extension / E&J Gallo Winery / National Grape

*Note: While our initial client pitch focused on a scented spotted lanternfly (SLF) trap, our design evolved into a retractable barrier system after finding that physically preventing access to grapevines offered a solution that is more appropiate to the scope of this class.* 

This project explores a **retractable protective enclosure for grapevines** designed to reduce spotted lanternfly access while still allowing growers to quickly open the system for harvesting and maintenance with any types of machines.
---
## Design Evolution

<div style="display:grid; grid-template-columns: repeat(2, 1fr); gap:1rem; margin-top:1rem;">

  <img src="{{ '/assets/images/9-28-48AM.png' | relative_url }}"
       style="width:100%; border-radius:12px; box-shadow:0 4px 12px rgba(0,0,0,0.12);">

  <img src="{{ '/assets/images/9-28-55AM.png' | relative_url }}"
       style="width:100%; border-radius:12px; box-shadow:0 4px 12px rgba(0,0,0,0.12);">

  <img src="{{ '/assets/images/9-29-03AM.png' | relative_url }}"
       style="width:100%; border-radius:12px; box-shadow:0 4px 12px rgba(0,0,0,0.12);">

  <img src="{{ '/assets/images/9-30-25AM.png' | relative_url }}"
       style="width:100%; border-radius:12px; box-shadow:0 4px 12px rgba(0,0,0,0.12);">

</div>

<p style="text-align:center; margin-top:0.5rem;">
Early concept sketches exploring retractable mesh enclosure and scissor-based expansion mechanisms.
</p>

---

<div class="quick-facts">
  <div class="fact-box">
    <strong>Main Goal</strong><br>
    Keep SLFs off grapevines while preserving access for harvesting.
  </div>
  <div class="fact-box">
    <strong>Core Mechanism</strong><br>
    Retractable scissor linkage on a rigid frame with a guided rail/wheel system.
  </div>
  <div class="fact-box">
    <strong>Prototype Focus</strong><br>
    Structural stability, motion reliability, and fastener security.
  </div>
</div>

---

## <span id="functional-prototype">Functional Prototype</span>

### Purpose of the Prototype

The purpose of this functional prototype was to test whether a **retractable enclosure system** could realistically protect grapevines from spotted lanternflies while remaining practical for vineyard use. The prototype focuses on the key mechanical idea: a rigid frame and expandable scissor link structure that can open and close to cover an area.

In the full concept, a mesh barrier would move with the mechanism to block SLFs while still allowing light and air to pass through. For this prototype, we primarily tested the **mechanical behavior of the structure itself**, especially the parts most likely to fail during the operation.

<div class="section-card">
  <strong>Prototype concept:</strong> when expanded, the structure encloses the grapevine area; when contracted, it opens to allow harvesting or maintenance access.
</div>

<img src="{{ '/assets/images/FunctionalPrototypeHero.png' | relative_url }}"
     alt="CAD view of the functional prototype showing the retractable frame and scissor linkage"
     class="clean-img">

<p><a class="jump-link" href="#tests">Jump to Tests ↓</a></p>
<div style="display:grid; grid-template-columns: repeat(2, 1fr); gap:1rem; margin-top:1rem;">

  <img src="{{ '/assets/images/9-29-31AM.png' | relative_url }}"
       style="width:100%; border-radius:12px;">

  <img src="{{ '/assets/images/9-29-41AM.png' | relative_url }}"
       style="width:100%; border-radius:12px;">

</div>

<p style="text-align:center;">
Detailed CAD model showing scissor linkage geometry and frame structure.
</p>
---

### Design Overview

The prototype used four main subsystems:

1. **Rigid support frame**  
   Aluminum framing members create the structure and maintain alignment.

2. **Scissor linkage**  
   A scissor linkage system allows the top of the enclosure to expand and contract.

3. **Wheel–rail system**  
   A wheel carriage moves along the lower rail to support the frame.

4. **Fastened joints**  
   L-brackets, bolts, and nuts hold the frame together and transfer load during motion.

Because several ordered parts did not arrive in time, some components were fabricated in the lab. The wheel assembly was 3D printed, and the scissor linkage was machined from wood for this iteration.

---

### Key Parts Used

<table class="clean-table">
  <thead>
    <tr>
      <th>Part</th>
      <th>Description</th>
      <th>Material</th>
      <th>Source / Fabrication</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>T-slotted framing rail</td>
      <td>1" × 1" four-slot rail</td>
      <td>Aluminum</td>
      <td>McMaster 47065T101</td>
    </tr>
    <tr>
      <td>Aluminum U-channel</td>
      <td>6063 aluminum, 1/16" wall</td>
      <td>Aluminum</td>
      <td>McMaster 9001K787</td>
    </tr>
    <tr>
      <td>Scissor linkage</td>
      <td>Two rows of 2" × 12" link members in criss-cross form</td>
      <td>Wood</td>
      <td>Fabricated in shop</td>
    </tr>
    <tr>
      <td>L-brackets + fasteners</td>
      <td>Frame joining hardware</td>
      <td>Aluminum / steel</td>
      <td>Spare parts</td>
    </tr>
    <tr>
      <td>Wheel + wheel mount</td>
      <td>Guided rail motion system</td>
      <td>PLA</td>
      <td>3D printed</td>
    </tr>
    <tr>
      <td>Driveshaft</td>
      <td>Wheel axle</td>
      <td>Steel</td>
      <td>Spare stock</td>
    </tr>
  </tbody>
</table>

---

### Assembly Summary

<img src="{{ '/assets/images/9-30-25AM.png' | relative_url }}" 
     style="width:100%; max-width:800px; display:block; margin:1rem auto; border-radius:12px;">

The frame was built from cut aluminum extrusions from McMaster Carr connected with L-brackets. A custom wheel assembly was designed and 3D printed to fit the lower rail. The scissor linkage mechanism was machined from wood strips, drilled at evenly spaced pivot locations, and mounted to the upper frame rail. One side of the linkage was coupled to the wheeled frame so that retraction and extension was able to be done in a synchronized motion.
---
## Physical Prototype

<div style="display:grid; grid-template-columns: repeat(3, 1fr); gap:1rem; margin-top:1rem;">

  <img src="{{ '/assets/images/9-28-25AM.png' | relative_url }}" 
      style="width:100%; border-radius:12px;">
  <img src="{{ '/assets/images/9-28-34AM.png' | relative_url }}" 
      style="width:100%; border-radius:12px;">
  <img src="{{ '/assets/images/9-28-48AM.png' | relative_url }}" 
      style="width:100%; border-radius:12px;">

  <img src="{{ '/assets/images/9-28-55AM.png' | relative_url }}" 
      style="width:100%; border-radius:12px;">
  <img src="{{ '/assets/images/9-29-03AM.png' | relative_url }}" 
      style="width:100%; border-radius:12px;">
  <img src="{{ '/assets/images/9-30-00AM.png' | relative_url }}" 
      style="width:100%; border-radius:12px;">

</div>

<p style="text-align:center;">
Early-stage physical prototype used to validate structure, motion, and assembly feasibility.
</p>
---
<img src="{{ '/assets/images/FunctionalPrototypeAssembly.png' | relative_url }}"
     alt="Assembly photos showing construction of the functional prototype"
     class="clean-img">

---

## <span id="tests">Design Tests</span>

The most important mechanical risks were:
- Whether the scissor linkage could hold shape under load.
- Whether the wheel carriage could move smoothly without jamming.
- Whether the fasteners would stay secure over repeated cycles.

Each test below states what was tested, how it was tested, the measured result, and what should change in the next iteration.

---

### 1) Scissor-Linkage Structural Test

<div class="section-card">
  <strong>What was tested:</strong> the structural integrity of the scissor linkage and how much the frame tilts under load.
</div>

**Method:**  
Equal masses were added to both sides of the scissor linkage in **88g increments** while the mechanism was extended. We recorded the angular tilt and noted any visible stress or creaking sounds.

<table class="clean-table">
  <thead>
    <tr>
      <th>Applied Load (each side)</th>
      <th>Observed Result</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>88 g</td>
      <td>~6° tilt</td>
    </tr>
    <tr>
      <td>176 g</td>
      <td>~10° tilt</td>
    </tr>
    <tr>
      <td>264 g</td>
      <td>~10° tilt with audible creaking in wood</td>
    </tr>
    <tr>
      <td>352 g</td>
      <td>~10° tilt, partially stabilized by screw coupling</td>
    </tr>
  </tbody>
</table>

**Outcome:**  
The linkage stayed functional, but we began noticing some tilt began at a relatively low load. Creaking at 264 g showed the current wood members were approaching their structural limit.

**Next iteration:**  
Replace the wooden scissor members with a stiffer material once it comes with the Amazon order, and improve the support so the movable frame stays upright during extension.

<div style="display:grid; grid-template-columns: repeat(2, 1fr); gap:1rem; margin-top:1rem;">

  <img src="{{ '/assets/images/9-28-25AM.png' | relative_url }}"
       style="width:100%; border-radius:12px;">

  <img src="{{ '/assets/images/9-28-34AM.png' | relative_url }}"
       style="width:100%; border-radius:12px;">

</div>

---

### 2) Wheel–Rail Motion Test

<div class="section-card">
  <strong>What was tested:</strong> whether the wheel system could move along the rail smoothly without jamming or derailment.
</div>

**Method:**  
The system was moved back and forth along the full rail length for 10 iterations. Jams were counted for each iteration.

<table class="clean-table">
  <thead>
    <tr>
      <th>Iteration</th>
      <th>Number of Jams</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>1</td><td>0</td></tr>
    <tr><td>2</td><td>0</td></tr>
    <tr><td>3</td><td>0</td></tr>
    <tr><td>4</td><td>1</td></tr>
    <tr><td>5</td><td>2</td></tr>
    <tr><td>6</td><td>2</td></tr>
    <tr><td>7</td><td>1</td></tr>
    <tr><td>8</td><td>3</td></tr>
    <tr><td>9</td><td>3</td></tr>
    <tr><td>10</td><td>3</td></tr>
  </tbody>
</table>

**Outcome:**  
The system moved smoothly during the early cycles and generally remained usable. Later jams suggested some alignment sensitivity, although our human error in manual operation likely contributed to inconsistency.

**Next iteration:**  
Add alignment guides or constraints and transition for our motor driven motion for more consistent force application when our motor arrives from Amazon.

---

### 3) Fastener Security Test

<div class="section-card">
  <strong>What was tested:</strong> whether bolts and bracket connections loosen during repeated motion.
</div>

**Method:**  
All fasteners were tightened before testing. After repeated expansion and contraction cycles, we recorded the number of loosened bolts.

<table class="clean-table">
  <thead>
    <tr>
      <th>Iteration</th>
      <th>Bolts That Loosened</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>1</td><td>0</td></tr>
    <tr><td>2</td><td>0</td></tr>
    <tr><td>3</td><td>1</td></tr>
    <tr><td>4</td><td>1</td></tr>
    <tr><td>5</td><td>2</td></tr>
    <tr><td>6</td><td>2</td></tr>
    <tr><td>7</td><td>2</td></tr>
    <tr><td>8</td><td>3</td></tr>
    <tr><td>9</td><td>4</td></tr>
    <tr><td>10</td><td>4</td></tr>
  </tbody>
</table>

**Outcome:**  
The joints stayed secure at first, but more fasteners loosened as cycling increased, showing that repeated motion and vibration reduce reliability.

**Next iteration:**  
Use lock nuts, washers, or thread-locking adhesive, and improve joint design to reduce vibration at connection points.

---

## Success Criteria

To judge whether the final prototype is successful, the design needs measurable criteria tied directly to vineyard use.

<table class="clean-table">
  <thead>
    <tr>
      <th>Criterion</th>
      <th>What It Assesses</th>
      <th>Quantitative Requirement</th>
      <th>How It Is Measured</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Structural stability</td>
      <td>Whether the frame and scissor mechanism remain upright and intact</td>
      <td>≤ 5 in deflection during operation; no structural failure after 20 cycles</td>
      <td>Measure top-frame displacement and inspect after repeated cycles</td>
    </tr>
    <tr>
      <td>Smooth motion</td>
      <td>Whether the wheel system moves continuously without major interruption</td>
      <td>Full rail travel without derailment or jamming; no stop longer than 5 seconds</td>
      <td>Run full travel tests and time interruptions</td>
    </tr>
    <tr>
      <td>Fastener reliability</td>
      <td>Whether joints remain secure during repeated use</td>
      <td>≤ 10% of fasteners require retightening after 20 cycles; no complete fastener failure</td>
      <td>Inspect and record loosened fasteners after cycling</td>
    </tr>
  </tbody>
</table>

---

## Exhibit-Day Demo

The clearest demo criterion is **smooth motion of the scissor linkage and wheel–rail system**.

For the exhibit, the prototype can be shown performing repeated full **expansion and contraction cycles**. The audience will be able to see the system move between an enclosed position and an open access position, while the cycle time is measured to give quantitative results.

---

## Reflection

This prototype successfully identified the key design risks in the current concept. The main positive result was that the enclosure mechanism could expand and retract in a reliable way. The main issues were structural tilt in the scissor linkage, jamming sensitivity in the rail system, and gradual fastener loosening under repeated use.

These results give a clear direction for the next prototype:
- Stronger linkage material.
- Better alignment control.
- More secure fastening methods.

---

### Related Work
- <a href="{{ '/projects/ClientPitch/' | relative_url }}">View the Client Pitch milestone</a>
- <a href="{{ '/projects/' | relative_url }}">Back to Projects</a>
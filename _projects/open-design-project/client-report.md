---
layout: project
title: Client Report
description: Final client report for the Open Design Project
technologies: Mechanical Design, Prototyping, Testing, Bill of Materials
image: /assets/images/Lanternfly.png
permalink: /projects/open-design-project/client-report/
show_in_projects: false
---

<h1>Client Report</h1>

<p><strong>MAE 2250 – Introduction to Mechanical Design Spring 2026</strong></p>

<p><strong>Bug-anators</strong><br>
Albert Zheng, Gary Chau, Lisa Iizuka, Phillip Osadsky, & Yolanda Zhou</p>

<hr>

<h2>Context & Problem Statement</h2>

<p><strong>Specific Problem:</strong> During mechanical harvesting, up to ~60% of SLF present on vines are collected into grape bins, and even 1–2 insects in a 1000 g sample can cause an entire shipment to be rejected.</p>

<p><strong>Why it Matters:</strong> This leads to significant economic losses, reduced crop quality, and inefficiencies since mechanical systems do not allow for manual sorting. As SLF continues to spread, this issue will scale rapidly across vineyards.</p>

<p><strong>Constraints:</strong></p>
<ul>
  <li>Must work with mechanical harvesting systems (no interference)</li>
  <li>Must allow airflow and sunlight for plant health</li>
  <li>Must be scalable across vineyard rows</li>
  <li>Must be retractable for operational efficiency</li>
  <li>Must be structurally stable under outdoor conditions</li>
</ul>

<hr>

<h2>Final Prototype and Application</h2>

<p><strong>Prototype Overview:</strong> A retractable vineyard enclosure that expands to protect grapevines from SLF and contracts to allow harvesting operations.</p>

<p><strong>How it Works:</strong></p>
<ul>
  <li>A scissor linkage expands horizontally to form a frame</li>
  <li>Mesh stretches across the frame to create a barrier</li>
  <li>A wheel–rail system enables smooth expansion and retraction</li>
  <li>The system encloses vines during growth and retracts during harvest</li>
</ul>

<p><strong>Key Components:</strong></p>
<ul>
  <li>Scissor linkage (expandable structure)</li>
  <li>Mesh enclosure (physical barrier)</li>
  <li>Wheel–rail system (guided motion)</li>
  <li>Structural support frame</li>
  <li>Fasteners and joints</li>
</ul>

<p><strong>Application:</strong> Used in vineyards to prevent SLF contamination before harvest, reducing reliance on pesticides and eliminating the need for post-harvest sorting.</p>

<hr>

<h2>Conclusion and Recommendation</h2>

<p><strong>Recommendation:</strong> Proceed with further development of the retractable enclosure design, with targeted improvements. The current bill of materials (displayed below) reflects a low cost prototype using readily available components from limited options rather than optimized ones. The following test results indicate that future iterations will require a greater variety of plentiful stronger materials to choose from for low cost mass production in order to span a whole vineyard.</p>

<p><strong>Justification:</strong> The prototype successfully demonstrates a prevention-based solution that blocks SLF at the source while maintaining compatibility with harvesting operations.</p>

<p><strong>Based on testing results:</strong></p>
<ul>
  <li>Structural instability (tilting under load) needs improvement</li>
  <li>Wheel–rail misalignment caused jamming</li>
  <li>Fasteners loosened after repeated cycles</li>
</ul>

<p><strong>Feasibility:</strong> The concept is feasible as a scalable vineyard solution, but requires refinement in structural rigidity, alignment precision, and durability for real-world deployment.</p>

<p><strong>Next Steps:</strong></p>
<ul>
  <li>Reinforce the scissor linkage with stronger materials like Aluminum 6061</li>
  <li>Improve wheel–rail alignment tolerances</li>
  <li>Add locking mechanisms for fasteners</li>
  <li>Integrate motorized actuation for consistent operation</li>
  <li>Conduct field testing in real vineyard conditions</li>
</ul>

<hr>

<h2>Testing and Results</h2>

<h3>Test 1: Structural Stability (Scissor Linkage)</h3>

<p><strong>Purpose:</strong> Evaluate how the structure behaves under load</p>

<p><strong>Method:</strong> Added calibrated weights to the center of the linkage and measured the tilt angle</p>

<p><strong>Results:</strong></p>
<ul>
  <li>Tilt angle increased with increasing load initially</li>
  <li>After a certain weight threshold (~mid-range loads), the tilt began to plateau around ~10°</li>
  <li>Additional weight beyond this point did not significantly increase deformation</li>
</ul>

<p><strong>Implications:</strong></p>
<ul>
  <li>The structure exhibits limited stiffness, deforming quickly under initial loading</li>
  <li>The plateau suggests the system reaches a geometric or structural limit, where further deformation is constrained</li>
  <li>While deformation does not increase indefinitely, a ~10° tilt is still significant and may impact performance</li>
  <li>Indicates need for increased rigidity (stronger materials, bracing, or improved linkage design)</li>
</ul>

<h3>Test 2: Wheel–Rail Motion Performance</h3>

<p><strong>Purpose:</strong> Evaluate the reliability and smoothness of the wheel–rail system during repeated expansion and contraction cycles.</p>

<p><strong>Method:</strong> The prototype was run through 10 full expansion–contraction cycles. During each cycle, the number of jams (instances where motion was obstructed or stopped) was recorded.</p>

<p><strong>Results:</strong></p>
<ul>
  <li>Early cycles showed smooth motion with little to no jamming</li>
  <li>Later cycles exhibited increased jamming events</li>
  <li>The total number of jams increased as the cycle number increased</li>
</ul>

<p><strong>Implications:</strong></p>
<ul>
  <li>The system is initially functional, but loses reliability over repeated use</li>
  <li>Small misalignments in the wheel–rail system accumulate and lead to jamming</li>
  <li>Precise alignment and tighter tolerances are critical for consistent performance</li>
</ul>

<h3>Test 3: Fastener Reliability</h3>

<p><strong>Purpose:</strong> Assess the durability of fasteners under repeated expansion–contraction cycles.</p>

<p><strong>Method:</strong> After performing 10 full expansion–contraction cycles, all bolts and fasteners in the prototype were inspected. The number of loosened fasteners was recorded after each cycle.</p>

<p><strong>Results:</strong></p>
<ul>
  <li>Fasteners began to loosen after several cycles</li>
  <li>The number of loose fasteners increased over time</li>
  <li>By later cycles, multiple fasteners required retightening</li>
</ul>

<p><strong>Implications:</strong></p>
<ul>
  <li>Repeated motion and vibration lead to gradual fastener loosening</li>
  <li>The current fastening method is not sufficient for long-term durability</li>
  <li>Indicates a need for locking mechanisms (e.g., lock nuts, thread-locking compounds)</li>
</ul>

<hr>

<h2>Prototype and Testing Details</h2>

<p><strong>Design Details:</strong> The design uses a horizontally expanding scissor linkage system combined with a mesh barrier to create a retractable enclosure that surrounds grapevines while maintaining environmental exposure.</p>

<p><strong>Assembly Overview:</strong></p>
<ul>
  <li>Constructed a 4-bar scissor-linkage frame constrained to 1 DOF, ensuring the entire mechanism moves from a single input motion.</li>
  <li>Cut 80/20 extrusion channels to length using a bandsaw and connected them with L-brackets to form the rigid end frames.</li>
  <li>Pinned the top of the scissor linkage to the frame (fixed) while leaving the bottom free to translate, enabling linear extension and retraction.</li>
  <li>Fabricated a wheel-motor mount in CAD, assembled it under the free end of the frame, and powered the motor via a DC adaptor with alligator clips provided to us.</li>
  <li>Secured the insect mesh enclosure to the scissor linkage using zip ties along the aluminum frame.</li>
  <li>Mounted the full assembly onto an L-bracket rail system, allowing the system to roll along a fixed linear track.</li>
</ul>

<p><strong>Testing Setup:</strong> The prototype was tested using controlled, repeatable setups to evaluate structural stability, motion performance, and fastener reliability under conditions that simulate real operation.</p>

<p><strong>Test 1: Structural Stability (Scissor Linkage):</strong> The prototype was fully expanded and placed on a stable surface. Calibrated weights were incrementally added to the center of the scissor linkage to simulate loading conditions. At each load step, the tilt angle of the structure was measured relative to the horizontal to quantify deformation.</p>

<p><strong>Test 2: Wheel–Rail Motion Performance:</strong> The prototype was mounted on its rail system and manually operated through repeated expansion and contraction cycles. A total of 10 full cycles were performed. During each cycle, the system was observed for interruptions in motion, and any instances of jamming or resistance were recorded.</p>

<p><strong>Test 3: Fastener Reliability:</strong> Following the motion testing, all fasteners (bolts and joints) were inspected after each cycle. The number of loosened fasteners was recorded to evaluate how repeated motion and vibration affected connection integrity over time.</p>

<hr>

<h2>Bill Of Materials</h2>

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Part Number</th>
      <th>Quantity</th>
      <th>Cost</th>
      <th>Justification</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Collapsible Gates (Amazon)</td>
      <td>B08L5FQYHS</td>
      <td>2</td>
      <td>$46</td>
      <td>This part is mainly for the expandable and collapsible portion of the shaft, which is essential for the top-most portion of our design. It is also not on McMaster, where we are only able to source it from Amazon.</td>
    </tr>
    <tr>
      <td>Mesh (Amazon)</td>
      <td>B087RSWLY8</td>
      <td>1</td>
      <td>$8</td>
      <td>A mesh is also an important part of our design. It acts as the main protective layer against SLFs. However, McMaster only has extremely heavy meshes, which are not structurally good for our design purposes. We are also not able to make this in the TDS or by machining any parts, so the only way is to buy it from Amazon.</td>
    </tr>
    <tr>
      <td>Wheels (Amazon)</td>
      <td>B0FLX9WQBH</td>
      <td>2</td>
      <td>$37.16</td>
      <td>This part is used for the rolling motion of the mesh and structural components. Wheels from McMaster are incredibly expensive, which makes buying wheels from Amazon the only realistic option for our team.</td>
    </tr>
    <tr>
      <td>Motor (Amazon)</td>
      <td>B089GTHGPZ</td>
      <td>2</td>
      <td>$30</td>
      <td>This part is used for electrically powering our wheels. This allows us to automate our system. Motors from McMaster are incredibly clunky, heavy, costly, and the specs are too high for our use case. Amazon was the only reasonably priced option.</td>
    </tr>
    <tr>
      <td>80/20 extrusions (McMaster)</td>
      <td>47065T101</td>
      <td>2</td>
      <td>$66.50</td>
      <td>6 ft each</td>
    </tr>
    <tr>
      <td>U channels (McMaster)</td>
      <td>9001K787</td>
      <td>2</td>
      <td>$17.48</td>
      <td>4 ft each</td>
    </tr>
    <tr>
      <td>L brackets + more nuts (Amazon)</td>
      <td>B0855V2JV3</td>
      <td>1</td>
      <td>$18</td>
      <td>These L brackets are for securing our frames together. These brackets could be found on McMaster, but McMaster charges $8 for each bracket, which is ludicrously overpriced and would put us over budget.</td>
    </tr>
  </tbody>
</table>

<p><strong>Total Cost: $233</strong></p>

<hr>

<h2>Work Cited</h2>

<p>Bekelja, K. M. (2026). NY grapes and the spotted lanternfly problem. Cornell Integrated Pest Management</p>

<p>Phillips-Russo, J. (2026). Spotted lanternfly mechanical harvester study. Lake Erie Regional Grape Program</p>

<hr>

<p>
  <a href="{{ '/projects/OpenDesignProject/' | relative_url }}">Back to Open Design Project</a>
</p>
---
layout: project
title: MAE 3270 Final Project
description: Torque Wrench Analysis
technologies: [Autodesk Inventor, ANSYS, MATLAB]
image: /assets/images/torquewrenchcad.png
---

For MAE 3270, Mechanics of Materials, we have a final project where we have to work on designing a torque wrench. This means doing hand calcs, making a CAD, and doing ANSYS. 


![Torque Wrench CAD]({{ "/assets/images/torquewrenchcad.png" | relative_url }}){: style="width: 450px; display: block; margin: 1rem auto;"}




The torque-arm assembly consists of two primary components: a rectangular arm and a square-section knob. The arm dimensions are 0.3 inches by 0.6 inches in cross section with a length of 16 inches, while the knob measures 0.375 inches by 0.375 inches by 0.5 inches. These dimensions define the load path and establish the stiffness distribution used throughout the subsequent analysis.

Material: Low-alloy steel 4330V, quenched and tempered
- Young’s modulus: 229.75 × 10^6 psi
- Yield strength: 195 ksi
- Fracture toughness, K_IC: 90.95 ksi√in
- Fatigue strength at 10^6 cycles: 110 × 10^3 psi
- Ductile failure mode expected based on material selection

ANSYS setup diagram:
![ANSYS setup diagram]({{ "/assets/images/torquewrenchansyssetup.png" | relative_url }}){: style="width: 450px; display: block; margin: 1rem auto;"}



ANSYS Normal Strain Contours (in Strain Gauge Direction):
![ANSYS Normal Strain Contours (in Strain Gauge Direction)]({{ "/assets/images/torquewrenchstraincontours.png" | relative_url }}){: style="width: 450px; display: block; margin: 1rem auto;"}


ANSYS Maximum Principal Stress Contours:
![ANSYS Maximum Principal Stress Contours]({{ "/assets/images/torquewrenchstresscontours.png" | relative_url }}){: style="width: 450px; display: block; margin: 1rem auto;"}

Maximum Normal Stress: 77.360 ksi at knob. 32.5 ksi in bar <br>
Strain @ Strain Gauge: 1053 µε <br>
Deflection @ Load Point: .37224'' <br>
<br>
Torque wrench sensitivity in mV/V using strains: 1.05 mV/V <br>

For this torque wrench design, I selected a foil strain gauge (OMEGA SGD‑1‑5‑120‑LY11) to measure strain on the rectangular arm. The gauge measures 0.5 inches long by 0.125 inches wide, which provides adequate coverage along the 0.6-inch width of the arm while leaving sufficient space for proper adhesive bonding. The gauge is mounted along the length of the arm to capture bending strains in the primary load path. To ensure reliable attachment and accurate strain readings, the gauge is bonded to the steel surface using OMEGA SG496 cold-curing strain-gage adhesive, which offers strong adhesion and minimal creep under load. 


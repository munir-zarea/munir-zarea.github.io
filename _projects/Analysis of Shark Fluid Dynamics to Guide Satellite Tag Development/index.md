---
layout: post
title: Hydrodynamic Analysis of Sharks to Guide Satellite Tag Design
description: In this project, completed as part of my undergraduate capstone at Oregon State University, I analyzed the hydrodynamic impact of satellite telemetry tags on sharks. Using CFD modeling and wind tunnel validation, the team and I developed a repeatable methodology to evaluate tag-induced drag and lift across different shark species.

skills: 
- CFD
- CAD
- 3D Printing
- Experimental Design
- Data Analysis
- Technical Writing

main-image: /assets/images/profile-image/Hammerhead in Wind Tunnel.jpg
---

## Tools Used
- **CFD Software:** STAR-CCM+
- **Modeling/Prep:** Blender, SolidWorks, Fusion 360
- **Experimental Setup:** Arduino Nano, Strain Gauges
- **Fabrication:** Ultimaker S5 (ABS), HP MJF (PA12)
- **Data Analysis:** MATLAB, Excel

---

## Project Goals
- Understand the hydrodynamic impact of telemetry tags on sharks.
- Use CFD and wind tunnel testing to estimate lift and drag forces.
- Validate computational models using physical prototypes.
- Provide a method for optimizing tag design.

---

## Methodology

### Computational Fluid Dynamics (CFD)
- 3D shark models obtained via photogrammetry.
- Simulated in STAR-CCM+ with SST k-ω turbulence model.
- Tested at 3 angles of attack: −12°, 0°, +12°.
- Lift and drag coefficients computed and visualized.

{% include image-gallery.html 
  images="/assets/images/profile-image/GeneralMethodologyFlowchart.jpeg, /assets/images/profile-image/CFD Mesh Generation.jpg" 
  height="300" 
  caption="Left: General methodology flowchart combining CFD and wind tunnel validation. Right: CFD mesh of blacktip reef shark model." 
%}

---

### Wind Tunnel Testing
- 3D-printed shark models (ABS and Nylon PA12).
- Force balance system connected to Arduino.
- Reynolds number matched CFD scenarios for validation.
- Calibration and mounting setup shown below:

{% include image-gallery.html 
  images="/assets/images/profile-image/Calibration Method.jpg, /assets/images/profile-image/Aluminum Sleeve.jpg" 
  height="300" 
  caption="Left: Calibration method using suspended weights. Right: Machined aluminum sleeve used for secure mounting in the wind tunnel." 
%}

<div style="text-align: center;">
  {% include image-gallery.html 
    images="/assets/images/profile-image/Hammerhead in Wind Tunnel.jpg" 
    height="300" 
    caption="3D printed hammerhead shark mounted in wind tunnel at 0° angle of attack." 
  %}
</div>

---

## Results

### Global Trends Across Species

{% include image-gallery.html 
  images="/assets/images/profile-image/Angle of Attack vs Drag Coefficient.jpg, /assets/images/profile-image/Frontal Area vs Drag Coefficient.jpg" 
  height="300" 
  caption="Left: Drag coefficient vs angle of attack for each species. Right: Drag coefficient vs frontal area for each shark." 
%}

{% include image-gallery.html 
  images="/assets/images/profile-image/Reynolds Number vs Drag Coefficient.jpg" 
  height="300" 
  caption="Validation of wind tunnel accuracy with CFD comparison for a standard sphere at various Reynolds numbers." 
%}

---

### Shark-Specific Results

{% include image-gallery.html 
  images="/assets/images/profile-image/Blacktip Results.jpg, /assets/images/profile-image/Mako Results.jpg" 
  height="250" 
  caption="Left: Results for Blacktip Reef Shark. Right: Results for Shortfin Mako Shark." 
%}

{% include image-gallery.html 
  images="/assets/images/profile-image/Caribbean Results.jpg, /assets/images/profile-image/Hammerhead Results.jpg" 
  height="250" 
  caption="Left: Results for Caribbean Reef Shark. Right: Results for Great Hammerhead Shark." 
%}

---

## Digital Modeling

### Shark Species Modeled
- Shortfin Mako (*Isurus oxyrinchus*)
- Caribbean Reef (*Carcharhinus perezii*)
- Blacktip Reef (*Carcharhinus limbatus*)
- Great Hammerhead (*Sphyrna mokarran*)

Photogrammetric 3D models were sourced from **DigitalLife3D**, processed for STAR-CCM+ simulation and 3D printing.

{% include image-gallery.html 
  images="/assets/images/profile-image/nemesis-3d-model-mesh.jpg" 
  height="300" 
  caption="Example of a high-resolution photogrammetric shark mesh prepared for CFD and fabrication." 
%}

---

## Key Findings
- Lift coefficients ranged from **−0.02 to 0.37**.
- Drag coefficients ranged from **0.14 to 0.21**.
- CFD models matched wind tunnel results within **<10% error**.
- Surface finish (ABS vs PA12) had **negligible impact**.
- **Shortfin Mako** had the lowest drag; **Great Hammerhead** had higher lift due to cephalofoil geometry.

---

## Reflection

This project brought together mechanical design, marine biology, and computational physics to solve a real conservation-driven engineering challenge. It provided hands-on experience with CAD modeling, CFD validation, and experimental methods. I'm proud to have contributed to a methodology that may support future biologging innovations.

---

## Improvements and Future Work
- Attach tag models to shark geometries and run new simulations.
- Incorporate dynamic (unsteady) flow modeling to capture fin/body flexion.
- Apply transition models (e.g., Gamma-Re-Theta) to improve turbulence resolution.
- Explore riblet surfaces or coatings inspired by shark skin to reduce drag on tags.

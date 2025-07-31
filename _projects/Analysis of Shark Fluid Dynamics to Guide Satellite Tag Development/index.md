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

### 📌 Computational Fluid Dynamics (CFD)
- 3D shark models obtained via photogrammetry.
- Simulated in STAR-CCM+ with SST k-ω turbulence model.
- Tested at 3 angles of attack: −12°, 0°, +12°.
- Lift and drag coefficients computed and visualized.

{% include image-gallery.html images="/assets/images/profile-image/GeneralMethodologyFlowchart.jpg" height="300" caption="General methodology flowchart for CFD and wind tunnel validation." %}
{% include image-gallery.html images="/assets/images/profile-image/nemesis-3d-model-mesh.jpg" height="300" caption="Photogrammetry-based 3D shark mesh imported into CFD software." %}
{% include image-gallery.html images="/assets/images/profile-image/CFD Mesh Generation.jpg" height="300" caption="Polyhedral mesh generated in STAR-CCM+ for blacktip reef shark." %}

---

### 📌 Wind Tunnel Testing
- 3D-printed shark models (ABS and Nylon PA12).
- Calibrated force balance system connected to Arduino.
- Reynolds number matched CFD scenarios for validation.
- Calibration and mounting setup shown below:

{% include image-gallery.html images="/assets/images/profile-image/Calibration Method.jpg" height="300" caption="3D-printed sleeve calibration system for force balance." %}
{% include image-gallery.html images="/assets/images/profile-image/Aluminum Sleeve.jpg" height="300" caption="Machined aluminum sleeve with set screw for wind tunnel mounting." %}
{% include image-gallery.html images="/assets/images/profile-image/Hammerhead in Wind Tunnel.jpg" height="300" caption="Great hammerhead shark model positioned for wind tunnel testing." %}

---

## Results

### 📈 Drag and Lift Coefficient Trends
{% include image-gallery.html images="/assets/images/profile-image/Angle of Attack vs Drag Coefficient.jpg" height="300" caption="Drag coefficient vs. angle of attack for each shark species (CFD results)." %}
{% include image-gallery.html images="/assets/images/profile-image/Frontal Area vs Drag Coefficient.jpg" height="300" caption="Drag coefficient vs. frontal area of shark models." %}
{% include image-gallery.html images="/assets/images/profile-image/Reynolds Number vs Drag Coefficient.jpg" height="300" caption="Comparison of CFD and wind tunnel results on a reference sphere across Reynolds numbers." %}

---

### 🦈 Shark-Specific Results

{% include image-gallery.html images="/assets/images/profile-image/Blacktip Results.jpg" height="250" caption="CFD and wind tunnel results for Blacktip Reef Shark." %}
{% include image-gallery.html images="/assets/images/profile-image/Mako Results.jpg" height="250" caption="CFD and wind tunnel results for Shortfin Mako Shark." %}
{% include image-gallery.html images="/assets/images/profile-image/Caribbean Results.jpg" height="250" caption="CFD and wind tunnel results for Caribbean Reef Shark." %}
{% include image-gallery.html images="/assets/images/profile-image/Hammerhead Results.jpg" height="250" caption="CFD and wind tunnel results for Great Hammerhead Shark." %}

---

## Digital Modeling

### Shark Species Modeled
- Shortfin Mako (*Isurus oxyrinchus*)
- Caribbean Reef (*Carcharhinus perezii*)
- Blacktip Reef (*Carcharhinus limbatus*)
- Great Hammerhead (*Sphyrna mokarran*)

We used photogrammetric 3D models from **DigitalLife3D**, prepared for both 3D printing and CFD simulation.

{% include image-gallery.html images="/assets/images/profile-image/nemesis-3d-model-mesh.jpg" height="300" caption="Example photogrammetry mesh used for modeling." %}

---

## Reflection

This project highlighted the real-world value of combining computational analysis with physical experimentation. The interdisciplinary work — spanning marine biology, fluid mechanics, CAD modeling, and fabrication — helped prepare me for further work in marine robotics and hydrodynamics.

---

## Future Improvements

- Add satellite tag models to shark meshes and re-run CFD/wind tunnel trials.
- Explore dynamic (unsteady) fluid simulation.
- Refine mesh for turbulence transition modeling.
- Incorporate drag reduction strategies from nature (riblets, coatings, etc.).


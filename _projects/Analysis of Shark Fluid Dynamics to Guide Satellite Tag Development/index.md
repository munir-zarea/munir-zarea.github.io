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
  
main-image: /Hammerhead in Wind Tunnel.jpg 
---

## Tools Used
- CFD Software: STAR-CCM+
- Modeling/Prep: Blender, SolidWorks, Fusion 360
- Experimental Setup: Arduino Nano, Strain Guages
- Fabrication: Ultimaker S5 (ABS), HP MJF (PA12)
- Data Analysis: MATLAB, Excel

## Project Goals
- Understand the hydrodynamic impact of telemetry tags on sharks.
- Use CFD and wind tunnel testing to estimate lift and drag forces.
- Validate computational models using physical prototypes.
- Provide a method for optimizing tag design.

## Methodology
### Computational Fluid Dynamics (CFD)
- 3D shark models obtained via photogrammetry.
- Simulated in STAR-CCM+ with SST k-&omega turbulence model.
- Tested at 3 angles of attack: -12 degrees, 0 degrees, and +12 degrees.
- Lift and drag coefficients computed and visualized.

{% include image-gallery.html images="/assets/images/profile-image/GeneralMethodologyFlowchart.jpeg" height="100"%}
{% include image-gallery.html images="/assets/images/profile-image/nemesis-3d-model-mesh.jpg" height="100"%} 
{% include image-gallery.html images="/assets/images/profile-image/Blacktip Results.jpg" height="100"%} 

### Wind Tunnel Testing
- 3D-printed shark models (ABS and Nylon PA12).
- Force balance system connected to Arduino for live data.
- Matched Reynolds number with CFD for validation.
- Conducted calibration and error analysis.
{% include image-gallery.html images="/assets/images/profile-image/Calibration Method.jpg" height="100"%}
{% include image-gallery.html images="/assets/images/profile-image/Aluminum Sleeve.jpg" height="100"%} 

## Key Findings 
- Lift coefficients ranged: -0.02 to 0.37.
- Drag coefficients ranged: 0.14 to 0.21.
- CFD generally matched wind tunnel data within acceptable error (<10%).
- Surface finish (ABS vs Nylon) had negligible impact.
- Shortfin mako had lowest drag, hammerhead had higher lift.

## Project Workflow
{% include image-gallery.html images="/assets/images/profile-image/GeneralMethodologyFlowchart.jpeg" height="400"%} 

### Digital Modeling
#### Four shark species were selected:
- Shortfin Mako
- Caribbean Reef
- Blacktip Reef
- Great Hammerhead


- We used photogrammetric 3D models of each shark provided to us from DigitalLife3D. These models were both prepared for 3D printing and STAR-CCM+.

{% include image-gallery.html images="/assets/images/profile-image/nemesis-3d-model-mesh.jpg" height="400"%} 

## Wind Tunnel Testing


## Results

## Reflection

## Improvements



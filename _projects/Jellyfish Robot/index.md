---
layout: post
title: Stiffness- and Buoyancy-Tunable Underwater Manipulator
description: 
  In this project, completed as part of my graduate research at the University of Hawaiʻi at Mānoa, I designed and built a bio-inspired underwater robotic manipulator that combines stiffness tuning, buoyancy-driven orientation control, and a detachable end effector for manipulation in fragile, confined, and hard-to-reach environments. Inspired by jellyfish and octopus-like locomotion and manipulation strategies, the system was developed as a soft robotic platform for underwater grasping tasks that conventional rigid manipulators struggle to perform. The work includes mechanical design, soft actuator fabrication, prototyping, experimental validation, and robotic control development, and was prepared for submission to IROS 2026.

paper:
  title: Stiffness- and Buoyancy-Tunable Underwater Object Manipulation with a Detachable End Effector
  url: /assets/pdfs/IROS_2026_manuscript.pdf

skills:
- Soft Robotics
- Mechanical Design
- Prototyping
- ROS 2
- Pneumatic Actuation
- Experimental Validation
- CAD
- 3D Printing
- System Integration
- Technical Writing

main-image: /assets/images/profile-image/jellyfish_robot_overview.jpg
---

## Tools Used
- **CAD / Mechanical Design:** SolidWorks, Onshape
- **Fabrication:** Bambu Lab X1 Carbon, resin printing, heat sealing, laser-cut / hand-cut flexible films
- **Materials:** Mylar PET films, TPU components, sandpaper jamming layers, flexible tubing
- **Controls / Software:** ROS 2, Python, joystick-based actuation control
- **Embedded / Hardware Integration:** Servo-actuated syringe pumps, pneumatic routing, external actuation architecture
- **Data Analysis / Modeling:** MATLAB, quasi-static stiffness modeling, experimental load testing

## Project Goals
- Develop an underwater manipulator capable of safely grasping fragile objects.
- Enable variable stiffness so the gripper can switch between compliant and load-bearing modes.
- Use buoyancy modulation to reorient the end effector without relying on thrusters.
- Expand access to confined and hard-to-reach spaces through a detachable end effector.
- Validate the system through underwater manipulation demonstrations and stiffness experiments.

---

## Project Overview

This project focused on designing a multifunctional underwater soft robotic manipulator for delicate interaction in marine environments. The system combines three core capabilities: a tendon-driven continuum arm for positioning, buoyancy-tunable pouches for smooth underwater orientation, and a stiffness-tunable soft gripper that can transition between gentle grasping and more stable load-bearing behavior. The end effector can also detach from the arm and operate independently, allowing manipulation in areas that are difficult to access with conventional arm-constrained systems. :contentReference[oaicite:2]{index=2}

Unlike traditional rigid underwater manipulators, this platform was designed around compliance, modularity, and mechanical adaptability. The goal was not just to build a novel prototype, but to create and experimentally validate a system architecture that could support future underwater inspection, environmental interaction, and object retrieval tasks in cluttered or fragile environments. :contentReference[oaicite:3]{index=3}

---

## System Architecture

### Continuum Arm
The manipulator includes a tendon-driven soft continuum arm inspired by octopus locomotion and reach. The arm is composed of 36 segmented elements, allowing smooth bending and omnidirectional positioning while maintaining structural compliance. Tendons were routed through each segment, and the distal interface was designed to support both fixed and rotatable end-effector configurations. This subsystem served as the primary positioning mechanism for arm-attached operation. :contentReference[oaicite:4]{index=4}

### Buoyancy-Controlled Main Body
The central body integrates multiple buoyancy-tunable pouches arranged symmetrically around a rigid core. By selectively inflating individual pouches, the system can generate controlled reorientation of the end effector with minimal hydrodynamic disturbance. This provided a low-energy alternative to thruster-based orientation control and enabled smooth underwater rotation of the manipulator in multiple directions. :contentReference[oaicite:5]{index=5}

### Stiffness-Tunable End Effector
The gripper was built around a pouch-driven soft bending actuator combined with a vacuum-activated layer-jamming mechanism. In its compliant state, the gripper conforms passively to object geometry for safer interaction. When vacuum is applied to the jamming layer, internal friction increases and the actuator becomes significantly stiffer, improving grasp stability during transport or under disturbance. The end effector also included propulsion flaps to help with retrieval in detached operation. :contentReference[oaicite:6]{index=6}

---

## Fabrication and Prototyping

A major part of this project involved hands-on fabrication and iterative prototyping. The rigid structural components, including the arm segments and central body, were manufactured through 3D printing. Flexible buoyancy and bending pouches were fabricated from heat-sealed Mylar PET films, while the variable-stiffness layer used sandpaper-based laminar jamming sealed within a dedicated vacuum pouch. This combination of rigid and soft fabrication methods allowed rapid iteration while maintaining a compact and modular underwater design. :contentReference[oaicite:7]{index=7}

The design process required balancing manufacturability, routing complexity, waterproofing, and mechanical performance. Pneumatic lines were distributed through the central hub to reduce clutter and avoid interference with grasped objects. The layered actuator architecture was designed so that bending and stiffening could be actuated independently, which made the system more modular and easier to test experimentally. :contentReference[oaicite:8]{index=8}

---

## Controls and Coding

On the controls side, I developed the robotic actuation architecture needed to independently command bending, stiffness tuning, buoyancy modulation, and propulsion behaviors. The system used an external pneumatic actuation setup with servo-driven syringe mechanisms and flexible tubing to supply and regulate different channels. This work involved coordinating multiple subsystems rather than treating the robot as a single actuator. :contentReference[oaicite:9]{index=9}

I also worked on the software side of the platform, using ROS 2 and custom control logic to interface with the actuation system during experimental testing and demonstrations. This included subsystem-level command structure, manual control workflows, and integration between mechanical hardware and robotic software. From a job perspective, this project reflects full-stack prototype development: mechanical design, fabrication, hardware integration, and controls implementation within one robotic platform.

---

## Modeling and Experimental Validation

To quantify how stiffness tuning affected gripper behavior, I developed a quasi-static modeling framework for the end effector and performed load-based experiments to identify pressure-dependent bending stiffness. Midpoint loading experiments were used to isolate the jamming layer response, and the identified stiffness function was then used to predict deformation under both midpoint and distal loading cases. The results showed that increasing vacuum pressure increased effective stiffness and reduced deformation under load. :contentReference[oaicite:10]{index=10}

This modeling and validation effort was important because it moved the work beyond a proof-of-concept prototype. It established a measurable relationship between actuation input and mechanical response, and showed that the system’s stiffening behavior could be experimentally characterized and used for predictive analysis. :contentReference[oaicite:11]{index=11}

---

## Demonstrations

### Buoyancy-Driven Orientation
Underwater demonstrations showed that the end effector could be reoriented through controlled actuation of buoyancy pouches, achieving smooth rotation without continuous thruster input. This highlighted the potential of buoyancy-based control for delicate underwater interaction tasks. :contentReference[oaicite:12]{index=12}

### Arm-Attached Manipulation
In arm-attached mode, the manipulator used the continuum arm for positioning while the end effector reoriented locally. This reduced the need for large arm motions and improved accessibility in cluttered environments. :contentReference[oaicite:13]{index=13}

### Arm-Detached Manipulation
One of the most distinctive features of the project was the detachable end effector. In detached mode, the end effector operated independently using buoyancy and propulsion, allowing it to access confined regions and perform deep grasping tasks that would be difficult for a conventional rigid arm. :contentReference[oaicite:14]{index=14}

### Stiffness-Enhanced Grasping
Grasping demonstrations compared compliant and stiffened modes during underwater manipulation. In the stiffened condition, the gripper better maintained object stability under motion and external disturbance, showing the practical value of tunable stiffness for underwater handling tasks. :contentReference[oaicite:15]{index=15}

---

## Key Outcomes
- Designed and built a multi-unit underwater robotic manipulation platform combining continuum positioning, buoyancy control, and variable stiffness. :contentReference[oaicite:16]{index=16}
- Developed a detachable end effector concept for manipulation in confined and hard-to-reach underwater spaces. :contentReference[oaicite:17]{index=17}
- Demonstrated stiffness change of more than 2× through layer-jamming activation. :contentReference[oaicite:18]{index=18}
- Achieved buoyancy-driven reorientation up to approximately ±180°. :contentReference[oaicite:19]{index=19}
- Built and experimentally validated a pressure-dependent stiffness model for the gripper actuator. :contentReference[oaicite:20]{index=20}
- Integrated mechanical design, soft actuator fabrication, experimental testing, and robotic controls into one working prototype.

---

## Reflection

This project represents the kind of engineering work I enjoy most: taking an idea from concept to hardware, solving fabrication and integration problems along the way, and validating the final system experimentally. It required me to work across CAD, soft actuator fabrication, underwater prototyping, mechanical modeling, and robotic control development. More than anything, it reflects my interest in underwater robotic systems that are not only functional, but thoughtfully designed for real interaction in difficult environments.

---

## Improvements and Future Work
- Integrate onboard sensing for closed-loop pose and grasp control.
- Replace bulky offboard actuation hardware with more compact deployable systems.
- Improve autonomy for detached end-effector navigation and retrieval.
- Expand testing into open-water or field-relevant underwater environments.
- Incorporate perception and tactile sensing for more robust object interaction. :contentReference[oaicite:21]{index=21}

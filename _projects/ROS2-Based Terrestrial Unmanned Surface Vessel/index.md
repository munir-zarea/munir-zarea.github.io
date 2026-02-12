---
layout: post
title: ROS2-Based Terrestrial Unmanned Surface Vessel
description:  As part of a project at the University of Hawaii at Manoa, my team and I developed a mobile terrestrial robot that mimics the planar motion dynamics of an Unmanned Surface Vessel (USV). Ultimately intended as a platform for future marine robotics students, the project involved the complete design, prototyping, fabrication, and implementation of the robot. I was responsible for ROS2 integration, software architecture, and testing. This page will discuss the design process for the robot and outline my key contributions throughout the project.

skills: 
- ROS 2
- Gazebo
main-image: /assets/images/profile-image/USV_Overall_Picture.png 
---

## Key Features
- 3-DOF planar motion (surge, sway, yaw)
- Dual ducted fan propulsion
- Untethered operation using LiPo batteries
- Bluetooth joystick control
- ROS 2 (Jazzy) integration for sensor streaming and control
- IMU-based state estimation, with Kalman filter (kinda)
- Modular, 3D printed chassis

## Design & Build
We started by designing a compact, modular platform that could house all electronics and withstand repeated use in a classroom.

{% include image-gallery.html 
  images="/assets/images/profile-image/GeneralMethodologyFlowchart.jpeg, /assets/images/profile-image/CFD_Mesh_Generation.jpg" 
  height="200" 
  caption="Left: General methodology flowchart combining CFD and wind tunnel validation. Right: CFD mesh of blacktip reef shark model." 
%}

Our goals:
- Simple mechanical design (3D printed parts)
- Dual ducted fans with independent speed control
- Untethered operation using LiPo batteries

{% include image-gallery.html 
  images="/assets/images/profile-image/GeneralMethodologyFlowchart.jpeg, /assets/images/profile-image/CFD_Mesh_Generation.jpg" 
  height="200" 
  caption="The vehicle uses two ducted fans mounted side-by-side, creating forward and lateral motion through differential thrust. Four caster wheels support the platform while minimizing ground friction." 
%}

## Motivation, Objectives, and Design

To replicate USV-like motion, caster wheels were chosen. This allowed for motion on a 2D plane with 3 DOF. For propulsion, ducted fans, used for remote controlled planes, were used along with an Electronic Speed Controller (ESC). 

## ROS2 Integration





## Challenges and Future Directions
- Attempted Kalman Filter

## Acknowledgments
Special thanks to Rex Imanaka, Jason Kanemoto, and Kurt Metrose for their collaboration on this project.





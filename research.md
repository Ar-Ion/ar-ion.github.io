---
layout: page
title: Research
permalink: /research/
---

My research focuses on advancing the state-of-the-art in autonomous systems, with particular emphasis on perception, localization, and motion planning for aerospace and robotics applications. I also have extensive experience in hardware prototyping and have pursued research on power system designs, optimizing for efficiency, throughput, bandwidth, and resilience.

## Perception & State Estimation

### Optimal Representation of Stochastic Processes (2025)
**Supervisor**: Prof. Soon-Jo Chung (Caltech)

Exploiting the structure of the time evolution of non-stationary probability distributions to represent the history of a stochastic process using finite-dimensional basis functions. Applications range from sensor noise characterization to financial market prediction.

### Autonomous Race Car Localization (2025)
**Supervisor**: Prof. Soon-Jo Chung (Caltech)

Extended MINS for real-time racecar applications with multi-threading support and prior LiDAR-map registration. Incorporating vehicle dynamics and custom sensor modeling for the wheel odometry and steering actuator.
Extended GLIM for offline mapping of the racetrack and added support for RTK GPS in the factor graph optimization.

![Laguna Seca LiDAR Map](../assets/images/lidar-map.png)

<div align="center" style="margin-bottom: 1em;">
<i>Race track map of Laguna Seca in Monterey in preparation for the Monterey Grand Prix 2025</i>
</div>

### Autonomous Race Car Perception (2024-2025)
**Supervisor**: Prof. Soon-Jo Chung (Caltech)

Designed the modular perception subsystem of Caltech Racer to track competing race cars using LiDARs and additional sensors. Modules were designed to work on either CPU with OpenMP support or GPU. Individual state estimates are cross-checked with chi-squared tests and incorporated into an EKF with feed-forward accelerations derived from an inferred trajectory.

### Pose Estimation of Unknown Tumbling Bodies (2024)
**Supervisor**: Prof. Soon-Jo Chung (Caltech) & Prof. Colin Jones (EPFL)

**Paper**: International Aeronautical Congress 2024, Milan. [Link](https://www.arxiv.org/abs/2508.03132) 

**Slides**: [Link](../assets/docs/coffee-slides.pdf) 

**Report**: [Link](../assets/docs/coffee-report.pdf) 

**Main repository**: [Link](https://github.com/Ar-Ion/AsteroidEstimation) 

**Simulator repository**: [Link](https://github.com/Ar-Ion/AsteroidSimulation) 

Master's Thesis. Investigated novel approaches for estimating the motion of unknown tumbling objects in space environments under challenging lighting conditions. This work has direct applications for:
- Autonomous space debris removal missions
- Satellite servicing operations
- Asteroid proximity operations
- Robotic capture of non-cooperative objects

Developed shadow-invariant sparse feature extraction method using sun phase angle prior.
Designed a neural network architecture with multiple ResNet layers of Sparse Submanifold CNNs and LightGlue-based feature matching.

![Asteroid Pose Estimation](../assets/images/asteroid.gif)

<div align="center" style="margin-bottom: 1em;">
<i>Pose estimation of a tumbling asteroid using visual features and motion tracking</i>
</div>

### Angle-of-Arrival Localization for Space Applications (2022-2023)
**Supervisor**: Prof. Andreas Burg (EPFL) & Prof. Jean-Paul Kneib (EPFL)

**Report**: [Link](../assets/docs/spaceloc-report.pdf) 

Developed a novel localization strategy using rotating high-bandwidth signals to generate a Doppler effect synchronous with the angle of arrival of the signal. This effect could then be used to estimate the relative angle between the mobile robot and the rotating source in a Maximum Likelihood framework, with minimal degradation from multipath effects. Multiple independent measurements of AoA could then be used to infer the position of the mobile robot.

## Power Systems

As part of my EE major, I spent significant time designing power supplies for EPFL Xplore's rovers and drones. The following sections highlight my research on these power systems.

### Pollux III (2023)

**Documentation**: [Link](../assets/docs/pollux-iii-ref.pdf) 

**Printable design files**: [Link](../assets/docs/pollux-iii-printable.pdf) 

**Design files**: [Link](../assets/archives/pollux-iii-design.zip) 

**Simulation files**: [Link](../assets/archives/pollux-iii-sim.zip) 

**Mission report (ERC 2023)**: [Link](../assets/docs/pollux-iii-output.pdf) 

Designed, implemented, and tested a fully-redundant high-throughput power supply. It features four 15A programmable channels in either synchronous buck or buck-boost configuration. Each channel is parallelizable and redundant, with automatic fallback. All channels are monitored independently, and real-time data is reported through a touchscreen and a web app accessible from a wireless hotspot. Data is logged at a programmable rate on internal flash memory and is available for download from a dedicated CLI.

<div align="center">
<img src="../assets/images/polluxiii.png" alt="Pollux III" width="500">
</div>

### Drone Power Supply (2023)

Designed, implemented, and tested a highly compact 35mm 2-channel 200W power module for an autonomous 7-inch drone.

<div align="center">
<img src="../assets/images/droneps.png" alt="Drone Power Supply">
</div>

### Pollux II (2022)

**Design files**: [Link](../assets/archives/pollux-ii-design.zip) 

**Simulation files**: [Link](../assets/archives/pollux-ii-sim.zip) 

Designed, implemented, and tested a high-throughput power system, driving 8 BLDC motors and switching up to 1kW of power.

<div align="center">
<iframe width="560" height="315" src="https://www.youtube.com/embed/cOQ0CWVfOLc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</div>

### Pollux I (2021)
**Supervisor**: Prof. Drazen Dujic

**Specifications**: [Link](../assets/docs/pollux-i-specs.pdf) 

**Report**: [Link](../assets/docs/pollux-i-report.pdf) 

**Design files**: [Link](../assets/archives/pollux-i-design.zip) 

**Simulation files**: [Link](../assets/archives/pollux-i-sim.zip) 

Designed, implemented, and tested a highly efficient 4-channel power supply for the EPFL Xplore rover.

<div align="center">
<iframe width="560" height="315" src="https://www.youtube.com/embed/MzJ2GEuEaqA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</div>

## Research Interests & Future Directions

### Space Robotics & Autonomous Systems
- **On-orbit servicing**: Autonomous manipulation of satellites and space debris
- **Planetary exploration**: Advanced navigation and science autonomy for rovers
- **Formation flying**: Coordinated control of multiple spacecraft

### Perception & State Estimation
- **Multi-modal sensor fusion**: Combining vision, LiDAR, radar, and inertial sensors
- **Robust estimation**: Algorithms that maintain performance under sensor failures
- **Factor graph optimization**: Efficient algorithms for large-scale SLAM problems

### Real-time Embedded Systems
- **Low-latency control**: Sub-millisecond control loops for critical applications
- **Fault-tolerant architectures**: Systems that gracefully handle component failures
- **Edge computing**: Efficient deployment of AI algorithms on resource-constrained platforms
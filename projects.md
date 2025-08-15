---
layout: page
title: Projects
permalink: /projects/
---

A showcase of my major robotics, aerospace, and software engineering projects.

## Robotics Projects

### Caltech Racer Autonomous Race Car (2025)
*Research Engineer*

High-speed autonomous racing on controlled environments (race tracks) and active participation in the Indie Autonomous Challenge international competition.

<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; margin: 1.5rem 0;">
  <iframe src="https://www.youtube.com/embed/v10TQy46cms" 
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" 
          frameborder="0" allowfullscreen></iframe>
</div>

**Highlights**: 
- Fully autonomous race car, able to overtake and make decisions in real time
- Speeds up to 300km/h, accelerations up to 1.5g
- Sensor suite consisting of 3 LiDARs, 6 cameras, 3 IMUs, 2 RTK GPS, 2 Radars, 4 wheel odometry sensors
- Non-linear controller, MPC, and offline global optimizer for motion planning
- LiDAR-based and YOLO competitor car detection and tracking
- Exciting SOTA research coming soon (ICRA'26)

**Achievements**: 
- Third fastest lap time at the Laguna Seca Indie Autonomous Challenge competition (before spinning out 🙊)

**Contributions (perception)**:
- Complete LiDAR-based perception stack to detect competing cars
- Modular C++ framework to accomodate other modalities for competitor car detection
- EKF with feed-forward accelerations inferred from an assumed global trajectory of the competing cars
- Testing and benchmarking suite to validate the perception stack
- Consolidated multi-car dataset with camera, lidar and groud-truth data.

**Contributions (localization)**:
- Mapping framework to generate LiDAR maps of racetracks
- Extended MSCKF state to include higher fidelity sensor measurement models
- Extended MINS with multi-threading capabilities
- Sensor calibration and low-level system tuning

**Technologies**: C++, ROS2, PCL, CUDA, GNN, YOLO, ICP, OpenMP, EKF, MSCKF

### EPFL Xplore Rovers (2020-2023)
*Founder, Project Manager, Systems Engineer*

Led a team of more than 60 students to develop autonomous rovers for the European Rover Challenge over three years, achieving multiple podium finishes and special recognition awards.

<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; margin: 1.5rem 0;">
  <iframe src="https://www.youtube.com/embed/UUAIprJ8epM" 
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" 
          frameborder="0" allowfullscreen></iframe>
</div>

**Highlights**:
- 60kg versatile rover participating yearly in the European Rover Challenge
- Full in-house structure, mechanisms, electronics and software stack
- Complete mission autonomy
- Perception system enabling autonomous navigation in challenging terrains
- Scientific analysis payload with chemical compounds sensor, raman spectrometry, camera-based sample statistics for complex scientific tasks
- 6DoF integrated robotic arm for complex manipulation tasks
- Rocker-differential 4-wheeled structure for a facilitated navigation in rough terrains
- Fully redundant power management system and avionics

**Achievements**:
- 3rd place at ERC2023 World Finals with special award for best robotic arm and best presentation
- 2nd place at ERC2022 World Finals with special award for best autonomous navigation
- 3rd place at ERC2021 World Finals with special award for best science plan and best sample probing

**Contributions (as co-founder)**:
- Sharing vision on the importance of robotics and space exploration
- Sharing vision on the importance of hands-on projects for EPFL students
- Fundraising ($150K per year)
- Interfacing project with stakeholders
- Organize / participate in events
- Deliverable consolidation for stakeholders and competiton committee

**Contributions (as electronics systems engineer)**:
- Requirements definition
- Initial electronics architecture
- Power system architecture
- Power and energy budget allocation
- Sensor selection
- Assembly, Integration & Testing planning
- ConOps definition

**Contributions (as software systems engineer)**:
- Requirements definition
- Initial software architecture
- Embedded software firmware and sensor acquisition
- Custom communication protocol ([Link](#roco-communication-protocol-2020))
- Networking with EtherCAT and PoE
- Part of the autonomous navigation stack (pointcloud segmentation and obstacle detection)
- Part of the navigation kinematics model
- Assembly, Integration & Testing planning
- ConOps definition

**Contributions (as project manager)**:
- Budget management
- Timeline management
- Risk management
- Sprints/PDR/CDR organization

**Contributions (as power system designer)**: [Link](/research/#power-systems)

**Contributions (as drone systems engineer)**: [Link](#epfl-xplore-drone-2023)

**Technologies**: ROS, ROS2, Altium, LTSpice, LTPowerCAD, Fusion 360, C, C++, PCL, LIO-SAM, Kinematics, Nvidia Jetson Xavier/Orin, Linux, EtherCat, CANopen

## Aerospace Projects

### EPFL Rocket Team Rockets (2019-2021)
*Avionics Team Leader*

Student-led rocketry association, designing sounding, bi-liquid and hybrid rockets. Leader of the avionics software team for the BellaLui II rocket and member of the avionics team for BellaLui I.

<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; margin: 1.5rem 0;">
  <iframe src="https://youtube.com/embed/ZRIaitkrEzc" 
          style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" 
          frameborder="0" allowfullscreen></iframe>
</div>

<div style="text-align: center; margin: 1.5rem 0;">
  <img src="{{ '/assets/images/rocket.png' | relative_url }}" alt="Rocket Avionics" style="max-width: 100%; height: auto;">
  <br>
  <small style="color: #666; font-style: italic;">Photo credit: Erik Uythoven</small>
</div>

**Highlights**:
- Hybrid rocket (N2O + ABS)
- 10000ft target altitude
- 2-stage recovery system

**Achievements**: 
- 1st place EuRoC International Competition
- 2nd place Spaceport America Cup in SRAD-10K category
- Successful launch and recovery with full mission objectives met

**Contributions**:
- Management of Avionics Team
- Embedded software architecture
- Sensor acquisition and filtering
- Telemetry
- Logging

**Technologies**: C, C++, Altium

### EPFL Xplore Drone (2023)
*Systems Engineer*

Rapid development of autonomous drone for rover-based aerial reconnaissance in under 6 months.

![Autonomous Drone](/assets/images/drone.png)

**Highlights**:
- In-house avionics and flight computer
- In-house motor controller
- In-house autonomy stack
- In-house structure
- Successful deployment at ERC 2023 World Finals

**Achievements**:
- Contributed to EPFL Xplore's 3rd place at ERC2023 World Finals

**Contributions**:
- Systems engineering and high-level design
- Perception and localization stack
- Power supply
- Numerous other contributions among all subsystems

**Technologies**: C++, ROS2, OpenCV, Capella MBSE, Fusion 360, KiCad, Altium, Embedded Linux, PID control

### SpeQtral QKD Satellite (2023)
*Systems Engineering Intern*

Quantum Key Distribution satellite startup in Singapore, focused on secure key exchange among banks and governments.

![SpeQtral-1 satellite](/assets/images/speqtral.png)

**Highlights**:
- 16U CubeSat
- BB84/BBM92 quantum protocols
- Weak coherent pulse source and entangled photon source

**Contributions**:
- Firmware validation of Speqtre (launching late 2025)
- Firmware architecture and development for SpeQtral-1 (launching late 2026)
- Design of a Thermal Test Model
- Design of spacegrade PCBs

**Technologies**: SystemVerilog, Altium

## Personal Projects

### Stealth Startup (2024-2025)
*Social x Review App*

**Highlights**: *secret*

**Technologies**: Kotlin, React native, Microservice architecture

### RoCo Communication Protocol (2020)
*EPFL Xplore*

Ultra-low-latency communication system for resource-constrained embedded systems implementing an OSI Network layer on standard embedded system busses (I2C, SPI, UART, Ethernet, CAN). 

**Highlights**: 
- Uses static memory exclusively 
- Publisher/Subscriber model 
- Interfacable with ROS2
- Actively used on EPFL Xplore rovers and drones

**Technologies**: C++, STM32

### Rocket Avionics Logging (2019)
*EPFL Rocket Team*

Robust logging system for rocket avionics. Stores flight data in QuadSPI flash memory.

**Highlights**: 
- Uses static memory exclusively
- Block-based filesystem with partition tables
- Survives shutdown-while-writing events and safely overrides irrelevant past logs

**Technologies**: C, STM32

### Lexis Language Learning App (2019)
*Personal Project*

Modernized teaching tool for ancient languages.
Adaptive vocabulary teaching of most used words in Latin and Ancient Greek.

**Highlights**: 
- Used by students of the 2019 Ancient Greek cohort in Geneva

**Technologies**: React native
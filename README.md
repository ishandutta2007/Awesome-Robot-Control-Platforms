# Awesome-Robot-Control-Platforms

# Awesome-Robot-Control-Platforms

# Top Robot Control Platforms Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Real-Time Motion Control, Hardware Abstraction & PLC-Robot Integration*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Robot Control Platforms**. These tools provide the low-level software layer between robot hardware and higher-level planning systems — handling joint trajectory execution, real-time control loops, hardware abstraction, and standardized communication across industrial and collaborative robots.

**Examples** include ROS 2 Control, Beckhoff TwinCAT, KEBA KeMotion, Universal Robots PolyScope, KUKA Sunrise.OS, ABB RobotStudio, FANUC ROBOGUIDE, Stäubli VAL 3, Yaskawa MotoLogix, and Siemens SIMATIC Robot Integrator (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, custom hardware interfaces, and transparent control loops — ideal for robotics engineers, industrial automation developers, and teams avoiding vendor lock-in.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Beckhoff TwinCAT](https://www.beckhoff.com/en-en/products/automation/twincat/)**  
  PC-based automation software suite with PLC, motion control, and robotics integration for industrial automation.

- **[KEBA KeMotion](https://www.keba.com/en/industrial-automation/)**  
  Robot control system with open interfaces for industrial robot manufacturers and system integrators.

- **[Universal Robots PolyScope](https://www.universal-robots.com/)**  
  Intuitive robot control interface for UR collaborative robots with graphical programming and force control.

- **[KUKA Sunrise.OS](https://www.kuka.com/)**  
  Operating system for KUKA LBR iiwa and other KUKA robots with Java-based programming and sensor integration.

- **[ABB RobotStudio](https://new.abb.com/products/robotics/robotstudio)**  
  Simulation and offline programming software for ABB robots with virtual commissioning and programming.

- **[FANUC ROBOGUIDE](https://www.fanucamerica.com/products/robots/robot-software/roboguide)**  
  Simulation software for FANUC robots with offline programming, layout design, and cycle time analysis.

- **[Stäubli VAL 3](https://www.staubli.com/)**  
  Robot programming language and control system for Stäubli industrial robots.

- **[Yaskawa MotoLogix](https://www.motoman.com/)**  
  PLC-based robot control solution allowing Yaskawa robots to be programmed directly from PLC environments.

- **[Siemens SIMATIC Robot Integrator](https://www.siemens.com/)**  
  Solution for integrating robots into Siemens TIA Portal environments with standardized interfaces.

## Open-Source GitHub Projects

- **[ros2_control](https://github.com/ros-controls/ros2_control)**  
  **The standard open-source framework for real-time robot control in ROS 2.** Provides hardware-agnostic control abstractions, controller lifecycle management, and modular composition of control systems. Includes widely-used controllers (joint trajectory, forward command, differential drive) and integrates with MoveIt2 and Nav2. Governed by the Open Source Robotics Alliance (OSRA). Apache 2.0 licensed.

- **[ROS-Industrial](https://rosindustrial.org/packages)**  
  **The bridge between ROS 2 and industrial robot vendors.** Provides ros2_control-compatible drivers for Universal Robots (500 Hz control via Ethernet), Yaskawa Motoman, ABB, FANUC, KUKA, and others. Enables industrial robots to be programmed using standard ROS 2 tools without vendor-specific code.

- **[Movensys WMX R2](https://github.com/movensys/wmx-r2)**  
  ROS 2 interface for WMX3, a real-time EtherCAT motion control SDK. Wraps the WMX3 C++ API into standard ROS 2 nodes, topics, services, and actions so you can drive any EtherCAT-based robot using MoveIt2 or Nav2 without vendor-specific motion code. Supports ROS 2 Humble and Jazzy. Hardware-proven with manipulator and differential-drive configurations.

- **[MotorBridge](https://wiki.seeedstudio.com/ja/rebot_physical_ai_course_chapter_7/)**  
  **Vendor-agnostic CAN motor control library for robotic joints.** Provides a unified API across Damiao, RobStride, MyActuator, HighTorque, and Hexfellow motors, absorbing protocol differences so switching motors requires only changing vendor parameters — not rewriting motion control logic. Rust core with Python/C++/ROS2 bindings, no GC pauses. Includes CLI and web visualization console (MotorBridge-Studio).

- **[CANOpenRobotController (CORC)](https://relatedrepos.com/gh/UniMelbHumanRoboticsLab/CANOpenRobotController)**  
  Free and open-source C++ robot development software stack with EtherCAT support. Provides hardware abstraction and real-time control for CANopen-based robot systems.

- **[RFX SDK](https://pypi.org/project/rfx-sdk/0.2.0/)**  
  Robotics framework for the foundation-model era with a three-method robot interface (`observe()`, `act()`, `reset()`) — same API for simulation and real hardware. Self-describing policies deployable with zero config, HuggingFace Hub native, Zenoh transport, and ROS 2 interop via zenoh-plugin-ros2dds bridge. Rust core for real-time control, Python SDK for fast research.

- **[Intrinsic Core](https://github.com/intrinsic)**  
  **Google's open-sourced industrial robotics platform** released under Apache 2.0. Includes control, motion planning, grasp planning, simulation, pose estimation, and camera calibration software used in real deployments. ROS-compatible by design, with the Open Machine Tending Solution supporting FANUC and Universal Robots out of the box.

- **[SAINT.OS](https://github.com/input-inc/saintos)**  
  ROS 2 control platform for multi-node animatronic and mobile robots. Central server coordinates microcontroller nodes over ROS 2 with web UI, WebSocket API, routing sheets for input-to-actuator binding, and OTA firmware updates. Robot-agnostic via one-file manifest. Reference robot: OpenSAINT (Short Circuit replica).

- **[Beremiz](https://github.com/beremiz/beremiz_public_dist)**  
  Free Software for machine automation with IEC 61131-3 PLC programming support. Includes SoftMotion libraries for CiA402 servo drivers and EtherCAT master integration (IgH EtherCAT Master). Open-source alternative to proprietary PLC platforms.

- **[OpenPLC](https://github.com/thiagoralves/OpenPLC_v3)**  
  Open-source PLC runtime with support for IEC 61131-3 languages. Can be combined with Ruckig motion generation and deployed on embedded platforms for robot control applications.

- **[Ruckig](https://github.com/pantor/ruckig)**  
  Instantaneous motion generation library for robots and machines. Computes jerk-limited trajectories in real-time, ensuring smooth motion without velocity, acceleration, or jerk discontinuities. Used in OpenPLC Drive-On-Chip examples and industrial motion control.

- **[RoboDK API](https://github.com/RoboDK/RoboDK-API)**  
  **Universal programming interface for industrial robots.** Provides simulation and offline programming in Python, C#, C++, Matlab, and JavaScript. Supports a large robot library (FANUC, KUKA, ABB, Yaskawa, Universal Robots) with post-processors generating vendor-specific programs. Free RoboDK license available for simulation and offline programming.

- **[botrail](https://pypi.org/project/botrail/0.12.0/)**  
  Beyond motion planning — verify robot cells, not just trajectories. Load URDF/Xacro/USD robots, add obstacles and behavior (conveyors, beam sensors), write process sequences as steps, and bake deterministic simulations. Same numbers every run means regression tests for your cell: "Move the beam sensor 0.25 m downstream and the cycle grows by exactly 1.0 s — a layout edit becomes a failing test instead of a shop-floor surprise".

- **[jacobi-*-driver](https://packages.ecosyste.ms/registries/pypi.org/keywords/robot-driver)**  
  Python drivers for ABB, Yaskawa, FANUC, and Universal Robots from the jacobi project. Actively maintained (versions released within days of this update), providing consistent Python interfaces across industrial robot brands.

### Additional Strong Open-Source Options

- **ros2_controllers** — Widely-used controllers including joint trajectory, forward command, and differential drive controllers for ros2_control.
- **gz_ros2_control** — Gazebo plugin for ros2_control simulation.
- **mujoco_ros2_control** — MuJoCo plugin for ros2_control simulation.
- **EtherCAT Master (IgH)** — Open-source EtherCAT master stack for real-time industrial communication.
- **SOEM (Simple Open EtherCAT Master)** — Lightweight EtherCAT master library for embedded robot controllers.
- **LeRobot** — Hugging Face's ML library for real-world robotics with training utilities and pretrained policies.
- **Anvil Robotics** — Open-source robotic development kits integrating hardware, controllers, teleoperation, and data pipelines with ROS2 and LeRobot compatibility.

**Frameworks for building custom systems**: Combine **ros2_control** for standardized control abstractions, **ROS-Industrial** drivers for vendor-specific hardware, **MotorBridge** for unified CAN motor control, **WMX R2** for real-time EtherCAT motion, and **RoboDK API** for universal offline programming to build a complete robot control stack.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Robot control platforms must comply with machinery safety directives, real-time constraints, and industry standards (IEC 61131, ISO 10218, ISO/TS 15066 for collaborative robots). Control software errors can cause physical injury or equipment damage.
- Self-hosted open-source solutions require proper real-time validation, safety certification where applicable, and hardware-in-the-loop testing before deployment.

---

**Made for robotics engineers, industrial automation developers, control systems integrators, and teams building robot control platforms.**  
Let's make robot control more open, standardized, and hardware-agnostic.

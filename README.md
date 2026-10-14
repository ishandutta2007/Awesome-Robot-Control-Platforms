# Awesome-Robot-Control-Platforms

# Top Robotics Deployment Tools Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Fleet Orchestration, Edge Deployment & Robot Lifecycle Management*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Robotics Deployment**. These tools help robotics companies get robots into production and keep them running — handling fleet orchestration, over-the-air updates, edge deployment, monitoring, and coordination across heterogeneous robot fleets and sites.

**Examples** include InOrbit, Formant, Freedom Robotics, Foxglove, SVT Robotics, MOV.AI, Cogniteam Nimbus, Rocos, Apex.AI, and RGo Robotics (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, custom fleet orchestration, and transparent robot operations — ideal for robotics companies prioritizing data ownership, developers building deployment infrastructure, and teams avoiding vendor lock-in.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[InOrbit](https://www.inorbit.ai/)**  
  Cloud-based robot operations (RobOps) platform with fleet management, real-time analytics, and incident management. Robot-agnostic agent with adaptive diagnostics, configurable dashboards, advanced teleoperation, and multi-map support. Data sampling modes include Regular, Diff, and Event. Compatible with ROS 1, ROS 2, and non-ROS robots through Edge SDK. Standard Edition free to start with pay-as-you-go pricing based on monthly active robots .

- **[Formant](https://formant.io/)**  
  Fleet observability and robot operations platform with comprehensive device management, incident management, and analytics. Device configuration templates for bulk provisioning, group-based organization, multi-device video monitoring, custom alerting, operator intervention requests, and Formant Analytics for fleet uptime and incident reporting. Supports Slack, SMS, PagerDuty, and webhook notifications .

- **[Freedom Robotics](https://www.freedomrobotics.ai/)**  
  Robot management and teleoperation platform with remote control, video streaming, and fleet monitoring for autonomous systems.

- **[Foxglove](https://foxglove.dev/)**  
  Visualization, observability, and data management platform purpose-built for robotics. Centralizes multimodal temporal datasets including time series, sensor logs, imagery, LiDAR/point clouds, and geospatial maps. Real-time ROS/ROS 2 connections via bridges and WebSockets, with desktop apps for Linux, Windows, and macOS. Free tier includes 3 developer seats, 10 GB cloud storage, and 5 connected devices. Paid plans from $18/month .

- **[SVT Robotics](https://svtrobotics.com/)**  
  SOFTBOT Platform for rapid robot deployment, enabling integration and orchestration across heterogeneous automation systems.

- **[MOV.AI](https://www.mov.ai/)**  
  Robotics engine platform for AMR fleet management and orchestration, with deployment tools and simulation support.

- **[Cogniteam Nimbus](https://www.cogniteam.com/)**  
  Cloud robotics platform for fleet management and autonomous operations.

- **[Rocos](https://www.rocos.io/)**  
  Cloud platform for robot fleet management, deployment, and remote operations.

- **[Apex.AI](https://www.apex.ai/)**  
  Safety-certified autonomous mobility software with fleet deployment tools and functional safety certification.

- **[RGo Robotics](https://www.rgorobotics.com/)**  
  Perception engine for autonomous mobile robots with deployment support for industrial environments.

## Open-Source GitHub Projects

- **[Transitive](https://github.com/transitiverobotics/transitive)**  
  Open-source framework for full-stack robotics with **fine-grained, namespaced access control**. Core concepts include full-stack packages (cross-device dependency management), real-time data synchronization with full-stack reactivity, and topic-based access control. Version 2.0 integrates ClickHouse for historic time-series data, Grafana for visualization, and Alertmanager for custom alerting. Includes free Health Monitoring with sparkline plots and 24-hour heartbeat visualization. Runs on Docker Compose with self-hosted deployment.

- **[Trillium](https://github.com/RobotnikAutomation/trillium)**  
  Free, open-source web-based robotics visualization and control application. Fork of Foxglove Studio v1.87.0 (last open-source release before Foxglove went proprietary). Features 40% smaller web app and 23% smaller desktop binaries compared to Lichtblick (another Foxglove fork). Available as web app, Docker container, or desktop installer for Linux and Windows. Extensions installable directly in browser or desktop app.

- **[OpenRobOps (ORO)](https://www.inorbit.ai/)**  
  InOrbit's open-source robot operations and fleet management layer, announced for full open-source release in 2026. Built on InOrbit's production-proven platform that has managed thousands of AMRs. Integrates natively with ROS on-device and Open RMF for coordination. Provides transparent architecture, observability, fleet control, and full data ownership. Aims to be the standard, self-hostable fleet manager for ROS developers.

- **[NexusOS](https://pypi.org/project/nexusos-robotics/)**  
  Universal OS and fleet middleware for heterogeneous robots, solving the "Tower of Babel" through zero-dependency hardware abstraction. Unifies multi-vendor fleets (mobile rovers, arms, quadrupeds, drones) under standardized messaging, control, and safety. Features asynchronous Python HAL plugin architecture (Serial, CAN, Modbus, ROS 2, MicroPython), Protobuf/WebSocket/gRPC transport, FastAPI cloud backend, and glassmorphic web dashboard with 2D pose trajectory and teleoperation. Docker Compose orchestration.

- **[Open-RMF](https://github.com/open-rmf/rmf)**  
  Open Robot Management Framework for multi-fleet robot coordination in shared spaces. Provides centralized fleet management, traffic scheduling, task allocation, and interoperability across different robot vendors. Used in airports, hospitals, and logistics facilities. Apache 2.0 licensed.

- **[openTCS](https://github.com/openTCS/opentcs)**  
  Open-source transport control system for coordinating fleets of autonomous vehicles in industrial environments. Provides vehicle routing, order management, and communication abstraction. LGPL licensed.

- **[Micro-ROS](https://github.com/micro-ROS/micro_ros_arduino)**  
  Brings ROS 2 to microcontrollers for edge deployment of robot components. Available in Arduino Library Manager. Lightweight client library enabling resource-constrained devices to participate in ROS 2 networks.

- **[Canonical Observability Stack (COS)](https://ubuntu.com/blog/roscon-2025)**  
  Fully open-source observability infrastructure for ROS 2 devices using Ubuntu. Combines Grafana, Prometheus, and Loki for unified monitoring. Features device onboarding, automatic ros2bag uploads to self-hosted server, remote fleet monitoring, live ROS data access, Ubuntu system data and logs access, and event alerting (low battery, network loss). Demonstrated at ROSCon 2025 with Botmind fleet management integration.

- **[Lichtblick](https://github.com/lichtblick-suite/lichtblick)**  
  Fork of Foxglove Studio maintained by BMW. Became the parent repo of Foxglove Studio forks when commit history was deleted. Provides visualization and data management for robotics development with larger binary sizes compared to Trillium (99 MB vs 76 MB for Linux .deb packages).

- **[Dora (dora-rs)](https://github.com/dora-rs/dora)**  
  Robotics dataflow framework and distributed orchestrator for edge AI pipelines. Supports multi-language nodes (Rust, Python, C, C++) with zero-copy shared-memory transport and columnar formats. Includes bidirectional bridges to external ecosystems. Rust-based.

- **[HORUS](https://pypi.org/project/horus-robotics/)**  
  Ultra-low latency robotics framework in Rust with Python bindings. Claims 87ns IPC latency and 12M+ messages/second throughput. Zero-copy shared memory transport, type-safe message validation, cross-language interoperability, and real-time priority-based scheduling. Apache 2.0 licensed.

- **[Open-RAIL](https://github.com/CMCC-TAO/open-rail)**  
  Middleware from China Mobile linking Vision-Language-Action (VLA) and World-Action Models (WAM) to real robot hardware. Three-thread asynchronous pipeline (observation, inference, control) with two-level online smoothing. Hardware abstraction layer standardizes control, state reading, and action execution. Apache 2.0 licensed.

### Additional Strong Open-Source Options

- **[SONNY OS](https://github.com/JackTrainer/Sonny)** — Ultra-lightweight microkernel for any robot built in Rust and Zenoh. JSON-based hardware abstraction layer, WASM sandbox for skill execution, real-time hard-watchdog monitoring. AGPLv3 licensed.
- **[LeRobot](https://github.com/huggingface/lerobot)** — Hugging Face's ML library for real-world robotics in PyTorch. Datasets, pretrained models, and training utilities for edge deployment of VLA models.
- **[Awesome Open Source Robots](https://github.com/stephane-caron/awesome-open-source-robots)** — Curated list of robots with open source software, hardware, and both. Includes arms, bipeds, quadrupeds, humanoids, drones, and mobile manipulators with license information.
- **[Awesome Robotics](https://github.com/ahundt/awesome-robotics)** — Curated list of robotics links and software libraries. 1,364 GitHub stars.
- **ROS 2 Ecosystem** — Standard robot operating system providing middleware, tools, and libraries for fleet deployment.
- **Edge Deployment Tools** — Balena, Ubuntu Core for container-based OTA updates and device fleet management.

**Frameworks for building custom systems**: Combine **Transitive** for full-stack robotics with ClickHouse/Grafana/Alertmanager stack, **Open-RMF** or **openTCS** for multi-fleet coordination, **NexusOS** for heterogeneous fleet abstraction, **Trillium** for open-source Foxglove-compatible visualization, and **Canonical Observability Stack** for ROS 2 fleet monitoring to build a complete self-hosted robotics deployment platform.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Robotics deployment tools must comply with safety regulations, data protection laws, and industry standards. Fleet operations require validation of deployment, update, and monitoring workflows before production use.
- Self-hosted open-source solutions require proper infrastructure, security hardening, and ongoing maintenance.

---

**Made for robotics engineers, fleet operators, DevOps teams, and developers building robot deployment platforms.**  
Let's make robotics deployment more open, observable, and fleet-friendly.

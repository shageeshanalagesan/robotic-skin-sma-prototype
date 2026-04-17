# 🦾 Robotic Skin — SMA-Actuated Programmable Matter Prototype

A lightweight, modular robotic skin prototype capable of conforming to the shape of a human forearm using Shape Memory Alloy (SMA) spring actuation. This project bridges **soft robotics**, **programmable matter**, and **adaptive wearable systems** — demonstrating controlled shape deformation without motors or complex electronics.

---

## 📋 Table of Contents

<details>
<summary>🔍 Click to expand navigation</summary>

- 🤖 [Overview](#-overview)
- 🎥 [Demonstration](#-demonstration)
- ⚡ [Key Features](#-key-features)
- 📁 [Project Structure](#-project-structure)
- 🔬 [Technical Deep Dive](#-technical-deep-dive)
  - [Structural Design](#1-structural-design)
  - [SMA Actuation System](#2-sma-actuation-system)
  - [Electrical Circuit Design](#3-electrical-circuit-design)
  - [Testing Methodology](#4-testing-methodology)
- 📊 [Results & Performance](#-results--performance)
- 🛠️ [Design Improvements](#️-design-improvements)
- 🚀 [Future Work](#-future-work)
- 🌍 [Applications](#-applications)
- 📝 [Academic Context](#-academic-context)
- 👤 [About](#-about)
- 📄 [License](#-license)
- 📧 [Contact](#-contact)

</details>

---

## 🤖 Overview

This project develops a **proof-of-concept robotic skin** — a flexible, modular surface structure that can change shape to wrap around a human forearm using electrical stimulation. The system uses **Shape Memory Alloy (SMA) springs** as compact, motorless actuators integrated into a panel-and-hinge mechanical framework.

Rather than relying on conventional motors or pneumatics, this prototype demonstrates that **smart materials combined with thoughtful mechanical design** can produce meaningful, controlled actuation at low cost and with minimal system complexity.

> 🎯 **Performance Highlights:** 6-Panel Modular Structure • SMA Spring Actuation • ~20s Closing Cycle • ~300J per Cycle • Battery Powered • No Motors

---

## 🎥 Demonstration

### 📸 Prototype Gallery

<img width="300" alt="IMG_8626" src="https://github.com/user-attachments/assets/7ac5f3b3-1b49-46f8-b31f-98846acb1264" /> <img width="300" alt="IMG_6793" src="https://github.com/user-attachments/assets/001575ca-b0d6-411c-9ec1-142e1513469c" />


> *Photos of the prototype in open, actuating, and closed states are documented in the Appendix of the project report.*

**Prototype States:**
- 🟢 **Open / Resting** — Panels flat, springs at resting length (~2 cm)
- 🔴 **Actuating (Closing)** — SMA springs contract under current, panels curl inward
- 🔵 **Closed / Wrapped** — Structure conforms around forearm geometry

---

## ⚡ Key Features

- 🧱 **Modular Panel Architecture** — Six 12 cm × 6 cm × 3.5 mm plywood panels connected by flush hinges for controlled, guided flexibility
- 🔩 **SMA Spring Actuation** — Nitinol helical springs provide large deformation range under resistive heating (~2.5 A), eliminating the need for motors
- ⚡ **Dual-Circuit Control** — Separate electrical circuits for opening and closing actuation, each with three springs in series
- 🔋 **Battery Powered** — Operates from a 4× AA battery pack (~6 V), making it portable and self-contained
- 📐 **Partial Bracing System** — Triangular plywood braces create a 120° guided deformation geometry; first three joints flexible, last three fixed
- ♻️ **Low-Cost & Sustainable** — Built from recyclable plywood and standard hardware; ~300 J per actuation cycle
- 🏥 **Multi-Domain Applicability** — Targets medical rehabilitation, VR/AR wearables, space adaptive structures, and robotic exosuits

---

## 📁 Project Structure

```
robotic-skin-sma-prototype/
├── report/
│   └── Shageeshan_Alagesan_201683484_Final_Report.pdf   # Full academic report
├── figures/
│   ├── fig1_sma_wire_before.jpg        # SMA wire pre-actuation (14.1 cm)
│   ├── fig2_sma_wire_after.jpg         # SMA wire post-actuation (13.4 cm)
│   ├── fig3_final_prototype.jpg        # Final assembled prototype
│   ├── fig4_preliminary_testing.jpg    # Wire routing / flex tests
│   ├── fig5_prototype_open.jpg         # Structure fully extended
│   ├── fig6_prototype_closed.jpg       # Structure manually closed
│   └── fig7_eyelets_installed.jpg      # Metal eyelets replacing plastic guides
├── circuit/
│   └── circuit_diagram.png            # Dual-circuit wiring schematic
└── README.md
```

---

## 🔬 Technical Deep Dive

### 1. Structural Design

The mechanical frame consists of **six modular plywood panels** (12 cm × 6 cm × 3.5 mm) connected sequentially by **flush hinges** to allow controlled bending. 

Key design decisions:
- **Plastic guides → Metal eyelets**: Initial plastic guides produced excessive friction at hinge joints. Replaced with steel eyelets screwed directly into the plywood for smoother actuator routing.
- **Triangular bracing**: Plywood braces added between panels to enforce a 120° angular geometry. The last three panels are **fully fixed** (rigid); the first three joints have **one-sided bracing** (hot glue only), enabling up to ~60° of flexible movement per joint.
- **Partial constraint approach**: This technique balances structural guidance with motion freedom, critical for reliable SMA actuation and return-to-form behaviour.

---

### 2. SMA Actuation System

**Why SMA Springs over SMA Wires?**

| Parameter | SMA Wire | SMA Spring |
|---|---|---|
| Resting length | 14.1 cm | ~2 cm |
| Contraction achieved | 7 mm (~5% strain) | Significantly larger |
| Required for actuation | ~8% strain (1.6 cm) | ✅ Sufficient |
| Verdict | ❌ Insufficient | ✅ Selected |

SMA wire tested at 0.8 A contracted only from 14.1 cm → 13.4 cm — not enough for functional bending. **SMA springs** (helical Nitinol) were selected due to their far greater deformation range under the same principle of resistive heating.

**Spring specification:**
- Resting length: ~2 cm per spring
- Operating current: 2.5–3 A
- Mounted horizontally across the first three joints using metal eyelets
- Validated via thermal test (boiling water >70°C) before electrical integration

---

### 3. Electrical Circuit Design

Two independent circuits power the actuation:

```
Closing Circuit:   [Battery Pack] ── Spring 1 ── Spring 2 ── Spring 3 ── [GND]
Opening Circuit:   [Battery Pack] ── Spring 4 ── Spring 5 ── Spring 6 ── [GND]
```

- **Power supply:** 4× AA batteries (~6 V, ~2.5 A)
- **Connections:** Manual bare-wire contact (no switches in V1)
- **Assembly:** Soldering completed under supervision; steel clips used as spring terminals

---

### 4. Testing Methodology

All testing was **qualitative** — focused on observing and documenting mechanical performance and deformation behaviour.

**Phase 1 — Pre-integration actuator testing:**
- SMA springs hand-stretched and submerged in boiling water (>70°C) → immediate shape recovery ✅
- Springs connected via steel clips to battery → electrical contraction confirmed ✅ (slower than thermal, as expected from resistive heating)

**Phase 2 — Integrated system testing:**
- Closing circuit energised → panels bent inward smoothly and consistently
- Opening circuit energised → partial recovery; springs jammed in hinge gaps at joints 2 and 3

---

## 📊 Results & Performance

| Test | Outcome |
|---|---|
| SMA thermal validation | ✅ Immediate recovery in boiling water |
| SMA electrical validation | ✅ Visible contraction at 2.5 A |
| Closing actuation | ✅ Full closure in ~20 seconds, repeatable |
| Opening actuation | ⚠️ Joint 1 fully recovered; joints 2–3 required manual assist |
| Energy per cycle | ~300 J (2.5 A × 6 V × 20 s) |
| Actuation method | Manual bare-wire contact |
| Sensors / feedback | None (qualitative observation) |

> ⚠️ **Key limitation:** SMA spring geometry (helical) caused jamming in hinge gaps during extension. The closing direction performed reliably; bidirectional autonomous actuation requires design iteration.

---

## 🛠️ Design Improvements

Based on experimental findings, the following improvements are proposed for V2:

- 📐 **Curved joint profiles** — Reduce panel edge gaps to prevent SMA spring jamming during extension
- 🖨️ **3D-printed structural frame** — Replace hand-cut plywood for higher dimensional accuracy, consistent hinge spacing, and better spring mounting points
- 🧤 **Thermal insulation sleeves** — Enclose SMA springs to prevent mechanical friction, environmental exposure, and user skin contact during heating
- 🎛️ **Arduino microcontroller** — Manage voltage regulation, actuation cycles, and sensor input for controlled, repeatable performance
- 🔘 **Electric switches** — Replace manual bare-wire contact to improve safety and activation consistency
- 📡 **Wireless/voice activation** — Enable remote triggering to eliminate manual contact with live circuits

---

## 🚀 Future Work

- **Full body scaling** — Extend the modular panel concept to larger adaptive surface systems (e.g. arm, torso)
- **Closed-loop control** — Integrate flex sensors or IMUs to provide real-time positional feedback for autonomous actuation
- **Reinforcement Learning** — Train an RL agent to optimise actuation sequences and timing for smoother, more consistent deformation
- **Bi-directional autonomy** — Redesign spring mounting geometry to achieve fully autonomous opening and closing without external input
- **Advanced materials** — Explore two-way SMAs or SMA composites to enable passive return-to-form without a second actuation circuit

---

## 🌍 Applications

| Domain | Application |
|---|---|
| 🏥 Medical Rehabilitation | Lightweight, flexible exoskeleton for limb recovery assistance |
| 🕹️ VR / AR | Adaptive haptic suit components with no rigid external hardware |
| 🚀 Space | Shape-adaptive structures that reduce payload weight and reconfigure on-mission |
| 🤖 Soft Robotics | Modular robotic skin for safe human-robot interaction |
| 🎓 Education | Low-cost programmable matter demonstrator kit |

---

## 📝 Academic Context

| | |
|---|---|
| **Module** | ENGG341 Individual Project |
| **Degree** | MEng Aerospace Engineering |
| **University** | University of Liverpool |
| **Submission** | May 2025 |
| **Supervisor** | Paolo Paoletti |
| **Technical Support** | Derek Neary (design, construction, testing), Richard Potter (SMA material selection) |

---

## 👤 About

**Shageeshan Alagesan**  
MEng Aerospace Engineering — University of Liverpool (2025)  
Currently based in Zürich, Switzerland, pursuing entry-level roles in MRO and aerospace engineering.

Interests: Aerospace systems, smart materials, soft robotics, CAD, and building things that work with minimal complexity.

---

## 📄 License

This project is licensed under the MIT License. See `LICENSE` for details.

---

## 📧 Contact

**Shageeshan Alagesan**  
🔗 [GitHub](https://github.com/shageeshanalagesan)  
📍 Zürich, Switzerland

---

*This prototype was developed as a proof-of-concept for programmable matter and adaptive structures using accessible materials and smart actuation. It demonstrates that meaningful shape adaptation is achievable without complex electronics — given careful mechanical design.*

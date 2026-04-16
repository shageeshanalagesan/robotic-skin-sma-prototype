# 🦾 Robotics Programmable Matter — Robotic Skin Prototype

> **Final Year Individual Project** | ENGG341 | University of Liverpool — School of Engineering  
> **Author:** Shageeshan Alagesan | MEng Aerospace Engineering | May 2025  
> **Supervisor:** Paolo Paoletti | Project No. 183/4

---

## 📌 Table of Contents

- [Project Overview](#project-overview)
- [Skills Demonstrated](#skills-demonstrated)
- [Background & Motivation](#background--motivation)
- [Aims & Objectives](#aims--objectives)
- [Project Approach](#project-approach)
- [Literature Review](#literature-review)
- [Methodology](#methodology)
- [Results](#results)
- [Discussion & Design Improvements](#discussion--design-improvements)
- [Sustainability & Reflections](#sustainability--reflections)
- [Conclusion](#conclusion)
- [References](#references)

---

## Project Overview

This project designed and built a **shape-adaptive robotic skin prototype** capable of wrapping around a human forearm through electrically-triggered actuation. The system uses **Shape Memory Alloy (SMA) springs** as the active actuators, embedded within a lightweight modular framework of plywood panels and flush hinges.

The prototype successfully demonstrated **controlled, repeatable inward bending** in approximately 20 seconds using a simple battery-powered circuit — with no motors, complex electronics, or external pneumatic systems required.

This work sits at the intersection of **programmable matter**, **soft robotics**, and **wearable technology**, with potential applications in:

- Medical rehabilitation exosuits
- VR / AR haptic feedback gloves
- Space exploration adaptive structures
- Lightweight robotic gripper mechanisms

---

## Skills Demonstrated

| Skill Area | Details |
|---|---|
| **Engineering Design** | Iterative prototype development from concept through physical build and testing |
| **Smart Materials** | Research and hands-on application of Shape Memory Alloys (Nitinol SMA springs) |
| **Mechanical Fabrication** | Panel cutting, hinge assembly, triangular bracing, and eyelet integration using workshop tools |
| **Electrical Systems** | Circuit design, soldering, resistive heating actuation, and dual-circuit (open/close) wiring |
| **Experimental Testing** | Qualitative performance evaluation through manual pull tests, thermal validation, and electrical actuation cycles |
| **Problem Solving & Iteration** | Identified and resolved friction, alignment, and actuation deficiencies across multiple design iterations |
| **Literature Research** | Comprehensive review of programmable matter, SMA actuation, robotic skins, and wearable robotics literature |
| **Technical Writing** | Structured academic report covering methodology, results, and critical analysis |
| **Sustainability Thinking** | Energy analysis (≈300 J per cycle), use of recyclable materials, and consideration of long-term fatigue |
| **Project Management** | Independently managed a multi-semester project with scope changes, workshop coordination, and supervised testing |

---

## Background & Motivation

Recent advances in engineering have enabled the development of materials and structures that adapt to changing conditions. **Programmable matter** refers to materials that can alter their composition, density, or stiffness upon external stimuli. **Adaptive robotics** involves devices that modify their motion based on the task at hand.

Three key domains motivate this research:

**Healthcare:** Existing exoskeleton devices for patient rehabilitation are heavy and uncomfortable. A lightweight, flexible alternative could improve patient compliance and recovery outcomes.

**Entertainment / VR:** Present-day VR suits are restricted by large sensors and wiring. Adaptive wearable skin can enable natural, fluid movement while delivering haptic feedback.

**Space Exploration:** Systems capable of changing shape based on mission demands reduce payload weight and increase flexibility in long-duration missions where repairs are impractical.

This project represents a proof-of-concept addressing these challenges using only low-cost, commonly available materials — demonstrating that meaningful progress can be achieved without high-cost laboratory resources.

---

## Aims & Objectives

### Aim
To design and develop a lightweight, flexible prototype structure capable of adapting its shape to wrap around the human forearm, using SMA springs as the primary actuation mechanism, as a proof of concept for future full-body adaptive systems.

### Objectives

1. Design and fabricate a flexible framework of light plywood panels and flush hinges to allow controlled flexibility.
2. Characterise the reaction of SMA springs to electrical stimulation to be utilised as actuating devices.
3. Integrate the structural design and SMA-based actuation system into a functioning prototype capable of shape adaptation.
4. Test the prototype's deformability, flexibility, and sensitivity through manual test procedures.
5. Determine the operational and performance limitations of the prototype from experimental test data.

---

## Project Approach

The project initially aimed to build an **origami-based foldable programmable matter system** combining SMA wires with an electromagnetic actuation system. However, during early planning (Week 4, Semester 1), this approach was found impractical — the required components were too small and complex to fabricate within the available time and resources.

The project direction was revised toward a **panel-and-hinge modular robotic skin** design. Key decisions in this pivot included:

- Replacing origami folds with **flush-hinged plywood panels** for simpler flexibility
- Switching from **SMA wires to SMA springs**, which offer a much greater deformation range per activation cycle
- Conducting preliminary mechanical testing using common wires before integrating SMA actuation

Mechanical fabrication was carried out at the **Harrison Hughes Building 4th Floor Workshop**. Electrical assembly, soldering, and testing were completed under supervision at **Derek Neary's office** using solder stations and multimeters. Expert guidance on SMA material selection was provided by Richard Potter.

---

## Literature Review

### Programmable Matter & Shape-Adaptive Systems
Programmable matter changes its physical properties (stiffness, shape, density) in response to external stimuli such as temperature, light, or electrical input (Gilpin et al., 2008). Combined with advances in smart materials and soft robotics, this enables structures that dynamically modify geometry to improve environmental interaction and efficiency.

### Robotic Skin & Flexible Surfaces
Robotic skin refers to flexible, adaptive surfaces inspired by biological skin, capable of protection, sensing, and mechanical flexibility (Kim et al., 2013). Advances in soft electronics have enabled skins that fold onto curved geometries, are mechanically responsive, and can actively reshape (Someya & Amagai, 2019).

### Shape Memory Alloys (SMAs)
SMAs recover a pre-strained form upon thermal stimulation via a reversible martensitic phase transformation (Otsuka & Wayman, 1999). **Nickel-titanium (Nitinol)** alloys are the most studied, offering high mechanical strength and energy density (Lagoudas & Lagoudas, 2008). SMA springs — with their helical structure — offer far greater deformation range than straight wires, making them especially suited for flexible surface applications.

### Actuation Method Selection

| Method | Advantages | Limitations |
|---|---|---|
| Pneumatic Actuators | High deformation, widely studied | Requires bulky external pumps; poor portability |
| Electroactive Polymers (EAPs) | High deformation, fast response, low weight | Operate at high voltage; low output force |
| **SMA Springs** ✅ | Compact, high deformation, sufficient force, no external hardware | Slower response; thermal fatigue over cycles |

SMA springs were selected as the optimal actuator for this project due to their balance of compactness, force output, and ability to produce visible shape adaptation without external bulky hardware.

### Research Gap
Most prior work has focused on SMA material properties or large-scale adaptive structures. This project addresses the gap of **integrating SMA springs into a compact, panel-based modular wearable skin** at low cost — bridging wearable technology and soft robotics.

---

## Methodology

### Prototype Structure

The prototype consisted of **six modular plywood panels** (12 cm × 6 cm × 3.5 mm each), connected in series using **flush hinges** to allow controlled bending.

**Structural evolution through iterations:**

1. **Initial build:** Fully flexible, six-panel chain with plastic wire guides (super-glued). Significant friction at hinge joints caused inconsistent movement — the last two panels barely bent under high pulling force.

2. **Iteration 1 — Metal Eyelets:** Plastic guides replaced with steel eyelets screwed directly into the plywood, reducing friction and improving wire motion.

3. **Iteration 2 — Triangular Braces:** Plywood triangular braces added between each panel to enforce a **120° fixed angular relationship**. The final three panels were fully fixed (rigid); the first three joints were partially braced (one side only), allowing bending up to approximately **60°**.

This partial-bracing technique created a balance between structural guidance and motion freedom — critical for successful actuation.

### Actuator Selection & Testing

**SMA Wire (rejected):**
- Wire was clamped and powered at 0.8 A under a 700 g load
- Contracted from 14.1 cm → 13.4 cm (only ~7 mm / ≈5% strain)
- Required ≈8% strain (1.6 cm) to close the structure — **insufficient**

**SMA Springs (selected):**
- Each spring ≈2 cm resting length, helical (Nitinol)
- Thermally validated: Boiling water (>70°C) test confirmed instantaneous shape recovery
- Electrically validated: Resistive heating via steel clips and battery current produced visible contraction
- Three springs connected in series per circuit, powered by a **four-AA battery pack (~6V)**
- Operating current: **2.5–3 A**

### Circuit Design

Two separate circuits were created:
- **Closing circuit:** Energises SMA springs to pull panels inward
- **Opening circuit:** Energises opposing SMA springs to push panels outward

Current was applied manually by connecting exposed wire ends — no electronic switches or microcontrollers were used in this prototype.

---

## Results

### Pre-Integration Actuator Testing
SMA springs were individually validated before integration. Boiling water testing confirmed the **thermal shape memory effect** — springs instantly returned to their coiled form. Electrical testing via battery confirmed **resistive heating contraction**, slightly slower than thermal activation, as expected.

### Functional Performance — Closing Actuation ✅
- When the closing circuit was energised, the **central three panels bent inward smoothly and visibly**
- Full closure reliably achieved in **approximately 20 seconds** across repeated tests
- The fixed triangular braces on the final three panels contributed to consistent overall curvature
- This confirmed the feasibility of SMA springs driving surface deformation in a modular architecture

### Functional Performance — Opening Actuation ⚠️
- Only the **joint immediately after the fixed section** fully extended (~35 seconds)
- The remaining two joints remained stuck — helical springs became caught between panel gaps and hinge joints
- A **manual external push** was required to complete the opening motion
- This indicates a mechanical constraint rather than an actuation force deficiency

### Key Performance Summary

| Test | Outcome |
|---|---|
| SMA wire actuation | ❌ Insufficient strain (5% vs 8% required) |
| SMA spring thermal test | ✅ Instant recovery confirmed |
| SMA spring electrical test | ✅ Contraction observed |
| Prototype closing | ✅ Full closure in ~20 seconds |
| Prototype opening | ⚠️ Partial — manual assist required |
| Forearm wrapping | ✅ Structure conformed around forearm |

---

## Discussion & Design Improvements

### Interpretation of Results
The project successfully demonstrated that **SMA springs can generate controlled, repeatable deformation** in a modular system. The 20-second closing cycle confirmed SMA springs are viable for small, low-power wearable applications. However, the prototype's inability to reopen fully revealed that **mechanical geometry** — not actuation force — was the limiting factor.

### Identified Challenges
- **Spring jamming:** Helical SMA springs caught between panel gaps and hinges during extension, particularly at partially-braced joints
- **Uneven actuation:** Manual spring and eyelet placement caused non-uniform pulling force across joints
- **Uneven heating:** Manual current application caused localised hotspots on some springs, slightly altering their geometry and reducing strength over cycles
- **Material fatigue:** Repeated thermal cycling caused gradual reduction in spring recovery capability and hinge loosening

### Proposed Design Improvements

| Improvement | Benefit |
|---|---|
| Reduce panel edge gaps; use curved joint profiles | Prevents spring jamming during reopening |
| 3D-printed structural frame | Improves dimensional accuracy, hinge spacing, and spring mounting precision |
| Thermal insulation sleeves on SMA springs | Prevents skin burns; protects springs from friction and environmental exposure |
| Arduino / microcontroller integration | Enables automated voltage control, actuation cycle management, and sensor input |
| Voice / remote-operated sensors | Allows wireless activation, eliminating manual contact |
| Electric switches + LED indicators | Improves user safety, circuit visibility, and consistent activation performance |
| Passive/active locking system | Holds the structure in deformed position when worn |

---

## Sustainability & Reflections

The prototype consumed approximately **300 joules per cycle** (2.5 A × 6 V × 20 s) — comparable to lightweight servo systems but with significantly fewer moving parts and lower structural complexity. The use of recyclable plywood and simple mechanical components minimised environmental impact.

SMA springs, however, are susceptible to **thermal-mechanical fatigue** from repeated cyclic loading, gradually reducing actuation reliability (Hartl & Lagoudas, 2007). A modular, replaceable spring design would address this for long-term sustainability.

The project demonstrated that **low-cost, hand-fabricated adaptive systems** can produce meaningful engineering results, supporting the broader goal of affordable and accessible soft robotics. The design philosophy prioritised mechanical simplicity and low fabrication cost over precision — a trade-off accepted in favour of accessibility and rapid prototyping.

> *"The success of smart material systems is not material selection alone but also mechanical integration and design optimisation."*

---

## Conclusion

A flexible six-panel robotic skin prototype was successfully developed using plywood, flush hinges, and SMA springs. The key outcomes were:

- **SMA springs provided effective actuation** — enabling controlled movement and partial wrapping around a forearm
- **Full closure was achieved reliably in ~20 seconds**, demonstrating SMA springs are viable for compact, motorless wearable systems
- **Opening actuation was partially limited** by spring geometry jamming at hinge gaps — a mechanical constraint, not an actuation force failure
- The project established a **solid proof-of-concept** for scalable, lightweight adaptive structures

This project shows it is possible to create smart, adaptive systems **without complex electronics**, provided mechanical design is carefully considered. The prototype offers a foundation for future development of simple, reliable, energy-efficient wearable assistive devices.

---

## References

- Asbeck et al. (2013). Biologically-inspired soft exosuit. *IEEE ICORR 2013*.
- Bar-Cohen, Y. (2004). Electroactive Polymer (EAP) Actuators as Artificial Muscles. https://doi.org/10.1117/3.547465
- Gilpin et al. (2008). Miche: Modular shape formation by self-disassembly. *International Journal of Robotics Research*, 27(3-4). https://doi.org/10.1177/0278364907085557
- Huang et al. (2010). Shape memory materials. *Materials Today*, 13(7-8). https://doi.org/10.1016/S1369-7021(10)70128-0
- Ilievski et al. (2011). Soft robotics for chemists. *Angewandte Chemie*, 50(8). https://doi.org/10.1002/anie.201006464
- Kim et al. (2013). Soft robotics: A bioinspired evolution. *Trends in Biotechnology*, 31(5). https://doi.org/10.1016/j.tibtech.2013.03.002
- Lagoudas & Lagoudas (2008). *Shape Memory Alloys* (Vol. 1). Springer. https://doi.org/10.1007/978-0-387-47685-8
- Majidi, C. (2014). Soft robotics: a perspective. *Soft Robotics*, 1(1).
- Mertmann & Vergani (2008). Design and application of shape memory actuators. *European Physical Journal Special Topics*, 158(1). https://doi.org/10.1140/epjst/e2008-00679-9
- Mohd Jani et al. (2014). A review of shape memory alloy research. *Materials and Design*, 56. https://doi.org/10.1016/j.matdes.2013.11.084
- Otsuka & Wayman (1999). *Shape Memory Materials*. Cambridge University Press.
- Polygerinos et al. (2015). Soft robotic glove for combined assistance and rehabilitation. *Robotics and Autonomous Systems*.
- Shepherd et al. (2011). Multigait soft robot. *PNAS*, 108(51). https://doi.org/10.1073/pnas.1116564108
- Shintake et al. (2018). Soft Robotic Grippers. *Advanced Materials*, 30(29). https://doi.org/10.1002/adma.201707035
- Someya & Amagai (2019). Toward a new generation of smart skins. *Nature Biotechnology*, 37(4). https://doi.org/10.1038/s41587-019-0079-1
- Tsukahara et al. (2009). Standing-up motion support with Robot Suit HAL. *IEEE ICORR 2009*.

---

*University of Liverpool — School of Engineering | ENGG341 Individual Project | May 2025*

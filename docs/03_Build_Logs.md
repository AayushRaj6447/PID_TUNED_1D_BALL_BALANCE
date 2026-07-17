<div align="center">

# 🔨 Build Logs

### *Development Journal • Fabrication • Integration • Testing*

<img src="../Images/build_logs_banner.png" width="100%">

---

![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)
![Documentation](https://img.shields.io/badge/Documentation-Build%20Logs-blue?style=for-the-badge)
![Engineering](https://img.shields.io/badge/Engineering-Prototype-success?style=for-the-badge)

---

*"Engineering is an iterative process. Every successful prototype is built upon lessons learned from previous attempts."*

</div>

---

# 📑 Table of Contents

- Overview
- Project Timeline
- Week 1 – Research
- Week 2 – Planning
- Week 3 – Mechanical Design
- Week 4 – Procurement
- Week 5 – Fabrication
- Week 6 – Electronics
- Week 7 – Programming
- Week 8 – PID Tuning
- Week 9 – Testing
- Week 10 – Final Assembly
- Challenges
- Lessons Learned

---

# 📖 Overview

This document records the complete development journey of the project.

Each phase includes:

- Objectives
- Work Completed
- Challenges
- Solutions
- Images
- Progress

The build log provides complete transparency into how the final system evolved from an initial concept to a working prototype.

---

# 📅 Project Timeline

```text
Research
   │
   ▼
Planning
   │
   ▼
CAD Design
   │
   ▼
Procurement
   │
   ▼
Fabrication
   │
   ▼
Electronics
   │
   ▼
Programming
   │
   ▼
PID Tuning
   │
   ▼
Testing
   │
   ▼
Documentation
```

---

# 📘 Week 1 — Literature Survey

## Objective

Understand the theory behind PID controllers and identify a suitable project that demonstrates real-time feedback control.

### Completed

- Studied closed-loop systems
- Learned PID fundamentals
- Reviewed existing ball balance projects
- Explored sensor options
- Finalized project concept

### Challenges

- Understanding controller tuning
- Choosing an appropriate sensor

### Outcome

✅ Project idea finalized

---

# 📘 Week 2 — System Planning

## Objective

Define project architecture and prepare an implementation roadmap.

### Completed

- Functional decomposition
- Hardware selection
- Initial block diagrams
- Component comparison

### Decisions

✅ Arduino Nano

✅ MG996R Servo

✅ VL53L1X Sensor

---

# 📘 Week 3 — CAD Design

## Objective

Design the mechanical structure.

### Completed

- Rail design
- Base support
- Servo mount
- Pivot mechanism

### Engineering Considerations

- Weight distribution
- Structural rigidity
- Servo clearance
- Sensor placement

<div align="center">

<img src="../Images/cad_week3.png" width="700">

</div>

---

# 📘 Week 4 — Component Procurement

## Components Purchased

| Component | Status |
|-----------|--------|
| Arduino Nano | ✅ |
| Servo Motor | ✅ |
| VL53L1X | ✅ |
| XL4015 | ✅ |
| Breadboard | ✅ |
| Capacitors | ✅ |

### Notes

Most electronic components were sourced from trusted online vendors to ensure compatibility and reliability.

---

# 📘 Week 5 — Mechanical Fabrication

## Work Completed

- Wooden frame fabrication
- Rail cutting
- Servo mounting
- Pivot installation
- Structural alignment

### Challenges

- Maintaining alignment
- Minimizing mechanical play

### Solution

Additional reinforcement and careful alignment of the pivot improved overall rigidity.

<div align="center">

<img src="../Images/fabrication.png" width="700">

</div>

---

# 📘 Week 6 — Electronics Assembly

## Completed

- Arduino wiring
- Sensor integration
- Servo wiring
- Power distribution
- Buck converter adjustment

### Circuit Verification

- Servo tested
- Sensor tested
- Voltage verified
- Ground continuity checked

---

# 📘 Week 7 — Embedded Programming

## Tasks

- Arduino setup
- Sensor initialization
- Servo control
- PID implementation
- Serial debugging

### Features Added

- Adjustable PID gains
- Live serial output
- Sensor calibration
- PWM control

---

# 📘 Week 8 — PID Tuning

## Initial Parameters

| Gain | Value |
|------|-------|
| Kp | — |
| Ki | — |
| Kd | — |

*(Replace with final tuned values.)*

### Procedure

1. Set Ki = 0
2. Set Kd = 0
3. Increase Kp
4. Tune Kd
5. Tune Ki
6. Repeat until stable

### Observations

- High Kp increased oscillations.
- Moderate Kd reduced overshoot.
- Small Ki eliminated steady-state error.

<div align="center">

<img src="../Images/pid_graph.png" width="700">

</div>

---

# 📘 Week 9 — System Testing

## Tests Performed

- Sensor Accuracy
- Servo Response
- PID Stability
- Disturbance Rejection
- Long Duration Operation

### Results

| Test | Status |
|------|--------|
| Sensor | ✅ |
| Servo | ✅ |
| PID | ✅ |
| Power | ✅ |

---

# 📘 Week 10 — Final Assembly

## Completed

- Final wiring
- Cable management
- Hardware tightening
- Documentation
- Demonstration video

<div align="center">

<img src="../Images/final_build.jpg" width="700">

</div>

---

# 🚧 Challenges Encountered

| Challenge | Solution |
|-----------|----------|
| Servo Jitter | Improved PID tuning |
| Mechanical Backlash | Reinforced linkage |
| Sensor Noise | Software filtering |
| Power Fluctuations | Buck converter and decoupling capacitor |
| Oscillations | Adjusted Kd |

---

# 📈 Development Progress

| Stage | Completion |
|--------|------------|
| Research | ✅ 100% |
| Design | ✅ 100% |
| Fabrication | ✅ 100% |
| Electronics | ✅ 100% |
| Programming | ✅ 100% |
| PID Tuning | ✅ 100% |
| Testing | ✅ 100% |
| Documentation | ✅ 100% |

---

# 📌 Lessons Learned

- Mechanical accuracy directly affects controller performance.
- Stable power supply is critical for servo operation.
- Sensor placement influences measurement reliability.
- Proper PID tuning requires patience and experimentation.
- Documentation should evolve alongside development.

---

> [!NOTE]
>
> Maintaining detailed build logs simplifies debugging and improves project reproducibility.

> [!TIP]
>
> Photograph each build stage. These images become valuable references during documentation and presentations.

> [!IMPORTANT]
>
> Never modify multiple subsystems simultaneously during testing. Change one variable at a time to isolate issues effectively.

---

<div align="center">

# 🎉 Prototype Successfully Completed

*"Every iteration brought the system one step closer to stability."*

---

➡ **Next Document:** `04_Testing.md`

</div>
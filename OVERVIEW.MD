# 🎯 Project Overview

<div align="center">

# ⚙️ PID Controlled 1-D Ball Balance System

### *Design, Development and Implementation of a Closed-Loop Control System*

---

**Department of Electronics & Communication Engineering**  
**Birla Institute of Technology, Mesra**

**Team 4**

</div>

---

# 📑 Table of Contents

- Project Description
- Objectives
- Project Scope
- Motivation
- System Overview
- Working Principle
- Expected Outcomes
- Project Deliverables
- Team Members
- Team Responsibilities
- Development Timeline
- Success Criteria
- Repository Structure

---

# 📖 Project Description

The **PID Controlled 1-D Ball Balance System** is an embedded control systems project developed to demonstrate the practical implementation of classical feedback control theory using a **Proportional–Integral–Derivative (PID) controller**.

The project consists of a wooden balancing rail actuated by a **high-torque servo motor**, while the position of the ball is continuously measured using a **VL53L1X Time-of-Flight (ToF) distance sensor**. The measured position is compared against a predefined setpoint, and the resulting error is processed by the PID algorithm running on an **Arduino Nano**.

Based on the controller output, the servo motor dynamically adjusts the inclination of the balancing rail to bring the ball back to the desired position.

This creates a **closed-loop feedback control system**, allowing the project to demonstrate important control engineering concepts including:

- Closed-loop control
- Stability
- Error correction
- Dynamic response
- Feedback systems
- Oscillation
- Overshoot
- Settling time
- Steady-state error
- Controller tuning

Although simple in appearance, the project represents the same control principles used in numerous industrial and aerospace applications such as autonomous drones, robotic manipulators, satellite attitude control, self-balancing robots, and industrial automation systems.

---

# 🎯 Objectives

The primary objectives of this project are:

- Design and fabricate a stable one-dimensional ball balancing mechanism.
- Develop a real-time embedded PID controller.
- Understand the behavior of proportional, integral, and derivative control actions.
- Learn the effect of PID parameters on system response.
- Implement sensor-based closed-loop feedback.
- Analyze system stability using practical experiments.
- Reduce overshoot while maintaining fast response.
- Achieve minimum steady-state error.
- Study controller robustness under external disturbances.
- Build a low-cost educational control systems platform.

---

# 🌍 Project Scope

This project focuses on the implementation of a **single-axis ball balancing system** capable of maintaining the position of a rolling ball near a predefined reference point.

### Included Scope

- Mechanical structure design
- CAD modelling
- Arduino programming
- PID controller implementation
- Servo control
- Position sensing
- Real-time control
- Hardware integration
- Experimental tuning
- Performance analysis

### Out of Scope

The following advanced control techniques are beyond the scope of this project:

- State-space control
- LQR controller
- Adaptive PID
- Fuzzy Logic Control
- Neural Network Controllers
- Reinforcement Learning
- Kalman Filtering
- Machine Vision Based Tracking
- Multi-axis balancing

---

# 💡 Motivation

Control systems are among the most important branches of modern engineering. Nearly every intelligent machine today relies on some form of feedback control.

Examples include:

- Aircraft flight stabilization
- Drone attitude control
- Self-driving vehicles
- CNC machining
- Robotic arms
- Industrial automation
- Medical devices
- Spacecraft attitude control

The 1-D Ball Balance System provides an excellent educational platform for understanding these concepts because it represents an inherently unstable system that requires continuous corrective action.

The project bridges the gap between theoretical control engineering and practical embedded system implementation.

---

# ⚙️ System Overview

The project consists of the following major subsystems.

```
             Desired Position
                     │
                     ▼
            Error Calculation
                     │
                     ▼
              PID Controller
                     │
                     ▼
             Servo Motor (MG996R)
                     │
                     ▼
             Tilting Wooden Rail
                     │
                     ▼
             Ball Movement
                     │
                     ▼
         VL53L1X ToF Sensor
                     │
                     └───────────────┐
                                     │
                                     ▼
                             Arduino Nano
```

The Arduino continuously executes the control algorithm, forming a closed feedback loop capable of correcting disturbances in real time.

---

# 🔄 Working Principle

The operation of the system follows these sequential steps:

1. The ball is placed on the balancing rail.
2. The Time-of-Flight sensor continuously measures its position.
3. Arduino computes the error:

\[
Error = Setpoint - Measured Position
\]

4. The PID controller calculates the required control output.

\[
u(t)=K_p e(t)+K_i\int e(t)dt+K_d\frac{de(t)}{dt}
\]

5. The servo motor tilts the rail.

6. The ball moves toward the desired position.

7. The sensor measures the new position.

8. The feedback loop repeats approximately every few milliseconds.

This continuous correction allows the system to maintain stability even when external disturbances are introduced.

---

# 📦 Major Hardware Components

| Component | Function |
|------------|----------|
| Arduino Nano | Executes PID algorithm |
| MG996R Servo | Tilts balancing rail |
| VL53L1X ToF Sensor | Measures ball position |
| Wooden Rail | Mechanical balancing platform |
| XL4015 Buck Converter | Stable power supply |
| Breadboard & Wiring | Hardware integration |

---

# 📊 Expected Outcomes

At the completion of the project, the system should be capable of:

- Detecting ball position accurately.
- Maintaining the ball near the desired setpoint.
- Rejecting external disturbances.
- Demonstrating stable PID control.
- Operating continuously without oscillation.
- Providing a platform for future control experiments.

---

# 📁 Project Deliverables

The final project includes:

- Complete CAD model
- Mechanical assembly
- Embedded software
- PID implementation
- Circuit diagram
- Testing documentation
- Build logs
- Source code
- Design report
- GitHub repository

---

# 👨‍💻 Team Members

| Name | Role |
|------|------|
| Aayush Raj | PID Algorithm, Embedded Programming, Documentation |
| Nityam Jayaswal | PID Algorithm, Procurement & Assembly, Documentation |
| Roushan Kumar Sinha |CAD, Build, Documentation & Quality Assurance |
| Vinayak Gupta | Testing & Validation, Doucmentation |



---

# 📅 Development Timeline

| Phase | Description |
|--------|-------------|
| Week 1 | Literature Survey |
| Week 2 | Concept Selection |
| Week 3 | CAD Design |
| Week 4 | Procurement |
| Week 5 | Mechanical Fabrication |
| Week 6 | Electronics Integration |
| Week 7 | Programming |
| Week 8 | PID Tuning |
| Week 9 | Testing |
| Week 10 | Documentation |

---

# ✅ Success Criteria

The project is considered successful if the following objectives are achieved:

- Ball remains near the desired position.
- Stable closed-loop control is maintained.
- Oscillations are minimized.
- Overshoot remains within acceptable limits.
- Steady-state error is minimized.
- Servo responds smoothly.
- Sensor readings remain consistent.
- System operates reliably over extended periods.

---

# 📂 Repository Structure

```
PID-1D-Ball-Balance/
│
├── docs/
│   ├── 00_Overview.md
│   ├── 01_Learning_Resources.md
│   ├── 02_Design.md
│   ├── 03_Build_Logs.md
│   ├── 04_Testing.md
│   ├── 05_Budget_Procurement.md
│   ├── 06_Safety.md
│   ├── 07_Lessons_Learnt.md
│   └── 08_Future_Work.md
│
├── CAD/
├── Images/
├── Code/
├── Testing_Data/
└── Videos/
```

---

# 🚀 Future Vision

Although this project demonstrates a classical PID controller for a one-dimensional balancing system, the same architecture can be extended to more sophisticated applications including:

- 2-D Ball-on-Plate Systems
- Autonomous UAV Stabilization
- Self-Balancing Robots
- Robotic Manipulators
- Adaptive Control Systems
- Vision-Based Tracking
- AI-Assisted Controller Tuning
- Industrial Motion Control

---

<div align="center">

## ⭐ "Understanding control theory is not merely about balancing a ball—it is about mastering the principles that stabilize aircraft, guide spacecraft, and automate the modern world."

---

**Department of Electronics & Communication Engineering**  
**Birla Institute of Technology, Mesra**

</div>

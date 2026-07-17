<div align="center">

# 🛡️ Safety Guidelines

### *Electrical Safety • Mechanical Safety • Operational Best Practices*

<img src="../Images/safety_banner.png" width="100%">

---

![Safety](https://img.shields.io/badge/Safety-First-red?style=for-the-badge)
![Electrical](https://img.shields.io/badge/Electrical-Protected-blue?style=for-the-badge)
![Mechanical](https://img.shields.io/badge/Mechanical-Verified-success?style=for-the-badge)

---

*"A successful experiment is one that protects both the engineer and the equipment."*

</div>

---

# 📑 Table of Contents

- Introduction
- Safety Objectives
- General Laboratory Safety
- Electrical Safety
- Mechanical Safety
- Sensor Safety
- Software Safety
- Emergency Procedures
- Maintenance
- Risk Assessment
- Safety Checklist
- Summary

---

# 📖 Introduction

Safety was considered throughout the design, fabrication, and testing phases of this project.

Although the system operates at low voltage, improper handling of electrical components, moving mechanical parts, and tools can still lead to equipment damage or personal injury.

This document outlines the precautions required for safe construction and operation.

---

# 🎯 Safety Objectives

The safety plan aims to:

- Protect users from electrical hazards
- Prevent mechanical injuries
- Reduce equipment damage
- Ensure reliable operation
- Promote safe laboratory practices
- Simplify troubleshooting without introducing additional risks

---

# ⚡ Electrical Safety

## Power Supply

Always verify the output voltage before powering the Arduino and servo motor.

Incorrect voltage may permanently damage the electronics.

---

## Wiring Inspection

Before powering the circuit:

- Verify all wire connections.
- Check for loose terminals.
- Ensure common grounding.
- Confirm correct polarity.
- Inspect solder joints.

---

## Short Circuit Prevention

- Never place conductive objects on the powered circuit.
- Avoid exposed wire ends.
- Use insulated connectors where possible.
- Disconnect power before modifying wiring.

---

## Voltage Regulation

The servo motor should be powered through a regulated supply.

Never power high-current loads directly from the Arduino's 5V pin.

---

# 🔩 Mechanical Safety

The balancing mechanism contains moving parts capable of sudden motion during PID tuning.

Always:

- Keep hands clear of the moving rail.
- Secure all fasteners before testing.
- Ensure the base is stable.
- Verify linkage alignment.

---

## Servo Precautions

The servo may move unexpectedly when the controller starts.

Recommendations:

- Power on only after verifying code.
- Keep fingers away from the linkage.
- Avoid forcing the servo manually while powered.

---

# 📏 Sensor Safety

The VL53L1X Time-of-Flight sensor should be handled carefully.

- Avoid touching the optical window.
- Keep the sensor clean.
- Prevent dust accumulation.
- Protect from moisture.

---

# 💻 Software Safety

Before uploading firmware:

- Review the code for logic errors.
- Verify pin assignments.
- Confirm PID constants are within safe limits.
- Ensure emergency stop functionality (if implemented).

During testing:

- Monitor Serial output.
- Observe unexpected behaviour.
- Stop execution immediately if unstable motion occurs.

---

# 🚨 Emergency Procedures

In case of abnormal operation:

1. Disconnect power immediately.
2. Inspect all wiring.
3. Check servo linkage.
4. Verify sensor connections.
5. Restart only after identifying the cause.

Never continue testing if:

- Components become excessively hot.
- Wiring emits smoke or odor.
- Servo behaves unpredictably.
- Electrical arcing is observed.

---

# 🔧 Preventive Maintenance

Regular maintenance improves reliability and extends component life.

## Before Every Session

- Inspect wiring
- Tighten fasteners
- Clean sensor
- Verify power supply
- Check servo horn

---

## Weekly

- Recalibrate sensor
- Inspect mechanical wear
- Verify rail alignment
- Clean moving parts

---

## Monthly

- Replace damaged jumper wires
- Inspect connectors
- Lubricate pivot if required
- Verify structural integrity

---

# ⚠ Risk Assessment

| Hazard | Likelihood | Severity | Mitigation |
|---------|:---------:|:--------:|------------|
| Loose Wiring | Medium | Medium | Inspect before powering |
| Servo Sudden Motion | Medium | Low | Keep hands clear |
| Short Circuit | Low | High | Verify wiring |
| Mechanical Misalignment | Medium | Medium | Periodic inspection |
| Component Overheating | Low | Medium | Use regulated power |

---

# ✅ Pre-Operation Checklist

| Check | Status |
|--------|:------:|
| Wiring Verified | ☐ |
| Power Supply Checked | ☐ |
| Sensor Connected | ☐ |
| Servo Mounted Securely | ☐ |
| Rail Alignment Verified | ☐ |
| Fasteners Tightened | ☐ |
| Arduino Program Uploaded | ☐ |
| Emergency Shutdown Accessible | ☐ |

---

# 📝 Best Practices

- Work on a clean and organized workspace.
- Keep liquids away from electronics.
- Label wires during assembly.
- Document hardware changes.
- Use proper tools for fabrication.
- Avoid rushing during PID tuning.

---

# 📌 Safety Summary

The project operates at relatively low voltages and moderate mechanical loads, making it suitable for educational demonstrations when basic engineering safety practices are followed.

Routine inspections, careful wiring, and controlled testing significantly reduce the likelihood of equipment failure and improve overall system reliability.

---

> [!NOTE]
>
> Most hardware failures result from wiring mistakes rather than component defects. Always perform a final inspection before applying power.

> [!TIP]
>
> Test new software with the ball removed from the rail to verify servo behaviour before full system operation.

> [!WARNING]
>
> Disconnect power immediately if abnormal heating, smoke, unusual noises, or uncontrolled servo motion are observed.

---

<div align="center">

# 🛡️ Safety Documentation Complete

*"Safety is not an additional feature—it is an essential part of every engineering design."*

---

➡ **Next Document:** `07_Lessons_Learnt.md`

</div>
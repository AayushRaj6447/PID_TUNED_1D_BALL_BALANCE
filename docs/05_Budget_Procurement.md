<div align="center">

# 💰 Budget & Procurement

### *Cost Analysis • Component Selection • Procurement Strategy*

<img src="../Images/budget_banner.png" width="100%">

---

![Budget](https://img.shields.io/badge/Budget-₹1681-success?style=for-the-badge)
![Procurement](https://img.shields.io/badge/Procurement-Completed-blue?style=for-the-badge)
![Status](https://img.shields.io/badge/Cost-Optimized-orange?style=for-the-badge)

---

*"Engineering is about achieving the best possible performance within practical financial constraints."*

</div>

---

# 📑 Table of Contents

- Overview
- Procurement Strategy
- Bill of Materials
- Cost Breakdown
- Vendor Selection
- Component Selection Rationale
- Budget Analysis
- Procurement Challenges
- Cost Optimisation
- Summary

---

# 📖 Overview

A major design objective of this project was to develop a reliable PID-controlled one-dimensional ball balancing system while maintaining a low overall project cost.

Every component was selected after evaluating:

- Performance
- Availability
- Cost
- Ease of replacement
- Compatibility
- Reliability

Where multiple alternatives were available, priority was given to components that provided the best balance between performance and affordability.

The final hardware cost of the complete prototype was **₹1681**, making the project economical while still meeting all functional requirements.

---

# 🛒 Procurement Strategy

The procurement workflow followed a structured engineering process.

```text
Project Requirements
          │
          ▼
 Component Selection
          │
          ▼
 Vendor Comparison
          │
          ▼
 Cost Evaluation
          │
          ▼
 Component Ordering
          │
          ▼
 Quality Verification
          │
          ▼
 System Integration
```

---

# 📦 Bill of Materials (BOM)

| Component | Quantity | Cost (₹) |
|-----------|---------:|---------:|
| Arduino Nano | 1 | 217 |
| MG996R Positional Servo | 1 | 343 |
| VL53L1X ToF Sensor | 1 | 302 |
| Buck Converter | 1 | 142 |
| Breadboard | 1 | 36 |
| Jumper Wires | 1 Set | 132 |
| Capacitor | 1 | 12 |
| Wooden Plank | 1 | 245 |
| Shipping Charges | — | 191 |
| **Total Cost** | | **₹1681** |

---

# 📊 Cost Breakdown

| Category | Cost (₹) |
|----------|---------:|
| Electronics | 1184 |
| Mechanical Structure | 245 |
| Shipping | 191 |
| Miscellaneous | 61 |
| **Grand Total** | **₹1681** |

---

# 📈 Budget Distribution

```text
Electronics          ██████████████████████████████ 70%

Mechanical           ██████ 15%

Shipping             █████ 11%

Miscellaneous        ██ 4%
```

---

# 🏪 Procurement Sources

The majority of the electronic components were purchased from reliable online robotics and electronics suppliers while structural materials were sourced locally.

| Component | Source |
|-----------|--------|
| Arduino Nano | Electronics Supplier |
| MG996R Servo | Robotics Store |
| VL53L1X Sensor | Robotics Supplier |
| Buck Converter | Electronics Supplier |
| Wooden Plank | Local Hardware Store |
| Breadboard & Wiring | Electronics Store |

---

# 🎯 Component Selection Rationale

## Arduino Nano

Chosen because of:

- Compact size
- ATmega328P reliability
- Excellent Arduino IDE support
- Large community
- Low cost

---

## MG996R Servo Motor

Selected due to:

- High torque output
- Affordable pricing
- Sufficient rotational accuracy
- Easy Arduino interfacing

---

## VL53L1X Time-of-Flight Sensor

Selected because it provides:

- High measurement accuracy
- Fast response time
- Better repeatability than conventional ultrasonic sensors
- Stable measurements required for PID control

---

## Buck Converter

The project initially considered a standard XL4015 module during design. During implementation, the power arrangement was revised to use an external power breakout configuration for improved stability and isolation of the servo supply. :contentReference[oaicite:1]{index=1}

Advantages include:

- Stable voltage
- Reduced heating
- Improved current capability
- Better protection for the Arduino

---

# ⚖ Cost vs Performance

| Component | Cost | Performance | Selected |
|-----------|:---:|:-----------:|:--------:|
| Arduino Nano | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐☆ | ✅ |
| MG996R Servo | ⭐⭐⭐⭐☆ | ⭐⭐⭐⭐⭐ | ✅ |
| VL53L1X Sensor | ⭐⭐⭐☆☆ | ⭐⭐⭐⭐⭐ | ✅ |
| Buck Converter | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐☆ | ✅ |

---

# 🚧 Procurement Challenges

Several practical issues were encountered during procurement:

- Limited local availability of robotics components
- Delivery delays
- Shipping charges increased the overall project cost
- Need to verify compatibility between purchased components
- Sensor availability varied across suppliers

Despite these challenges, all required components were procured successfully without affecting the development schedule.

---

# 💡 Cost Optimisation

Future versions of the system can further reduce cost by:

- Designing a custom PCB
- Eliminating breadboard wiring
- Ordering components in bulk
- Reusing laboratory hardware
- Fabricating custom mechanical parts using 3D printing

---

# 📌 Budget Summary

The complete PID Ball Balance System was successfully developed with a total expenditure of **₹1681**.

The procurement process prioritized performance, compatibility, and long-term reliability while keeping the project affordable for educational and research purposes.

The selected hardware also allows easy replacement and future upgrades without requiring significant redesign.

---

> [!NOTE]
>
> Maintain invoices and purchase records for future maintenance and component replacement.

> [!TIP]
>
> Always verify voltage ratings, current requirements, dimensions and compatibility before purchasing electronic components.

> [!IMPORTANT]
>
> The cheapest component is not always the best choice. Long-term reliability and compatibility should always be prioritised over minimal cost.

---

<div align="center">

# 💰 Final Project Cost

# **₹1681**

---

**Affordable • Reliable • Educational • Expandable**

➡ **Next Document:** `06_Safety.md`

</div>

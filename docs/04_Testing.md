<div align="center">

# 🧪 Testing & Validation

### *Performance Evaluation • PID Tuning • Experimental Analysis*

<img src="../Images/testing_banner.png" width="100%">

---

![Testing](https://img.shields.io/badge/Testing-Completed-success?style=for-the-badge)
![Validation](https://img.shields.io/badge/Validation-Passed-blue?style=for-the-badge)
![PID](https://img.shields.io/badge/Controller-Tuned-orange?style=for-the-badge)

---

*"A controller is only as good as the experiments that validate it."*

</div>

---

# 📑 Table of Contents

- Testing Objectives
- Test Environment
- Equipment Used
- Calibration
- Test Cases
- PID Tuning Procedure
- Experimental Results
- Error Analysis
- System Limitations
- Validation Summary

---

# 🎯 Testing Objectives

The testing phase was conducted to verify that the designed system satisfies the functional and performance requirements.

The objectives were:

- Verify sensor accuracy
- Validate servo response
- Tune PID parameters
- Measure stability
- Evaluate repeatability
- Observe transient response
- Analyze steady-state performance
- Document limitations

---

# 🧪 Test Environment

| Parameter | Value |
|-----------|-------|
| Controller | Arduino Nano |
| Sensor | VL53L1X |
| Servo | MG996R |
| Power Supply | 5V Regulated |
| Rail Length | 600 mm |
| Test Surface | Flat Wooden Table |
| Ambient Conditions | Indoor |

---

# 🔧 Equipment Used

| Equipment | Purpose |
|-----------|---------|
| Steel Ball | Controlled Object |
| Scale | Distance Verification |
| Laptop | Serial Monitoring |
| Arduino IDE | Data Logging |
| Power Supply | Stable Operation |

---

# 📏 Sensor Calibration

Before performing experiments, the distance sensor was calibrated.

## Procedure

1. Place the ball at known positions.
2. Record measured values.
3. Compare with actual distances.
4. Calculate measurement error.
5. Repeat for multiple positions.

---

# ⚙ Servo Calibration

Servo calibration ensures that the commanded angle matches the actual rail inclination.

### Procedure

- Set servo to neutral position.
- Align the balancing rail horizontally.
- Adjust linkage if required.
- Verify full operating range.

---

# 📋 Test Cases

## Test Case 1 — Sensor Accuracy

### Objective

Verify the accuracy and repeatability of the VL53L1X sensor.

### Procedure

- Position the ball at predefined intervals.
- Record measured distance.
- Compare against actual position.

| Test | Expected | Result |
|------|----------|--------|
| Position Detection | Accurate | ✅ Pass |
| Repeatability | Stable | ✅ Pass |

---

## Test Case 2 — Servo Response

### Objective

Measure the response of the actuator.

### Procedure

- Apply fixed PWM commands.
- Observe rail inclination.
- Check smoothness of motion.

| Observation | Status |
|-------------|--------|
| Smooth Motion | ✅ |
| No Stalling | ✅ |
| Full Range | ✅ |

---

## Test Case 3 — Closed Loop Stability

### Objective

Verify that the PID controller maintains the desired ball position.

### Expected Behaviour

- Ball moves toward setpoint.
- Oscillations reduce over time.
- Stable equilibrium achieved.

### Result

✅ Stable Operation Achieved

---

## Test Case 4 — Disturbance Rejection

### Objective

Evaluate controller performance after external disturbances.

### Procedure

- Push the ball away from equilibrium.
- Observe system recovery.

### Observation

The controller successfully returned the ball to the reference position after a short transient period.

---

# 📈 PID Tuning

The PID controller was tuned experimentally.

## Step 1

Set

```
Ki = 0
Kd = 0
```

Increase Kp gradually until oscillations begin.

---

## Step 2

Increase Kd

Observe

- Reduced overshoot
- Faster settling
- Improved damping

---

## Step 3

Introduce Ki

Observe

- Reduced steady-state error
- Improved accuracy

---

# 📊 Tuned PID Parameters

| Parameter | Value |
|-----------|-------|
| Kp | *(Insert Final Value)* |
| Ki | *(Insert Final Value)* |
| Kd | *(Insert Final Value)* |

---

# 📉 System Response

<div align="center">

<img src="../Images/system_response.png" width="750">

</div>

### Observations

- Initial overshoot observed.
- Oscillations damped rapidly.
- Stable equilibrium achieved.
- Minimal steady-state error.

---

# 📊 Performance Metrics

| Metric | Observation |
|---------|-------------|
| Rise Time | Good |
| Overshoot | Low |
| Settling Time | Acceptable |
| Steady-State Error | Minimal |
| Stability | Stable |

---

# 🔬 Error Analysis

Several sources of error were identified during experimentation.

| Source | Effect |
|---------|--------|
| Sensor Noise | Position fluctuations |
| Servo Backlash | Reduced precision |
| Rail Friction | Slower response |
| Mechanical Misalignment | Tracking error |
| Power Supply Ripple | Servo jitter |

---

# 📉 Limitations

The current prototype has several practical limitations.

- Limited servo resolution
- Mechanical backlash
- Friction losses
- Fixed PID gains
- Single-axis balancing
- Manual tuning

---

# 💡 Possible Improvements

- Replace MG996R with a digital servo.
- Add encoder feedback.
- Implement adaptive PID.
- Introduce Kalman filtering.
- Upgrade to STM32 for faster execution.
- Add wireless telemetry.

---

# ✅ Validation Summary

| Test | Result |
|------|--------|
| Sensor Calibration | ✅ Pass |
| Servo Calibration | ✅ Pass |
| Position Detection | ✅ Pass |
| PID Stability | ✅ Pass |
| Disturbance Rejection | ✅ Pass |
| Long Duration Operation | ✅ Pass |

---

# 📌 Conclusions

The testing phase confirmed that the designed PID-controlled ball balance system meets the intended educational objectives. The controller successfully stabilized the ball around the desired setpoint under normal operating conditions, demonstrating the effectiveness of classical feedback control.

Although practical limitations such as servo backlash and sensor noise affected overall precision, the system remained stable and repeatable throughout testing.

---

> [!NOTE]
>
> Accurate testing requires a rigid mechanical structure and a stable power supply.

> [!TIP]
>
> Record serial data during every experiment. Logged data is invaluable for analysing controller performance and tuning.

> [!IMPORTANT]
>
> Tune only one PID parameter at a time. Simultaneous adjustments make it difficult to determine the effect of individual gains.

---

<div align="center">

# 📈 Testing Successfully Completed

*"Design proves intent. Testing proves reality."*

---

➡ **Next Document:** `05_Budget_Procurement.md`

</div>
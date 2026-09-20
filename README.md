# 🏎️ FSAE Vehicle Dynamics Simulator

**Open-source vehicle dynamics and design simulator for Formula SAE vehicles.**

🌐 **[Live Demo](https://diegolin156.github.io/Simulador-general-para-dise-o-de-auto-de-FSAE/)**

---

## What is this?

A browser-based engineering tool designed to help **Formula SAE teams analyze, design and optimize a race car** using an integrated vehicle model.

The simulator connects:

- Suspension
- Tire dynamics
- Vehicle dynamics
- Aerodynamics
- Powertrain
- Differential
- Braking
- Mass distribution
- Vertical dynamics
- Lap simulation
- Telemetry
- Real-time vehicle simulation

The goal is to create a workflow where a design decision can be evaluated through its effect on the **complete vehicle**, rather than through isolated calculations.

> **Design → Simulate → Analyze → Iterate**

---

## 🚗 Main Features

### Suspension & Kinematics

Analyze the geometric behavior of the suspension throughout wheel travel.

- Camber
- Toe
- Caster
- Kingpin inclination
- Motion ratio
- Wheel rate
- Spring rate
- Anti-dive
- Anti-squat
- Roll center
- Roll stiffness
- Suspension travel

---

### 🛞 Tire Model

The simulator includes a tire model based on **Pacejka's Magic Formula**.

The model considers:

- Longitudinal slip
- Lateral slip angle
- Combined slip
- Vertical load
- Tire forces
- Tire moments

> Tire parameters are currently generic. Accurate competition results require measured or manufacturer-provided tire data.

---

### ⚙️ Powertrain

Model the vehicle's longitudinal performance through:

- Engine / motor characteristics
- Gear ratios
- Final drive
- Wheel radius
- Drivetrain losses
- Traction limits
- Differential behavior

---

### 🌬️ Aerodynamics

Model the aerodynamic contribution to vehicle performance:

- Downforce
- Drag
- Center of pressure
- Aero balance
- Speed-dependent aerodynamic forces

---

### 🛑 Braking

Analyze braking performance including:

- Brake force distribution
- Weight transfer
- Tire grip limits
- Lock-up conditions
- Longitudinal deceleration

---

### 🏁 Vehicle Dynamics

The simulator combines the individual subsystems into a complete vehicle model.

The model can analyze:

- Longitudinal acceleration
- Braking
- Cornering
- Load transfer
- Roll
- Pitch
- Tire forces
- Vehicle slip
- Suspension response

---

### 📊 Lap Simulation

Evaluate how a vehicle configuration affects track performance.

The simulator can be used to investigate the influence of:

- Mass
- Power
- Gear ratios
- Aerodynamics
- Tire characteristics
- Suspension setup
- Weight distribution

on simulated lap performance.

---

### 🎮 Real-Time Driving

The project also includes a real-time vehicle simulation environment.

It provides:

- Manual driving
- Autonomous driving
- Steering input
- Throttle
- Brake
- Vehicle dynamics
- Real-time telemetry

Telemetry can be used to inspect the vehicle's behavior while driving.

---

## 🔬 Engineering Workflow

The simulator is intended to support an iterative engineering workflow:

```text
        VEHICLE DESIGN
              │
              ▼
      ┌───────────────┐
      │ Vehicle Setup │
      └───────┬───────┘
              │
              ▼
      ┌───────────────┐
      │ Physics Model │
      └───────┬───────┘
              │
              ▼
       ┌─────────────┐
       │ Simulation  │
       └──────┬──────┘
              │
       ┌──────┴──────┐
       ▼             ▼
   Telemetry     Lap Time
       │             │
       └──────┬──────┘
              ▼
       DESIGN ITERATION
```

The objective is not simply to calculate individual parameters, but to understand **how design decisions propagate through the vehicle**.

---

## 📐 Physics Models

The simulator currently incorporates models for:

| System | Model / Method |
|---|---|
| Tires | Pacejka / Magic Formula |
| Suspension | Kinematic & geometric analysis |
| Load transfer | Vehicle dynamics model |
| Longitudinal dynamics | Force-based vehicle model |
| Lateral dynamics | Tire force / vehicle dynamics model |
| Aerodynamics | Downforce & drag model |
| Powertrain | Torque / gearing model |
| Braking | Tire-limited braking model |
| Vertical dynamics | Suspension response model |

---

## ⚠️ Model Limitations

This project is intended as an **engineering analysis and design tool**, not as a replacement for physical testing.

Important limitations include:

- Tire parameters are not currently based on a specific competition tire.
- Some vehicle parameters must be obtained experimentally.
- Real suspension compliance is not fully represented.
- Real-world tire temperature effects are simplified.
- Aerodynamic coefficients depend on the accuracy of the input data.
- Simulation accuracy depends strongly on the quality of the vehicle parameters.

For competition use, simulation results should be validated against:

**CAD → Bench testing → Track data → Telemetry**

---

## 🧪 Validation

A major objective of the project is to compare simulation results against real-world measurements.

Potential validation cases include:

- 0–75 m acceleration
- Braking distance
- Skidpad lateral acceleration
- Autocross lap time
- Suspension travel
- Wheel loads
- Vehicle yaw response
- Tire behavior

Validation data can be used to calibrate the vehicle model and improve predictive accuracy.

---

## 🛠️ Technology

The project is designed to run directly in the browser.

No installation is required for the live version.

**Live application:**

[https://diegolin156.github.io/Simulador-general-para-dise-o-de-auto-de-FSAE/](https://diegolin156.github.io/Simulador-general-para-dise-o-de-auto-de-FSAE/)

---

## 🎯 Project Goals

The long-term goal is to develop a **general-purpose open-source vehicle dynamics platform for Formula SAE teams**.

Planned development areas include:

- [ ] Experimental tire-data calibration
- [ ] Real vehicle telemetry import
- [ ] Simulation vs. telemetry comparison
- [ ] Setup comparison
- [ ] Automated setup optimization
- [ ] Track editor
- [ ] More advanced tire models
- [ ] Aero map integration
- [ ] Vehicle parameter optimization
- [ ] Exportable engineering reports

---

## 🤝 Contributing

Contributions, suggestions, validation data and engineering feedback are welcome.

If you are part of a Formula SAE / Formula Student team and want to contribute real vehicle data, testing results or models, feel free to open an issue or pull request.

---

## 📚 Engineering References

The project is based on established vehicle dynamics concepts and models, including:

- Pacejka — *Tire and Vehicle Dynamics*
- Milliken & Milliken — *Race Car Vehicle Dynamics*
- Gillespie — *Fundamentals of Vehicle Dynamics*
- Formula SAE technical regulations
- Vehicle dynamics and tire-model literature

---

## 📄 License

[Add your chosen license here.]

---

## 👨‍💻 Author

**Diego**

Mechanical Engineering student developing an open-source vehicle dynamics simulator focused on Formula SAE applications.

---

### ⭐ If you find the project useful

Give the repository a **star ⭐** and share it with other Formula SAE / Formula Student teams.

Feedback, bug reports and engineering contributions are welcome.

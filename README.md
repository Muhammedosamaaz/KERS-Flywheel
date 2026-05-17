# KERS — Kinetic Energy Recovery System

**Bench-scale flywheel regenerative braking prototype**  
Sinai University | Mechanical Engineering | 2025/2026  
Student: Muhammed Osama Muhammed | Supervised by: Prof. Waleed Farag

---

## Overview

This project implements a closed-loop KERS that stores kinetic energy in a steel flywheel during acceleration and recovers it as electrical energy during regenerative braking.

**Key results:**
- 307 J stored at 3000 RPM
- 35.7 J recovered to 2.5 F supercapacitor
- Round-trip efficiency: 15–22%
- Speed fluctuation coefficient Cs = 0.03–0.06
- Structural safety factor = 71

---

## Hardware

| Component | Specification |
|-----------|---------------|
| Flywheel | Mild steel, 1.7 kg, I = 0.006216 kg·m² |
| Motor | 775 DC, 12 V |
| Motor driver | BTS7960 H-bridge (490 Hz PWM) |
| Microcontroller | Arduino UNO |
| Sensors | LM393 optical encoder, ACS712 current sensor |
| Energy storage | 2.5 F / 5.4 V supercapacitor |

---

## Software

- **Arduino** – State machine (DRIVE/COAST/REGEN), RPM measurement, safety interlocks
- **MATLAB** – Post-processing, turning moment diagrams, efficiency calculation
- **Web dashboard** – Real-time telemetry (Chart.js)

---

## Repository Contents

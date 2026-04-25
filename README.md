#  Automated Speed & Direction Control using Siemens PLC & Delta VFD

##  Overview

This project demonstrates a **fully automated motor control system** using:

* Siemens PLC 
* Delta Variable Frequency Drive (VFD)
* Real industrial wiring setup

The system automatically controls **motor speed and direction** in a cyclic sequence based on time.

---

##  Objective

Design a control system where the motor:

* Changes **speed (frequency)** step-by-step
* Switches between **Forward and Reverse**
* Operates in a continuous automatic loop
* Uses **PLC logic + VFD control integration**

---

## ⚙️ System Components

* Siemens PLC (Programmed using TIA Portal)
* Delta VFD (Motor Drive)
* 3-Phase Induction Motor
* Real Wiring & Control Circuit
* Digital Outputs from PLC → VFD Inputs

---

##  Operation Sequence (IMPORTANT)

Each step runs for **3 seconds**:

| Step | Direction    | Frequency |
| ---- | ------------ | --------- |
| 1    | Forward      | 15 Hz     |
| 2    | Forward      | 30 Hz     |
| 3    | Forward      | 50 Hz     |
| 4    | Reverse      | 50 Hz     |
| 5    | Reverse      | 30 Hz     |
| 6    | Reverse      | 15 Hz     |
| 7    | Forward      | 15 Hz     |
| 🔁   | Repeat Cycle |           |

---


## ⏱️ Timing Configuration

* Step Time = **3 Seconds**
* Acceleration Time = **1 Second**
* Deceleration Time = **1 Second**


---


##  VFD Configuration

* Run Command Source → External Terminals
* Frequency Source → Multi-step Speed / Preset
* Acceleration Time → 1 sec
* Deceleration Time → 1 sec

---


##  Demo
[Watch The Video](video.mp4)
###  System Operation Video

Shows:

* Automatic speed transitions
* Forward & Reverse switching
* Real-time execution on hardware

---

## 📚 References

* Delta VFD Manual (Official Documentation)

---

## 🚀 Key Learning Outcomes

* PLC Sequential Control using Timers
* Interfacing PLC with VFD
* Multi-speed motor control
* Forward/Reverse logic implementation
* Real industrial wiring experience

---


# Real-Time Sensor Fault-Tolerant Control of DC-DC Converters in DC Microgrids

This repository contains the MATLAB/Simulink simulation files supporting the paper:

**📄 Citation:**  
Ouahabi, M. S., Benyounes, A., Barkat, S., Ihammouchen, S., Rekioua, T., Rabehi, A., El-Kenawy, E. M., & Alharbi, A. H.  
**"Real-Time Sensor Fault Tolerant Control of DC-DC Converters in DC Microgrids Using a Switching Unknown Input Observer."**  
*IEEE Access, 2025.*  
DOI: [10.1109/ACCESS.2025.3571650](https://doi.org/10.1109/ACCESS.2025.3571650)

---

## 🧠 System Description

The simulated DC Microgrid consists of the following:

- ⚡ **DGU 1**: A **boost converter** delivering **constant current** into the DC bus.
- ☀️ **DGU 2**: A **PV array + boost converter** operating under **MPPT** with **variable irradiance**, injecting **variable current**.
- 🪫 **Bidirectional DC-DC Converter**:
  - Connected to a **battery** (160V).
  - Maintains the **DC-bus voltage** at 380V.
  - Operates in **charge/discharge** mode based on power balance.
- 🔻 **Load Side**: A **buck converter** connected to a **variable resistive load**.
- 🌀 **Control**: All converters implement **dual-loop control** (inner current loop, outer voltage loop).

---

## 🔧 Overview

This work proposes a real-time **Sensor Fault-Tolerant Control (FTC)** strategy for DC-DC converters using a **Switching Unknown Input Observer (SW-UIO)**. Highlights:

- Tolerates multiple types of voltage/current sensor faults (including simultaneous and complete failures).
- Requires **no communication** (suitable for primary-level control).
- Enables **fast control reconfiguration** (~1μs) after fault detection.
- Designed to be computationally efficient for embedded use.

> **Note**: The fault scenarios in the simulations can be easily modified for custom testing.

---

## 🧪 Simulation Scenarios

This repository includes Simulink models that implement the four fault injection scenarios described in the paper:
1. Bias faults
2. Time-varying and noise faults
3. Intermittent and saturation faults
4. Sensor stuck and complete sensor failures

The simulation models allow flexible fault insertion and observer validation.


## 📈 Notes on Results

- The simulation results shown here are **more accurate than the real-time (OPAL-RT) results**, due to numerical solver precision and idealized computational speed.
- However, real-time performance is consistent and robust within hardware constraints.

---

## 🖥️ Requirements

- MATLAB R2018b or newer 
- Simulink


## 📬 Questions?

If you have any questions, suggestions, or would like to collaborate, feel free to contact me:  
📧 **mohammedsaid.ouahabi@univ-msila.dz**

---

## 📚 License

This repository and its content are shared under:  
**Attribution-NonCommercial-NoDerivatives 4.0 International (CC BY-NC-ND 4.0)**  
🔗 [License Details]([https://creativecommons.org/licenses/by-nc-nd/4.0/](https://creativecommons.org/licenses/by-nc-nd/4.0/))

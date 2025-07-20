# Real-Time Sensor Fault-Tolerant Control of DC-DC Converters in DC Microgrids

This repository provides the MATLAB/Simulink simulation files used in our research paper:

**📄 Citation:**  
Ouahabi, M. S., Benyounes, A., Barkat, S., Ihammouchen, S., Rekioua, T., Rabehi, A., El-Kenawy, E. M., & Alharbi, A. H.  
**"Real-Time Sensor Fault Tolerant Control of DC-DC Converters in DC Microgrids Using a Switching Unknown Input Observer."**  
*IEEE Access, 2025.*  
DOI: [10.1109/ACCESS.2025.3571650](https://doi.org/10.1109/ACCESS.2025.3571650)

---

## 🔧 Overview

This work proposes a real-time **Sensor Fault-Tolerant Control (FTC)** strategy for DC-DC converters in DC microgrids, based on a **Switching Unknown Input Observer (SW-UIO)**. The proposed method:
- Estimates arbitrary sensor faults (voltage & current) with high accuracy .
- Accommodates complete and simultaneous sensor failures.
- Operates **communication-free** and is suitable for primary-level control.
- Is validated using real-time simulations on an **OPAL-RT** platform.

---

## 🧪 Simulation Scenarios

The provided Simulink models reproduce the four main scenarios in the paper:
1. **Scenario 1:** Positive & negative bias faults.
2. **Scenario 2:** Time-varying and random noise faults.
3. **Scenario 3:** Intermittent and saturation faults.
4. **Scenario 4:** Sensor stuck and complete sensor failure.





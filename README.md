# Electric Vehicle Battery Management System (BMS)

This repository contains a comprehensive software-based Battery Management System (BMS) developed for Electric Vehicle (EV) lithium-ion battery packs using MATLAB and Simulink. The system integrates State-of-Charge (SOC) estimation using an Extended Kalman Filter, thermal management with PID control, cell balancing algorithms, safety and protection mechanisms, and machine learning models for charging time prediction.

---

## Key Features

### Battery Pack Modeling
- Lithium-ion 18650 cell model with electrical and thermal characteristics
- Configured as 10S1P pack (10 cells in series, 1 parallel string)
- Sensor modeling for voltage, current, and temperature

### SOC/SOH Estimation
- Extended Kalman Filter (EKF) based SOC estimation
- Considers thermal coupling and sensor noise
- Accurate tracking under dynamic operating conditions

### Thermal Management System
- Heat generation and thermal behavior modeling
- PID-based cooling system for safe temperature regulation
- Active safety interlocks for over-temperature scenarios

### Cell Balancing
- Voltage-based and SOC-based passive balancing strategies
- Ensures uniform charge distribution across cells
- Thermal-aware balancing control logic

### Protection and Safety System
- Multi-layer fault detection (overvoltage, undervoltage, overcurrent, thermal fault)
- Stateflow-based protection state machine
- Emergency cut-off and system safety logic

### Machine Learning Integration
- Charging duration prediction model
- Explainability support (SHAP-based interpretation)
- Parameter tuning and predictive charging strategy

### End-to-End Simulink System
- Fully integrated model combining EKF, thermal control, balancing, and safety logic
- Supports embedded code generation and HIL readiness
- Visualization scripts for simulation analysis

---

## System Flow Diagram 
<img width="822" height="601" alt="Screenshot 2025-11-05 at 9 45 36 PM" src="https://github.com/user-attachments/assets/a3283b6a-0a37-4a2a-84b0-d9ed0194ea2f" />

---

## How To Use
1. Install MATLAB with required toolboxes:
   - Simulink  
   - Simscape Battery  
   - Stateflow  
   - Control System Toolbox  

2. Open the model file  
   `BMS_Complete_System.slx`

3. Run the model simulation

4. Inspect system outputs:
   - SOC trends
   - Temperature variation
   - Cell balancing behavior
   - Protection state activities

5. Modify system parameters to match your battery pack specifications

Overview
This project presents a comprehensive software-based Battery Management System (BMS) for Electric Vehicle (EV) batteries using MATLAB Simulink. The system includes advanced features like state-of-charge (SOC) estimation using an Extended Kalman Filter, thermal management with PID control, cell balancing algorithms, and fault protection modules. Additionally, it integrates machine learning models for intelligent charging duration prediction.
Project Phases
Phase 1: MATLAB Setup
	•	Installed MATLAB with required toolboxes: Simulink, Simscape Battery, Stateflow, Control System Toolbox.
	•	Verified example battery models and toolboxes.
Phase 2: Battery Pack Modeling
	•	Created 18650 Li-ion battery cell parameters with thermal properties.
	•	Configured battery pack as 10S1P (10 cells in series, 1 parallel string).
Phase 3: Advanced SOC Estimation
	•	Developed Extended Kalman Filter for accurate SOC estimation considering thermal effects and sensor noise.
  Phase 4: Thermal Management System
	•	Modeled heat generation and dissipation.
	•	Designed PID-based active cooling system to maintain safe battery temperature.
Phase 5: Cell Balancing Algorithm
	•	Implemented voltage-based and SOC-based passive balancing techniques.
	•	Included safety interlocks for temperature and voltage thresholds.
Phase 6: Protection System
	•	Designed multi-layer protection logic (overvoltage, undervoltage, overcurrent, thermal fault).
	•	Implemented Stateflow state machine for safety state management.
Phase 7: Machine Learning Integration
	•	Incorporated ML models for charging duration predictions to optimize battery charging strategy.
  Phase 8: Complete Simulink Model
	•	Combined all modules into a single Simulink model for end-to-end simulation.
Phase 9: Simulation and Visualization
	•	Simulated battery behavior, SOC, temperature, balancing and protection states.
	•	Visualized results with graphs for analysis.
Phase 10: Advanced Features
	•	Added explainability tools such as SHAP integration for ML model insights.
	•	Prepared for real-time embedded deployment (code generation).
System Flow Diagram
<img width="814" height="592" alt="Screenshot 2025-11-05 at 9 41 03 PM" src="https://github.com/user-attachments/assets/c446517f-eb0e-4adf-a194-7d100684566a" />
How to Use
	1.	Open the Simulink model file `BMS_Complete_System.slx` in MATLAB.
	2.	Run the simulation to evaluate battery charging scenarios.
	3.	Analyze the simulation outputs using the included visualization scripts.
	4.	Modify parameters as per your battery specifications and requirements.
	5.	Integrate your trained machine learning model for charging optimization.

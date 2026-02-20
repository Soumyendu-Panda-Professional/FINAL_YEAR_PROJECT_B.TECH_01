# FINAL_YEAR_PROJECT_B.TECH_01

# Mixed-Signal AI Accelerator 

## Description

This project implements a hardware-software co-design of a mixed-signal AI accelerator tailored for real-time fault detection in robotics. By integrating an Analog Front-End with a custom digital hardware accelerator, the system enables low-latency inference directly at the sensor level. This architecture eliminates the need for external processors, significantly optimizing power efficiency for autonomous edge devices.

---

## System Architecture

The system is divided into three primary domains to ensure a seamless signal chain from sensing to decision-making:

* **Analog Domain:** Handles signal sensing, amplification, and noise filtering using transistor-level CMOS design.


* **Software Domain:** Used for AI model training, weight optimization, and quantization mapping.


* **Digital Domain:** Features RTL-based logic for low-power inference, control, and classification.



## Project Workflow

The implementation follows a phase-by-phase co-design methodology:

1. **AI Model Development:** Training a Multi-Layer Perceptron (MLP) on vibration time-series data and quantizing weights for hardware compatibility.


2. **Analog Front-End Design:** Implementing a CMOS Operational Amplifier to condition weak sensor signals for processing.


3. **Data Conversion Interface:** Utilizing a virtual interface to map analog signal ranges into digital representations.


4. **Hardware Acceleration:** Developing Verilog-based MAC units and finite state machines (FSM) for synchronized digital processing.


5. **Simulation & Verification:** Conducting functional verification and power analysis to ensure accuracy against the software model.


6. **Physical Implementation:** Synthesizing the design for FPGA platforms to demonstrate real-time classification.



## Research Impact

* **Complete Co-Design:** Demonstrates a full workflow from analog circuits to digital logic.


* **Edge Optimization:** Utilizes integer quantization to achieve high-speed inference with minimal power overhead.


* **Real-Time Performance:** Enables immediate fault detection suitable for next-generation autonomous systems.


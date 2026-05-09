# VLSI Design & Physical Verification Portfolio

## Overview
This repository contains a comprehensive portfolio documenting advanced concepts in VLSI Design and Physical Verification. It covers analog signal processing, custom standard cell design, pipeline delay analysis, and memory array architecture. 

The full compiled document includes detailed schematics, pre- and post-layout extraction data, and hardware characterization graphs.

**[📄 Click here to view the full PDF Portfolio](./Portfolio_VLSI(2).pdf)**

## EDA Toolchain
* **Cadence Virtuoso Suite**: Schematic entry, logic verification, custom layout, DRC, LVS, and RC parasitic extraction.
* **LTspice**: Analog circuit simulation and verification.

## Core Competencies Demonstrated
* Continuous-Time Analog Signal Processing 
* Operational Mirrored Amplifiers (OMA) & Translinear Circuits
* Full Custom Physical Layout (DRC, LVS, and RC Parasitic Extraction)
* Logical Effort & Pipeline Delay Analysis
* Memory Array Architecture (ROM Implementation)

---

## Project Phases & Highlights

### Phase 1: Analog IC Design & Current-Mode Signal Processing
* **Operational Mirrored Amplifier (OMA):** Designed and characterized current followers, proving that a Cascode Current Mirror effectively mitigates the Early effect and extends operational bandwidth compared to simple mirrors.
* **Constant Bandwidth Variable Gain Amplifier (CFOA):** Demonstrated the decoupling of gain and bandwidth using an AD844 CFOA architecture, overcoming traditional Gain-Bandwidth (GBW) limitations of standard Voltage Feedback Amplifiers.
* **Translinear Current Squarer:** Validated a precision current squarer circuit utilizing the translinear principle for analog computation, proven both via simulation and hardware prototypes.
* **Negative Impedance Converter (NIC):** Implemented a CCII+ based NIC for parasitic resistance cancellation and Voltage Controlled Resistor (VCR) applications.
* **Two-CFOA Universal Multifunction Filter:** Designed a unified voltage-mode biquad filter capable of realizing Low-Pass, High-Pass, Band-Pass, Notch, and All-Pass responses simultaneously.

### Phase 2: Standard Cell Physical Design & Characterization
* Full physical design flow from schematic entry to layout generation for fundamental CMOS logic gates.
* **CMOS Inverter, NAND2, and NOR2 Gates:** Performed DRC and LVS checks, followed by RC extraction. 
* Conducted rigorous post-layout delay analysis, identifying the impact of parasitic capacitance ($C_{par}$) on signal integrity and propagation delays.

### Phase 3: Technology Node Scaling Analysis
* Evaluated 3-Input standard cells across multiple technology nodes: $0.35\mu m$, $0.18\mu m$, and 45nm.
* Analyzed scaling effects, noting that while 45nm significantly improves switching speeds, the $0.18\mu m$ node provided the best balance between speed and simulation reliability against parasitic sensitivity.

### Phase 4: Pipeline Delay & Logical Effort
* Investigated logic pipeline delays involving unit inverters driving NAND2 and NOR2 gates.
* Applied **Logical Effort** principles to size gates properly, demonstrating that scaling a NOR2 gate to balance input capacitance prevents significant propagation delay penalties in previous stages.

### Phase 5: Advanced Logic Styles & Limitations
* Evaluated Pass Transistor Logic (PTL) architectures.
* Demonstrated inherent signal degradation limits—specifically showing NMOS passing a "Weak 1" and PMOS passing a "Weak 0"—validating the necessity of CMOS Transmission Gates for full-swing logic.

### Phase 6: Memory Architecture Implementation
* **4x4 NOR ROM Array:** Designed the physical layout using NMOS pull-down arrays, proving robust decoding isolation and word-line assertions through post-extraction verification.
* **4x4 NAND ROM Array:** Verified the dual architecture leveraging series MOS chains, successfully validating high-density word-line decoding mechanisms.

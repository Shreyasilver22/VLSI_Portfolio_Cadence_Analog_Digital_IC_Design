# VLSI Design & Physical Verification Portfolio

## Overview
[cite_start]This repository contains a comprehensive portfolio documenting advanced concepts in VLSI Design and Physical Verification[cite: 53]. [cite_start]It covers analog signal processing, custom standard cell design, pipeline delay analysis, and memory array architecture[cite: 54, 58]. 

[cite_start]The full compiled document includes detailed schematics, pre- and post-layout extraction data, and hardware characterization graphs[cite: 56].

**[📄 Click here to view the full PDF Portfolio](./Portfolio_VLSI.pdf)** *(Make sure to update this link with your actual file name)*

## EDA Toolchain
* [cite_start]**Cadence Virtuoso Suite**: Schematic entry, logic verification, custom layout, DRC, LVS, and RC parasitic extraction[cite: 55, 58].
* [cite_start]**LTspice**: Analog circuit simulation and verification[cite: 55].

## Core Competencies Demonstrated
* [cite_start]Continuous-Time Analog Signal Processing [cite: 58]
* [cite_start]Operational Mirrored Amplifiers (OMA) & Translinear Circuits [cite: 58]
* [cite_start]Full Custom Physical Layout (DRC, LVS, and RC Parasitic Extraction) [cite: 58]
* [cite_start]Logical Effort & Pipeline Delay Analysis [cite: 58]
* [cite_start]Memory Array Architecture (ROM Implementation) [cite: 58]

---

## Project Phases & Highlights

### Phase 1: Analog IC Design & Current-Mode Signal Processing
* [cite_start]**Operational Mirrored Amplifier (OMA):** Designed and characterized current followers, proving that a Cascode Current Mirror effectively mitigates the Early effect and extends operational bandwidth compared to simple mirrors[cite: 69, 70, 99, 127].
* [cite_start]**Constant Bandwidth Variable Gain Amplifier (CFOA):** Demonstrated the decoupling of gain and bandwidth using an AD844 CFOA architecture, overcoming traditional Gain-Bandwidth (GBW) limitations of standard Voltage Feedback Amplifiers[cite: 139, 140].
* [cite_start]**Translinear Current Squarer:** Validated a precision current squarer circuit utilizing the translinear principle for analog computation, proven both via simulation and hardware prototypes[cite: 151, 152].
* [cite_start]**Negative Impedance Converter (NIC):** Implemented a CCII+ based NIC for parasitic resistance cancellation and Voltage Controlled Resistor (VCR) applications[cite: 197, 198, 222].
* [cite_start]**Two-CFOA Universal Multifunction Filter:** Designed a unified voltage-mode biquad filter capable of realizing Low-Pass, High-Pass, Band-Pass, Notch, and All-Pass responses simultaneously[cite: 224, 225].

### Phase 2: Standard Cell Physical Design & Characterization
* [cite_start]Full physical design flow from schematic entry to layout generation for fundamental CMOS logic gates[cite: 278].
* [cite_start]**CMOS Inverter, NAND2, and NOR2 Gates:** Performed DRC and LVS checks, followed by RC extraction[cite: 281, 353, 409, 410]. 
* [cite_start]Conducted rigorous post-layout delay analysis, identifying the impact of parasitic capacitance ($C_{par}$) on signal integrity and propagation delays[cite: 307, 406, 407].

### Phase 3: Technology Node Scaling Analysis
* [cite_start]Evaluated 3-Input standard cells across multiple technology nodes: $0.35\mu m$, $0.18\mu m$, and 45nm[cite: 455, 457].
* [cite_start]Analyzed scaling effects, noting that while 45nm significantly improves switching speeds, the $0.18\mu m$ node provided the best balance between speed and simulation reliability against parasitic sensitivity[cite: 487, 488, 489].

### Phase 4: Pipeline Delay & Logical Effort
* [cite_start]Investigated logic pipeline delays involving unit inverters driving NAND2 and NOR2 gates[cite: 494].
* [cite_start]Applied **Logical Effort** principles to size gates properly, demonstrating that scaling a NOR2 gate to balance input capacitance prevents significant propagation delay penalties in previous stages[cite: 495, 502, 503].

### Phase 5: Advanced Logic Styles & Limitations
* [cite_start]Evaluated Pass Transistor Logic (PTL) architectures[cite: 507].
* [cite_start]Demonstrated inherent signal degradation limits—specifically showing NMOS passing a "Weak 1" and PMOS passing a "Weak 0"—validating the necessity of CMOS Transmission Gates for full-swing logic[cite: 514, 515, 516].

### Phase 6: Memory Architecture Implementation
* [cite_start]**4x4 NOR ROM Array:** Designed the physical layout using NMOS pull-down arrays, proving robust decoding isolation and word-line assertions through post-extraction verification[cite: 520, 524, 546].
* [cite_start]**4x4 NAND ROM Array:** Verified the dual architecture leveraging series MOS chains, successfully validating high-density word-line decoding mechanisms[cite: 548, 551, 570].

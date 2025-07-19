
# CMOS SR Flip-Flop Design in Cadence Virtuoso (GPDK 90nm)

This repository presents the complete implementation of an **SR Flip-Flop** using **Cadence Virtuoso** with **GPDK 90nm technology**. The design includes schematic capture, symbol creation, simulation, layout, DRC/LVS checks, parasitic extraction, and energy analysis.

---

## Table of Contents  
- [Schematic](#schematic)  
- [Symbol View](#symbol-view)  
- [Testbench](#testbench)  
- [Transient Simulation](#transient-simulation)  
- [Layout](#layout)  
- [DRC and LVS Checks](#drc-and-lvs-checks)  
- [Schematic vs Layout Matching](#schematic-vs-layout-matching)  
- [Parasitic Extraction (RCX)](#parasitic-extraction-rcx)  
- [AV Extracted View](#av-extracted-view)  
- [Energy Analysis](#energy-analysis)  
- [Tools Used](#tools-used)  
- [Author](#author)

---

## Schematic  
The SR Flip-Flop circuit was designed using basic logic gates following standard flip-flop design principles.

![Schematic](./SR_Flip_flop_schematic.png)

---

## Symbol View  
A reusable symbol view of the SR Flip-Flop was created for easy integration into larger designs.

![Symbol](./SR_Flip_flop_symbol.png)

---

## Testbench  
The testbench validates the operation of the flip-flop using a set of predefined input conditions.

![Testbench](./SR_Flip_flop_tb.png)

---

## Transient Simulation  
Transient analysis confirms the expected behavior of the SR Flip-Flop over time.

![Transient Waveform](./SR_Flip_Flop_transient.png)

---

## Layout  
Physical implementation of the SR Flip-Flop following the design rules of GPDK 90nm.

![Layout](./Layout_SR_Flip_Flop.png)

---

## DRC and LVS Checks

### DRC: Design Rule Check  
Layout is verified to be free of design rule violations.

![DRC](./NO_DRC_SR_Flip_Flop.png)

### LVS: Layout vs Schematic  
Layout is confirmed to match the schematic connectivity.

![LVS](./LVS_Run_SR_Flip_Flop.png)

---

## Schematic vs Layout Matching  
Graphical confirmation of matched schematic and layout topologies.

![Layout vs Schematic](./Layout_and_Schematic_match_SR_Flip_flop.png)

---

## Parasitic Extraction (RCX)  
Parasitic elements are extracted using RCX for post-layout simulation accuracy.

![RCX](./RCX_Run_SR_Flip_flop.png)

---

## AV Extracted View  
The extracted view includes parasitic capacitance and resistance for post-layout simulations.

![AV Extracted View](./AV_Extracted_view_SR_Flip_flop.png)

---

## Energy Analysis  
Estimation of energy consumption per switching event.

![Energy Estimation](./Energy_estimation_SR_Flip_flop.png)

---

## Tools Used  
- **Cadence Virtuoso** for design and simulation  
- **GPDK 90nm PDK**  
- **Assura** for DRC, LVS, and RC extraction  
- **Spectre Simulator** for transient analysis

---

## Author  
**Ram Tripathi**

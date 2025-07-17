# CMOS SR Latch Using NOR Gates in Cadence Virtuoso

This repository contains the design and simulation of an **SR Latch using NOR gates** using **GPDK 90nm** technology in **Cadence Virtuoso**. It includes schematic design, symbol creation, testbench setup, transient simulation, custom layout, and verification steps like DRC, LVS, RCX, and energy estimation.

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
The SR latch is implemented using cross-coupled NOR gates, forming a basic memory element.

![Schematic](./SR_Latch_using_NOR_Schematic.png)

---

## Symbol View  
A simplified symbol was created to use in higher-level designs and testbenches.

![Symbol](./SR_Latch_using_NOR_Gates.png)

---

## Testbench  
The testbench applies input vectors to verify the functional behavior of the SR latch.

![Testbench](./SR_Latch_using_NOR_Tb.png)

---

## Transient Simulation  
Simulation results show expected output behavior based on input combinations, confirming correct latch functionality.

![Transient Waveform](./SR_Latch_using_NOR_Transient_waveform.png)

---

## Layout  
Custom layout was drawn using 90nm standard cell design rules in Cadence Virtuoso.

![Layout](./LAYOUT_SR_Latch_using_NOR.png)

---

## DRC and LVS Checks

### DRC: Design Rule Check  
No violations were found; layout is clean.

![DRC](./NO_DRC_SR_LATCH_usimg_NOR.png)

### LVS: Layout vs Schematic  
Schematic and layout netlists matched successfully.

![LVS](./LVS_RUN_SR_Latch_using_NOR.png)

---

## Schematic vs Layout Matching  
Shows correspondence between designed schematic and physical layout.

![Match](./Layout_and_schematic_match_SR_Latch_using_NOR_Gate.png)

---

## Parasitic Extraction (RCX)  
RCX extraction adds parasitic capacitance and resistance for post-layout simulation.

![RCX](./RCX_Run_SR_Latch_using_NOR.png)

---

## AV Extracted View  
The AV view represents the extracted design including parasitics.

![AV Extracted View](./AV_Extracted_view_SL_Latch_using_NOR.png)

---

## Energy Analysis  
Energy estimation performed for one complete cycle using post-layout data.

![Energy](./Energy_estimation_SR_Latch_using_NOR.png)

---

## Tools Used  
- **Cadence Virtuoso** with **GPDK 90nm**  
- **Assura DRC/LVS/RCX**  
- **Spectre ADE** for transient simulations

---

## Author  
**Ram Tripathi**

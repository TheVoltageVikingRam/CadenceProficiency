
# CMOS 4-Bit OR Gate Design in Cadence Virtuoso

This repository documents the full design, simulation, and verification process of a **4-Bit OR Gate** implemented using **Cadence Virtuoso**. The project includes schematic design, layout drawing, DRC/LVS verification, RC parasitic extraction, and transient simulation.

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
- [Tools Used](#tools-used)  
- [Author](#author)

---

## Schematic  
The 4-bit OR gate is constructed using multiple 2-input OR gates in CMOS logic. It performs a bitwise OR on two 4-bit inputs.

![Schematic](./4_Bit_OR_Gate_Schematic.png)

---

## Symbol View  
A symbol view was created for hierarchical design, simplifying connections in the testbench and top-level design.

![Symbol](./4_bit_OR_gate_symbol.png)

---

## Testbench  
The testbench stimulates the 4-bit OR gate with a variety of input combinations to verify its truth table.

![Testbench](./4_bit_OR_Gate_test_bench.png)

---

## Transient Simulation  
Transient analysis confirms that the 4-bit OR gate performs as expected, outputting the correct logic OR for each bit.

![Transient](./4_BIT_OR_gate_Transient_waveform.png)

---

## Layout  
The layout of the 4-bit OR gate was created using Cadence Virtuoso layout editor while adhering to all design rules.

![Layout](./Layout_4_bit_OR_Gate.png)

---

## DRC and LVS Checks

### DRC: Design Rule Check  
No DRC errors were found, confirming the layout complies with fabrication constraints.

![DRC Clearance](./No_DRC_Errors.png)

### LVS: Layout vs Schematic  
The LVS check shows the layout matches the schematic. A minor warning (non-critical) was observed during debug.

![LVS Run](./LVS_Run.png)  
![LVS Debug](./LVS_Debug_no_extraction_warning.png)

---

## Schematic vs Layout Matching  
This visual validation ensures that the physical layout matches the schematic structure and connectivity.

![Match View](./Layout_and_schematic_match.png)

---

## Parasitic Extraction (RCX)  
RCX analysis was performed to extract parasitic resistances and capacitances from the layout for accurate timing simulations.

![RCX Run](./RCX_Run.png)

---

## AV Extracted View  
The Annotated View shows the netlist after RC extraction, including parasitics for back-annotated simulation.

![AV Extracted View](./AV_extracted_view.png)

---

## Tools Used  
- **Cadence Virtuoso** – Schematic & Layout Design  
- **Assura** – DRC, LVS, and RCX Extraction  
- **Spectre / ADE L/XL** – Simulation & Waveform Analysis  

---

## Author  
**Ram Tripathi**

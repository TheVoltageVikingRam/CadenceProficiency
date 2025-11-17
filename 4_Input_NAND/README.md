# NAND4 Gate Design in Cadence Virtuoso

This repository demonstrates the full-custom VLSI design of a **4-input NAND (NAND4) Gate** using Cadence Virtuoso.  
It includes the schematic, symbol, layout, extracted view, testbench, LVS, and verification images.

---

## Table of Contents
- [Schematic](#schematic)
- [Symbol](#symbol)
- [Testbench](#testbench)
- [Prelayout Transient](#prelayout-transient)
- [Layout](#layout)
- [DRC Clean Layout](#drc-clean-layout)
- [Extracted View](#extracted-view)
- [LVS Results](#lvs-results)
- [Tools Used](#tools-used)
- [Author](#author)

---

## Schematic
The NAND4 schematic designed in Cadence Virtuoso.

![NAND4 Schematic](NAND4_SCHEMATIC.png)

---

## Symbol
Custom symbol created for use in the testbench.

![NAND4 Symbol](nand4_symbol.png)

---

## Testbench
Testbench used to verify logic and transient behavior.

![NAND4 Testbench](NAND4_TB.png)

---

## Prelayout Transient
Prelayout transient / prelayout reference waveform.

![SRAM Prelayout Simulation](SRAM_Cadence_Simulation_Prelayout.png)

---

## Layout
Initial layout of the NAND4 gate.

![NAND4 Layout](Layout_NAND4.png)

---

## DRC Clean Layout
Layout after fixing Design Rule Check (DRC) violations.

![DRC Clean Layout](NAND_4_Layout_No_DRC.png)

---

## Extracted View
Extracted layout used for post-layout simulation.

![Extracted View](av_extracted_view_nand4.png)

---

## LVS Results
Layout vs Schematic (LVS) verification and transient comparison.

### LVS Comparison Window
![LVS Comparison](layout_vs_schematic_comparison.png)

### LVS Match – No Mismatch
![LVS Match](nand4_no_Lvs_mismatch.png)

### Layout and Schematic Comparison at Switching
![Layout vs Schematic - minimal differences](nand4_schematic_vs_layout_very_minimal_difference.png)

---

## Tools Used
- Cadence Virtuoso — schematic & layout
- Spectre — simulations
- Assura (or your DRC/LVS tool) — DRC & LVS checks

---

## Author
**Ram Tripathi (22HEL2231)**  
BSc (Hons.) Electronics — Final Year Project

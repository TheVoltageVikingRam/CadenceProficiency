# CMOS Inverter Design in Cadence Virtuoso  

This demonstrates the design and simulation of a **CMOS Inverter** using **Cadence Virtuoso**. It includes the **schematic, layout, testbench circuit, and output waveforms**.  

## Table of Contents  
- [Schematic](#schematic)  
- [Layout](#layout)  
- [Testbench Circuit](#testbench-circuit)  
- [Simulation and Output Waveform](#simulation-and-output-waveform)  
- [Tools Used](#tools-used)  
- [Parametric Analysis](#Parametric-Analysis)
---

## Schematic  
The schematic of the CMOS inverter is designed using **Cadence Virtuoso**.  

![Schematic](inverter.png)  

---

## Layout  
The layout follows **design rules (DRC)** and has been verified for **LVS**.  

![Layout](layoutview.png)  

---

## Testbench Circuit  
The testbench is designed to verify the functionality of the CMOS inverter.  

![Testbench](sim.png)  

---

## Simulation and Output Waveform  
The waveform below shows the CMOS inverter's response to different input conditions.  

![Output Waveform](Output_Record.png)  

---

## Extracted View 
  

![Layout](Extracted_View.png)  

---

## Layout vs Scheamtic Transient Response  
  

![LVS](LAYOUT_VS_SCHEMATIC_TR_RESPONSE.png)  

---
## Propagation Delay  
  

![Propataion Delay](Propgation_Delay_inADE_XL.png)  

---
## Parametric Analysis
Parametric Analysis of Inverter Circuit by varying Gate width of PMOS and NMOS.

![Parametric Analysis](Parametric_Analysis_of_CMOS_Inv.png)

---
## Tools Used  
- **Cadence Virtuoso** – Schematic and Layout Design  
- **Spectre Simulator** – Circuit Simulation  
- **Assura / Calibre** – DRC & LVS Checks  

---

## Author  
**Ram Tripathi**  

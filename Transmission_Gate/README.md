# 🔀 Transmission Gate using GPDK 90nm

This repository showcases the complete analog design flow of a **Transmission Gate**, implemented using **Cadence Virtuoso** with the **GPDK 90nm** technology. It includes schematic design, layout, simulation, verification, and energy analysis.

---

## 📚 Table of Contents

- [🧰 Schematic](#-schematic)
- [📐 Symbol](#-symbol)
- [🧪 Testbench](#-testbench)
- [📊 Transient Response](#-transient-response)
- [⚡ Spectral Power Analysis](#-spectral-power-analysis)
- [🔋 Energy Estimation](#-energy-estimation)
- [🏗️ Layout](#-layout)
- [✅ DRC Check](#-drc-check)
- [🔍 LVS Check](#-lvs-check)
- [🧩 Layout vs Schematic Match](#-layout-vs-schematic-match)
- [🧠 RCX Extraction](#-rcx-extraction)
- [📡 AV Extracted View](#-av-extracted-view)
- [🛠️ Tools Used](#-tools-used)
- [👨‍💻 Author](#-author)

---

## 🧰 Schematic

Schematic of the Transmission Gate drawn in Cadence Virtuoso.

![Schematic](Transmission_Gate_Schematic.png)

---

## 📐 Symbol

Hierarchical symbol created for simulation testbench connectivity.

![Symbol](Transmission_gate_symbol.png)

---

## 🧪 Testbench

Testbench circuit used for transient and power simulations.

![Testbench](Transmission_gate_tb.png)

---

## 📊 Transient Response

Transient simulation showing gate functionality over time.

![Transient](Transmission_Gate_transient_waveform.png)

---

## ⚡ Spectral Power Analysis

Power waveform from simulation, showing dynamic power consumption.

![Spectral Power](Transmission_gate_spectral_power.png)

---

## 🔋 Energy Estimation

Calculated energy usage based on simulation data.

![Energy Estimation](Energy_Estimation_transmission_gate.png)

---

## 🏗️ Layout

Full-custom layout designed for DRC compliance.

![Layout](Layout_Transmission_Gate.png)

---

## ✅ DRC Check

Design Rule Check passed without errors.

![No DRC](No_DRC_Transmission_Gate.png)

---

## 🔍 LVS Check

Layout Versus Schematic verified and matched.

![LVS](LVS_Run_Transmission_gate.png)

---

## 🧩 Layout vs Schematic Match

Visual confirmation of matching layout and schematic.

![Layout Match](Layout_and_schematic_match_transmission_gate.png)

---

## 🧠 RCX Extraction

Parasitic RC extraction using post-layout view.

![RCX](RCX_Run_transmission_gate.png)

---

## 📡 AV Extracted View

Annotated view for simulation with extracted parasitics.

![AV View](AV_Extracted_view_tranmission_gate.png)

---

## 🛠️ Tools Used

- **Cadence Virtuoso** – Schematic, Layout & Simulation  
- **Spectre** – Transient and Power Simulations  
- **Assura/Calibre** – DRC & LVS  
- **QRC/RCX** – Parasitic Extraction  
- **GPDK 90nm** – Technology Library  

---

## 👨‍💻 Author

**Ram Tripathi**  
B.Tech – Electronics and Communication Engineering  
Analog IC Design Enthusiast

---

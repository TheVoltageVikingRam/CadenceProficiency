
# 🔀 Transmission Gate using GPDK 90nm

This repository showcases the complete analog design flow of a **Transmission Gate** implemented using **Cadence Virtuoso** with the **GPDK 90nm** technology. The project includes schematic capture, layout, simulations, verification, and power analysis.

---

## 📚 Table of Contents

- [🧰 Schematic](#-schematic)
- [📐 Symbol](#-symbol)
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

The schematic of the Transmission Gate circuit drawn in Virtuoso.

![Schematic](Transmission_Gate_Schematic.png)

---

## 📐 Symbol

The symbol created for hierarchical design and testbench connections.

![Symbol](Transmission_gate_symbol.png)

---

## 📊 Transient Response

Transient waveform showing the switching characteristics of the transmission gate.

![Transient Response](Transmission_Gate_transient_waveform.png)

---

## ⚡ Spectral Power Analysis

Power waveform captured using Virtuoso's waveform viewer.

![Spectral Power](Transmission_gate_spectral_power.png)

---

## 🔋 Energy Estimation

Estimated energy consumed during operation of the transmission gate.

![Energy Estimation](Energy_Estimation_transmission_gate.png)

---

## 🏗️ Layout

Full-custom layout of the Transmission Gate in compliance with 90nm design rules.

![Layout](Layout_Transmission_Gate.png)

---

## ✅ DRC Check

Design Rule Check passed successfully with no errors.

![DRC](No_DRC_Transmission_Gate.png)

---

## 🔍 LVS Check

Layout Versus Schematic (LVS) verified and passed.

![LVS](LVS_Run_Transmission_gate.png)

---

## 🧩 Layout vs Schematic Match

Confirmation of matching connectivity between layout and schematic.

![Match](Layout_and_schematic_match_transmission_gate.png)

---

## 🧠 RCX Extraction

Post-layout RC extraction for accurate simulation.

![RCX](RCX_Run_transmission_gate.png)

---

## 📡 AV Extracted View

Annotated view showing extracted parasitics for simulation.

![AV View](AV_Extracted_view_tranmission_gate.png)

---

## 🛠️ Tools Used

- **Cadence Virtuoso** – Schematic & Layout Design  
- **Spectre Simulator** – Transient, power, and energy simulations  
- **Assura** – DRC and LVS verification  
- **RCX** – Parasitic Extraction  
- **GPDK 90nm** – Technology library  

---

## 👨‍💻 Author

**Ram Tripathi**  


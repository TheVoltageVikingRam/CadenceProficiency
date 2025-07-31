
# 🔁 Schmitt Trigger using GPDK 90nm

This repository contains the complete design flow of a **Schmitt Trigger** circuit implemented using the **GPDK 90nm** technology node in **Cadence Virtuoso**. It includes schematic design, layout, simulation results, verification checks, and energy estimation.

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

This is the core schematic of the Schmitt Trigger designed in Virtuoso.

![Schematic](Schematic_schmitt_trigger.png)

---

## 📐 Symbol

The symbol generated for reuse and easier testbench integration.

![Symbol](Schmitt_trigger_symbol.png)

---

## 🧪 Testbench

Testbench to verify transient response and hysteresis behavior.

![Testbench](Schmitt_trigger_tb.png)

---

## 📊 Transient Response

Output waveform showing hysteresis behavior of the Schmitt Trigger.

![Transient Waveform](Schmitt_trigger_transient_waveform.png)

---

## ⚡ Spectral Power Analysis

Power waveform captured over time using calculator and waveform tool.

![Spectral Power](Schmitt_trigger_Spectral_power_waveform.png)

---

## 🔋 Energy Estimation

Estimation of energy consumed during one switching cycle.

![Energy Estimation](Energy_Estimation_schmitt_trigger.png)

---

## 🏗️ Layout

Custom layout designed for the Schmitt Trigger circuit.

![Layout](Schmitt_trigger_Layout.png)

---

## ✅ DRC Check

Design Rule Check (DRC) passed successfully with no violations.

![No DRC](Schmitt_Trigger_No_DRC.png)

---

## 🔍 LVS Check

Layout Versus Schematic (LVS) successfully completed.

![LVS](Schmitt_trigger_LVS_Run.png)

---

## 🧩 Layout vs Schematic Match

Physical layout matches schematic connectivity perfectly.

![Layout Match](Schmitt_trigger_Layout_vs_Schematic_match.png)

---

## 🧠 RCX Extraction

RC parasitic extraction performed for post-layout simulation.

![RCX](Schmitt_trigger_RCX_Run.png)

---

## 📡 AV Extracted View

View of the extracted netlist including parasitics for accurate post-layout simulation.

![AV Extracted](Schmitt_trigger_AV_Extracted_view.png)

---

## 🛠️ Tools Used

- **Cadence Virtuoso** – Schematic & Layout Design  
- **Spectre Simulator** – Transient, power, and energy simulations  
- **Assura** – DRC and LVS verification  
- **RCX** – RC Extraction  
- **Virtuoso Waveform Viewer** – Signal and power plotting  
- **GPDK 90nm** – Process Design Kit  

---

## 👨‍💻 Author

**Ram Tripathi**  



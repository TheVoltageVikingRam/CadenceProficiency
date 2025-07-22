# 📘 Common Source Amplifier (CS Amp) – GPDK 90nm

This project demonstrates the design, layout, and analysis of a **Common Source Amplifier** using the **GPDK 90nm** technology in **Cadence Virtuoso**. The design includes schematic capture, layout, verification (DRC/LVS/RCX), and simulation (transient and DC), along with energy and power estimation.

---

## 📂 Table of Contents

- [1️⃣ Schematic](#1️⃣-schematic)
- [2️⃣ Testbench](#2️⃣-testbench)
- [3️⃣ Transient & DC Response](#3️⃣-transient--dc-response)
- [4️⃣ Layout](#4️⃣-layout)
- [5️⃣ DRC Check](#5️⃣-drc-check)
- [6️⃣ LVS Verification](#6️⃣-lvs-verification)
- [7️⃣ Layout vs Schematic Match](#7️⃣-layout-vs-schematic-match)
- [8️⃣ RC Extraction (RCX)](#8️⃣-rc-extraction-rcx)
- [9️⃣ AV Extracted View](#9️⃣-av-extracted-view)
- [🔟 Energy and Power Estimation](#🔟-energy-and-power-estimation)
- [🛠 Tools Used](#🛠-tools-used)
- [👤 Author](#👤-author)

---

## 1️⃣ Schematic

Basic schematic of a common source amplifier using NMOS and passive load.

![Schematic](./Common_source_amplifier_schematic.png)

---

## 2️⃣ Testbench

Simulation setup used to verify amplifier behavior.

![Testbench](./CS_Amp_tb.png)

---

## 3️⃣ Transient & DC Response

### 📈 Transient Response

Shows amplifier gain and performance with AC input.

![Transient Response](./Transient_Response_CS_amp.png)

### 🧾 DC Sweep

Shows transfer characteristics and operating region.

![DC Response](./dc_response.png)

---

## 4️⃣ Layout

Physical design of the common source amplifier.

![Layout](./Lyout_CS_Amp.png)

---

## 5️⃣ DRC Check

Design passes all physical design rules.

![DRC](./No_DRC_CS_amp.png)

---

## 6️⃣ LVS Verification

Layout successfully matches the schematic netlist.

![LVS](./LVS_Run_CS_Amp.png)

---

## 7️⃣ Layout vs Schematic Match

Visual overlay confirming device and net matching.

![Layout vs Schematic](./Layout_and_schematic_match_CS_amp.png)

---

## 8️⃣ RC Extraction (RCX)

Parasitics extracted to analyze post-layout behavior.

![RCX](./RCX_Run_CS_Amp.png)

---

## 9️⃣ AV Extracted View

Extracted view with parasitics for high-accuracy simulation.

![AV Extracted](./AV_Extracted_view_CS_Amp.png)

---


### ⚡ Power Curve

Time-dependent power profile during simulation.

![Power Curve](./Power_Curve.png)

---

## 🛠 Tools Used

- **Cadence Virtuoso** (Schematic/Layout)
- **Assura** (DRC, LVS, RCX)
- **Spectre** (Simulation)
- **Technology**: GPDK 90nm

---

## 👤 Author

**Ram Tripathi**

---


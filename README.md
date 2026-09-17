# ⚡ Substation Protection & Fault Analysis

## 📌 Project Overview

This project focuses on the **design, simulation, and protection analysis of a 33/11 kV, 5 MVA electrical substation** using **ETAP** and **AutoCAD Electrical**.

The project models a 33 kV incoming supply, 33/11 kV transformer, 11 kV bus, outgoing feeders, CTs, PTs, circuit breakers, and protection relays. The system is analyzed under different fault conditions to study **fault current, voltage disturbances, relay operation, and circuit-breaker response**.

The project demonstrates practical concepts related to **power systems, substation design, short-circuit analysis, electrical protection, and relay coordination**.

---

## 🎯 Objectives

* Design a **33/11 kV, 5 MVA substation** model.
* Develop the substation single-line diagram.
* Perform power-system analysis using ETAP.
* Analyze short-circuit fault conditions.
* Study fault current levels at different locations.
* Configure overcurrent and earth-fault protection.
* Analyze relay operating characteristics.
* Study circuit-breaker operation during faults.
* Perform protection coordination between primary and backup relays.
* Prepare electrical schematics using AutoCAD Electrical.

---

## 🏗️ System Architecture

```text
                         33 kV GRID
                             │
                             │
                       ┌─────▼─────┐
                       │  33 kV CB │
                       └─────┬─────┘
                             │
                       ┌─────▼─────┐
                       │   33 kV   │
                       │    BUS    │
                       └─────┬─────┘
                             │
                     ┌───────▼────────┐
                     │ 33/11 kV       │
                     │ 5 MVA          │
                     │ Transformer    │
                     └───────┬────────┘
                             │
                       ┌─────▼─────┐
                       │  11 kV CB │
                       └─────┬─────┘
                             │
                       ┌─────▼─────┐
                       │   11 kV   │
                       │    BUS    │
                       └───┬───┬───┘
                           │   │   │
                          F1  F2  F3
                           │   │   │
                       Feeder Feeder Feeder
```

---

## ⚙️ System Specifications

| Parameter          | Specification                    |
| ------------------ | -------------------------------- |
| Substation Type    | 33/11 kV Distribution Substation |
| Incoming Voltage   | 33 kV                            |
| Transformer Rating | 5 MVA                            |
| Transformer Ratio  | 33/11 kV                         |
| Secondary Voltage  | 11 kV                            |
| Outgoing Feeders   | 3                                |
| Protection         | Overcurrent & Earth Fault        |
| Instrumentation    | CTs & PTs                        |
| Switching          | Circuit Breakers                 |
| Simulation         | ETAP                             |
| Electrical Design  | AutoCAD Electrical               |

---

## 🛠️ Software & Tools

### Simulation

* **ETAP**
* Short-Circuit Analysis
* Load Flow Analysis
* Protection Coordination
* Relay Coordination

### Electrical Design

* **AutoCAD Electrical**
* Single-Line Diagram
* Protection Schematic
* Control/Wiring Diagram

---

# 🔬 Methodology

## 1. Substation Modeling

The complete electrical network is modeled in ETAP using:

* Utility/Grid
* 33 kV bus
* 33/11 kV transformer
* 11 kV bus
* Three outgoing feeders
* Loads
* Circuit breakers
* CTs and PTs
* Protection relays

---

## 2. Transformer Modeling

A **5 MVA, 33/11 kV transformer** is modeled as the main step-down transformer.

The transformer is analyzed for:

* Voltage transformation
* Loading
* Current levels
* Short-circuit contribution
* Protection requirements

---

## 3. Load Flow Analysis

Load-flow analysis is performed to evaluate the steady-state operating condition of the substation.

Parameters analyzed include:

* Bus voltage
* Branch current
* Active power
* Reactive power
* Power factor
* Transformer loading

---

# ⚠️ Fault Analysis

Five fault scenarios are considered in the study.

| Case | Fault Type           | Location        |
| ---- | -------------------- | --------------- |
| 1    | Three-Phase Fault    | 11 kV Bus       |
| 2    | Line-to-Ground Fault | 11 kV Bus       |
| 3    | Line-to-Line Fault   | 11 kV Bus       |
| 4    | Three-Phase Fault    | Outgoing Feeder |
| 5    | Line-to-Ground Fault | Outgoing Feeder |

For each fault, the following parameters are evaluated:

* Fault current
* Bus voltage
* Feeder current
* Fault location
* Relay response
* Circuit-breaker operation

---

# 🛡️ Protection System

## Overcurrent Protection

Overcurrent relays are used to detect abnormal increases in phase current.

The protection study considers:

* Pickup current
* Time-current characteristics
* Time multiplier/time dial
* Instantaneous protection where applicable

---

## Earth-Fault Protection

Earth-fault protection is used to detect current associated with ground faults.

The study evaluates:

* Earth-fault pickup
* Operating time
* Relay response
* Circuit-breaker trip operation

---

## Circuit Breaker Protection

Circuit breakers isolate the faulted section after receiving a trip signal from the protection relay.

The protection sequence is:

```text
Fault Occurs
     ↓
Current Increases
     ↓
Protection Relay Detects Fault
     ↓
Relay Issues Trip Command
     ↓
Circuit Breaker Opens
     ↓
Faulted Section Isolated
```

---

# 🔄 Relay Coordination

Protection coordination is performed to ensure appropriate selectivity between downstream and upstream protection devices.

```text
                  FAULT
                    │
                    ▼
             Primary Relay
                    │
                    ▼
          Primary Circuit Breaker
                    │
                    │
             Backup Protection
                    │
                    ▼
          Backup Circuit Breaker
```

The coordination study evaluates:

* Relay pickup
* Relay operating time
* Coordination margin
* Primary protection
* Backup protection
* Circuit-breaker operation

---

# 📊 Fault Analysis Results

The final results should be populated using values obtained directly from the ETAP simulation.

| Fault Case     | Fault Current | Minimum Voltage | Relay Operation | Breaker Operation |
| -------------- | ------------: | --------------: | --------------- | ----------------- |
| 3-Phase Bus    |           TBD |             TBD | TBD             | TBD               |
| L-G Bus        |           TBD |             TBD | TBD             | TBD               |
| L-L Bus        |           TBD |             TBD | TBD             | TBD               |
| 3-Phase Feeder |           TBD |             TBD | TBD             | TBD               |
| L-G Feeder     |           TBD |             TBD | TBD             | TBD               |

> **Note:** `TBD` values should be replaced only with results generated by the actual ETAP model.

---

# 📈 Protection Coordination Results

| Relay                | CT Ratio | Pickup | Operating Time | Curve |
| -------------------- | -------- | -----: | -------------: | ----- |
| Feeder Overcurrent   | TBD      |    TBD |            TBD | TBD   |
| Feeder Earth Fault   | TBD      |    TBD |            TBD | TBD   |
| Incoming Overcurrent | TBD      |    TBD |            TBD | TBD   |
| Incoming Earth Fault | TBD      |    TBD |            TBD | TBD   |

Add ETAP time-current characteristic (TCC) curves to the `results/` folder.

---

# 🖥️ AutoCAD Electrical Design

AutoCAD Electrical is used to document the electrical protection and control system.

The documentation can include:

* Single-line diagram
* Protection schematic
* CT/PT connections
* Relay wiring
* Circuit-breaker control circuit
* Feeder protection
* Electrical interconnections

---

# 📁 Repository Structure

```text
Substation-Protection-Fault-Analysis/
│
├── README.md
├── LICENSE
├── .gitignore
├── project_config.json
│
├── etap/
│   └── README.md
│
├── autocad/
│   └── README.md
│
├── calculations/
│   ├── transformer_calculations.md
│   ├── fault_calculations.md
│   └── protection_settings.md
│
├── documentation/
│   ├── single_line_diagram.md
│   ├── protection_scheme.md
│   └── methodology.md
│
├── results/
│   ├── README.md
│   ├── fault_analysis.csv
│   └── protection_coordination.md
│
└── screenshots/
    └── README.md
```

---

# 📚 Key Engineering Concepts

This project covers:

* Electrical Substations
* Power Systems
* Power System Analysis
* Short-Circuit Analysis
* Transformer Analysis
* Distribution Systems
* Electrical Protection
* Overcurrent Protection
* Earth-Fault Protection
* Relay Coordination
* Circuit Breakers
* CTs and PTs
* Fault Isolation
* Single-Line Diagrams

---

# 💡 Skills Demonstrated

### Electrical Engineering

* Power System Analysis
* Substation Design
* Short-Circuit Analysis
* Electrical Protection
* Transformer Analysis
* Relay Coordination
* Fault Analysis
* Circuit Breaker Protection

### Software

* ETAP
* AutoCAD Electrical

### Engineering Documentation

* Single-Line Diagrams
* Protection Schematics
* Technical Analysis
* Simulation Reporting

---

# 🚀 Future Improvements

* Add transformer differential protection.
* Implement busbar protection.
* Add detailed transformer fault analysis.
* Perform voltage-drop analysis.
* Add transformer inrush-current analysis.
* Compare different relay operating characteristics.
* Add automated protection coordination reports.
* Extend the model to an industrial distribution network.
* Include additional feeder protection schemes.

---

# 👨‍💻 Author

**Manish**

**B.Tech – Electrical Engineering**
Delhi Technological University (DTU)

### Areas of Interest

* Power Systems
* Electrical Protection
* Substations
* Renewable Energy
* Electrical System Simulation
* Power System Analysis

---

# ⚠️ Disclaimer

This project is an **academic simulation study** intended for educational and engineering-analysis purposes.

The substation configuration, protection settings, fault-current values, and simulation results should be verified against the actual ETAP model before being presented as final engineering results.

This project is **not intended to represent an industrial substation design or field-tested protection system**.


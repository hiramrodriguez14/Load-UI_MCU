# Horizontal Axis Wind Turbine Electronic Control Unit (ECU)

## Load Control & User Interface PCB

Printed Circuit Board (PCB) design for the **Load Control & User Interface (Load & UI) MCU** of the **Horizontal Axis Wind Turbine Electronic Control Unit (ECU)**.

This repository contains the complete KiCad hardware design, manufacturing files, and production documentation for the embedded controller responsible for battery charging, power management, user interaction, and system monitoring.

---

# Documentation & Demo

| Resource                 | Link                            |
| ------------------------ | ------------------------------- |
| 🎥 Project Demonstration | *(Add YouTube Link)*            |
| 📄 Final Project Report  | *(Add Final Report Link)*       |
| 📚 Technical Appendix    | *(Add Technical Appendix Link)* |

---

# Overview

The Load Control & User Interface PCB serves as the primary electrical control board of the Horizontal Axis Wind Turbine Electronic Control Unit (ECU).

Designed using **KiCad**, this board integrates sensing, power management, user interaction, communication, and data logging into a single embedded platform. It operates alongside the Turbine MCU PCB to provide complete supervision of the wind turbine system.

The PCB was designed with debugging, manufacturability, and future expansion in mind, incorporating dedicated test points, modular circuitry, and production-ready manufacturing files.

---

# Engineering Highlights

* Custom 2-layer PCB
* Designed in KiCad
* Texas Instruments MSPM0G3519
* Dual INA229 Power Monitors
* SEPIC Converter Control
* Battery Management System (BMS)
* LCD User Interface
* Push Button Interface
* Status LEDs
* UART Communication
* microSD Card Interface
* Relay Driver
* Barrel Jack Power Input
* Production-ready Gerber files
* Pick-and-Place (CPL) files
* Manufacturing BOM

---

# Hardware Features

The PCB integrates the following subsystems:

### Power Management

* Battery charging controller
* SEPIC converter interface
* Power monitoring
* Relay control
* Load protection

### User Interface

* 20×4 LCD connector
* Navigation buttons
* Record button
* Start / Stop controls
* Status LEDs

### Communication

* UART interface to Turbine MCU
* Programming interface
* Debug connectors

### Data Logging

* microSD card socket
* Real-Time Clock (RTC)

---

# Hardware Architecture

The Load Control & UI PCB serves as the electrical management hub of the complete ECU.

Primary functions include:

* Battery charging
* Converter control
* Power measurement
* User interaction
* Data logging
* Load protection
* Communication with the Turbine MCU

**Suggested image**

`images/system_overview.png`

*Figure 2 – Top-Level System View*

---

# PCB Design

The board was designed using KiCad following standard PCB design practices for embedded systems.

Design considerations include:

* Component placement optimization
* Short signal routing
* Power integrity
* Ground plane utilization
* Test point accessibility
* Manufacturing compatibility

**Suggested images**

`images/pcb_top.png`

Top Layer PCB

`images/pcb_bottom.png`

Bottom Layer PCB

---

# Manufacturing Files

This repository includes all files required for PCB fabrication and assembly.

Included manufacturing assets:

* Gerber files
* Drill files
* Pick-and-Place (CPL)
* BOM
* Schematic
* PCB Layout

---

# Development Tools

### PCB Design

* KiCad

### Target MCU

* Texas Instruments MSPM0G3519

---

# Repository Structure

```text
HAWT-LoadUI-PCB
│
├── gerbers/                    Manufacturing Gerber files
├── mylib/                       Custom KiCad component library
├── Load-UI_MCU.kicad_pcb        PCB layout
├── Load-UI_MCU.kicad_sch        Main schematic
├── Load-UI_MCU.kicad_pro        KiCad project
├── Load-UI_MCU-final.csv        Manufacturing BOM
├── Load-UI_MCU-all-pos.csv      Pick-and-Place (CPL)
├── load.kicad_sch               Power subsystem schematic
├── ui.kicad_sch                 User Interface schematic
├── README.md
└── LICENSE
```

---

# Related Repositories

| Repository               | Description                |
| ------------------------ | -------------------------- |
| HAWT-TurbineMCU-Firmware | Turbine control firmware   |
| HAWT-Load_Control_and_UI | Load Control & UI firmware |
| HAWT-TurbineMCU-PCB      | Turbine MCU PCB            |

---

# Authors

* Hiram R. Rodríguez Hernández
* José M. Burgos Guntín
* Sergio A. Meléndez Padilla
* Sergio A. Da Silva López

Department of Electrical & Computer Engineering

University of Puerto Rico – Mayagüez

---

# License

This project was developed for educational and research purposes as part of the Embedded Systems Design course at the University of Puerto Rico – Mayagüez.

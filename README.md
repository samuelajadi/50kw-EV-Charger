 # 50kW EV Charger Design — From Concept to Prototype

## Overview

This project documents the complete engineering process of designing a **50kW DC fast EV charger** from system requirements to prototype-ready architecture.

The goal is to develop and document the hardware, firmware, and software architecture behind a modern EV charging system, including the engineering decisions, calculations, simulations, and validation process.

This project covers:

- Power electronics architecture
- Active Front End (AFE) design
- Dual Active Bridge (DAB) isolated DC/DC converter
- High-frequency magnetics design
- Embedded control firmware
- Communication systems
- PCB design using KiCad
- Monitoring and software architecture

---

## Target Specification

**Power:** 50kW

**Input:** 3-phase 400VAC, 50Hz

**Output:** 200–1000VDC

**Maximum Output Current:** 250A

**Power Factor Target:** ≥0.99

**Input Current THD:** <5%

**Enclosure Target:** IP68

**Cooling:** Active thermal management

---

## System Architecture


3-Phase AC Grid
|
|
Active Front End (AFE)
|
|
DC Link
|
|
Dual Active Bridge (DAB)
|
|
EV Battery


---

## Major Design Blocks

### AC/DC Active Front End

The charger uses an actively controlled three-phase rectification stage designed for:

- High power factor
- Low harmonic distortion
- Stable DC-link regulation
- High efficiency operation

---

### Isolated DC/DC Stage

The DC/DC stage uses a **Dual Active Bridge (DAB)** converter.

Focus areas:

- High-frequency transformer design
- Phase-shift power control
- Wide voltage regulation
- Soft-switching operation
- Thermal optimisation

---

### Embedded Control

The control system will include:

- Real-time PWM control
- Voltage and current regulation
- Protection management
- Fault detection
- Communication handling

Communication architecture:

- CAN/CAN FD for internal communication
- EV charging communication interface
- UART/USART for auxiliary communication and debugging

---

## PCB Design

PCB development will be done using **KiCad**.

Design considerations:

- High-current routing
- Creepage and clearance
- Gate-drive layout
- EMI reduction
- Thermal management
- Power loop optimisation

---

## Development Roadmap

1. System specification and architecture  
2. Power stage design  
3. Magnetics design  
4. Control firmware development  
5. PCB design  
6. Prototype development  
7. Testing and validation  

---

## Project Philosophy

A high-power converter is not designed by selecting components randomly.

Every decision affects:

- Efficiency
- Reliability
- Cost
- Thermal performance
- EMI
- Manufacturability

This project documents the engineering process:

**Requirements → Architecture → Design → Prototype → Testing → Validation**

The complete design journey will be shared publicly.

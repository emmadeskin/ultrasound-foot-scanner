# Automated Weight-Bearing 3D Ultrasound Foot Scanner

**University of Arizona — ENGR 498 Interdisciplinary Capstone | 2025–2026**  
**Sponsors:** Dr. Daniel Latt & Dr. Russell Witte, Department of Biomedical Engineering  
**Team:** Shea, Ariana, Emma, Justin, Ruth, Tanisha

---

## Overview

A clinical-grade automated medical imaging device designed to diagnose **Progressive Collapsing Foot Deformity (PCFD)** — a condition affecting five million people in the US annually — by scanning foot soft tissue stiffness under weight-bearing conditions. The system combines **B-mode ultrasound** and **Shear Wave Elastography (SWE)** to produce anatomical images and quantitative stiffness maps of arch-supporting structures while the patient stands, capturing tissue behavior that non-weight-bearing imaging cannot replicate.

This year's scope built on a prior mechanical foundation to deliver full system integration: automated 3-axis motion, synchronized ultrasound acquisition, a MATLAB GUI, and a complete V&V campaign.

---

## System Architecture

The device is composed of four integrated subsystems:

- **Mechanical assembly** — weight-bearing platform, X/Y linear actuators, rotation motor, probe mount, 3D-printed heel cup, gel pad holder, and slide track
- **Electrical subsystem** — Teensy 4.1 microcontroller, DM320T and TB6600 stepper drivers, X/Y limit switches, 24V AC/DC adapter, emergency stop, and power shutoff
- **Software subsystem** — MATLAB AppDesigner GUI, motor movement control scripts, B-mode acquisition, SWE acquisition, and volumetric image output
- **Ultrasound subsystem** — Verasonics Vantage 256 system, GE 9L-D linear array transducer, Aquaflex coupling gel pad

---

## Key Results

- **±0.04 mm** linear positioning accuracy over 50 mm travel (5× better than the ±0.2 mm requirement)
- **±1°** rotational accuracy over a full 360° rotation (3× better than the ±3° requirement)
- **3-minute** patient setup time (requirement: <10 minutes)
- **≤120 kg** weight-bearing operation verified
- **Emergency stop** halts all motion in ≤1 second
- **10 of 16** system requirements verified and passed
- **$641.85 spent** of a $4,500 budget — full system delivered with $3,858.15 remaining
- Real-time B-mode image display during scanning confirmed
- Verasonics–Teensy serial communication and synchronized motion triggering verified
- Heel cup accommodates foot sizes up to men's 14 and widths up to 10 cm

---

## My Contributions

- **MATLAB scripts** for B-mode and SWE data acquisition via the Verasonics Vantage platform
- **Mechanical design** — heel cup and probe mount components modeled in SolidWorks and fabricated via 3D printing
- **Microcontroller programming** — Teensy 4.1 firmware for 3-axis stepper motor control via serial communication
- **Electrical integration** — wiring diagrams for stepper drivers (DM320T, TB6600), limit switches, and emergency stop circuit
- **V&V and documentation** — executed formal verification and validation testing protocol; authored the System Requirements Document (SRD), System Design Document (SDD), and user manual

---

## Tools & Technologies

`MATLAB` `Verasonics Vantage` `Teensy 4.1` `SolidWorks` `Arduino IDE` `3D printing`

---

## Documentation

The full technical data package includes:

- System Requirements Document (SRD)
- System Design Document (SDD)
- System Verification Plan and Results (8 test procedures)
- Hardware drawing package (piece-part drawings, electrical schematics, ultrasound layout)
- Software documentation and GUI design
- User manual

---

## Background

PCFD affects the posterior tibial tendon and plantar fascia, causing arch collapse, hindfoot valgus, and forefoot abduction. Current diagnostic tools (X-ray, CT, standard ultrasound) are typically performed non-weight-bearing and lack the ability to measure soft tissue stiffness quantitatively. Shear Wave Elastography detects subtle changes in tissue stiffness and, integrated with automated scanning, offers a path toward earlier, more consistent diagnosis and better treatment planning.

No existing clinical system combines weight-bearing imaging with automated, repeatable multi-axis scanning — this project addresses that gap.

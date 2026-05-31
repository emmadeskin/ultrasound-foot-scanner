# ultrasound-foot-scanner
Automated weight-bearing 3D ultrasound foot scanner for PCFD diagnosis — University of Arizona Senior Capstone 2025-2026
# Automated Weight-Bearing 3D Ultrasound Foot Scanner

**University of Arizona Senior Capstone | 2025–2026**
**Sponsors:** Department of Biomedical Engineering — Dr. Daniel Latt & Dr. Russell Witte

## Overview
A clinical-grade automated medical imaging device designed to diagnose 
Progressive Collapsing Foot Deformity (PCFD) by scanning foot soft tissue 
stiffness under weight-bearing conditions using B-mode ultrasound and 
Shear Wave Elastography (SWE).

## My Contributions
- Developed MATLAB scripts for B-mode and SWE data acquisition via Verasonics Vantage
- Designed heel cup and mechanical components in SolidWorks; fabricated via 3D printing
- Programmed Teensy 4.1 microcontroller for 3-axis motor control via serial communication
- Developed wiring diagrams integrating stepper drivers, limit switches, and emergency stop
- Executed formal V&V testing protocol; authored SRD, SDD, and user manual

## System Architecture
- **Mechanical:** X/Y linear actuators, rotation motor, probe mount, heel cup, gel pad holder
- **Electrical:** Teensy 4.1, DM320T & TB6600 stepper drivers, limit switches, 24V power, emergency stop
- **Software:** MATLAB AppDesigner GUI, motor control scripts, B-mode acquisition, SWE acquisition
- **Ultrasound:** Verasonics Vantage 256, GE 9L-D transducer, Aquaflex gel pad

## Key Results
- Linear positioning accuracy: ±0.04 mm (requirement: ±0.2 mm)
- Rotational accuracy: ±1° (requirement: ±3°)
- Setup time: 3 minutes (requirement: <10 minutes)
- Delivered under $4,500 budget

## Tools & Technologies
MATLAB · Verasonics Vantage · Teensy 4.1 · SolidWorks · Arduino IDE · 3D printing

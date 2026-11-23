# Haptic Exoskeleton — Electrical Power-System Research

**Status:** In progress (November 2026) · **Organization:** UBC Open Robotics  
**Role:** Electrical team member · **Focus:** power electronics, motor control, battery systems and protection

> This repository documents **my individual research and general engineering contributions** toward a wearable haptic exoskeleton. It is not the team's official design repository.

## Overview

As part of UBC Open Robotics, I am working on the electrical requirements for a haptic exoskeleton intended to provide force feedback during robotic teleoperation. My current focus includes battery chemistry and operating voltage, power converters for low-voltage electronics, BLDC motor drive requirements, and basic electrical safety/protection concepts.

We are currently designing the schematic for the PCB.

## Electrical topics investigated

### Battery and supply architecture
- Compared lithium-ion and LiFePO4 battery types, including pack voltage, capacity, energy density, protection and practical packaging.
- Investigated 4-series lithium-ion packs: approximately **14.8 V nominal and 16.8 V fully charged** for 3.7 V nominal cells.
- Researched cell balancing, voltage/current protection, battery monitoring and thermal sensing.
- Investigated switching voltage regulators for proposed **5 V and 3.3 V** electronics rails.

### Motor drive
- Studied 3-phase BLDC commutation and field-oriented control (FOC).
- Investigated the operation of **three half-bridges / six MOSFETs**, high/low-side gate drivers, dead time and shoot-through.
- Evaluated motor driver selection criteria: voltage and current ranges, current sensing, encoder feedback, PWM interfaces and built-in protections.
- Compared integrated drive solutions and external MOSFET/gate-driver architectures.

### Circuit safety and power integrity
- Researched PMOS-based reverse-polarity protection, series fusing and TVS transient suppression.
- Investigated placement of DC-bus bulk capacitance versus local decoupling capacitors.
- Distinguished disabling drive torque from physically isolating electrical power during an emergency stop.
- Studied regenerative energy and potential DC-bus voltage rise, including the limitations of bulk capacitors and TVS diodes for sustained regeneration.

## Research summary

| Workstream | Current status |
| --- | --- |
| Battery chemistry and 4S voltage research | Initial comparison performed |
| BLDC motor / driver requirements | Initial comparison performed |
| DC-DC regulation alternatives | Initial evaluation performed |
| Input protection and emergency-stop concepts | Under investigation |
| Detailed schematic and PCB | In progress |
| Hardware fabrication and testing | No measurements documented |

## Engineering documentation

- [Public-safe architecture notes](docs/architecture.md)
- [Tradeoffs and design decisions](docs/design-decisions.md)
- [Proposed validation checklist](docs/testing.md)
- [Progress log](docs/progress-log.md)
- [Hardware publishing policy](hardware/README.md)


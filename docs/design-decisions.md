# Engineering research and design tradeoffs

## Battery chemistry
Compared 4S conventional Li-ion (about 14.8 V nominal / 16.8 V full with 3.7 V cells) with 4S lithium iron phosphate (about 12.8 V nominal / 14.6 V full). Relevant considerations include energy density, mass, capacity, charging, voltage limits, cycle life and protection.

## Regulation
Compared LDO regulation against switching buck conversion for significant voltage drops. Discussed converter capabilities using candidate families including TPS62110, MP1584, LMR51420 and TPS62933. Input-voltage margin must account for the fully charged battery and expected transients.

## Motor controllers
Researched three-phase inverter topology, integrated drivers versus external MOSFET stages, encoder/current feedback, PWM control and field-oriented control. Considered protection against shoot-through, overcurrent and undervoltage.

## Protection concepts
Investigated fuses, reverse-polarity MOSFETs, TVS transient suppression and bus bulk capacitance. Considered the difference between stopping motor torque and disconnecting power. Investigated how regeneration may raise bus voltage, requiring more than temporary energy storage.

## Status
These comparisons document research and not finalized or validated hardware selections. Specific team design documents are not published here.

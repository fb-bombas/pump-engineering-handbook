---
title: Thermal-oil pumps — design considerations
description: Closed-loop circulation of heat-transfer fluids at 250-350 °C
---

# Thermal-oil circulation pumps

A thermal-oil heating system circulates a synthetic or mineral heat-transfer
fluid through a fired heater and back to process consumers (jacketed reactors,
heat exchangers, calanders). The pump runs **continuously** at fluid
temperatures typically between 200 and 350 °C.

Three constraints dominate pump selection:

1. **Mechanical seal life** at temperature. Standard elastomers fail above
   180 °C. Thermal-oil pumps use hard-face mechanical seals (typically
   silicon carbide vs silicon carbide) with cooled seal flush.
2. **Bearing temperature**. The bearing housing must be thermally isolated
   from the fluid casing — usually a finned spool piece between casing and
   bearing housing dissipates heat.
3. **Flow stability**. Thermal-oil systems are sensitive to flow drop —
   reduced flow at high temperature accelerates fluid breakdown (cracking,
   coke formation).

## Operating envelope of the FB Bombas FBOT line

The [FBOT thermal-oil line](https://www.fbbombas.com.br/produtos/serie-fbot)
covers, per the official catalog:

- Sizes: DN25 to DN300
- Flow: up to 2.200 m³/h
- Head: up to 135 m
- Temperature: continuous duty up to 350 °C
- Maximum rotation: 3.500 rpm
- Maximum suction pressure: 10 bar

Construction and shaft-sealing options are configured per application.
For the recommended materials and seal arrangement at any specific
service, consult the FBOT technical manual (linked from the catalog
page) or [FB Bombas application engineering](https://www.fbbombas.com.br/contato).

## Common failure mode: fluid degradation

Thermal-oil itself is a consumable. Over time it cracks (long molecules break
into smaller volatile fragments) and oxidizes (if air ingresses through a bad
seal or expansion-tank vent). Symptoms:

- Rising viscosity → flow drop → temperature spike
- Acid number > 0.5 mg KOH/g → corrosion accelerates
- Carbon deposits in heater coils → hotspots → coil failure

Best practice: sample the fluid every 6-12 months. Replace before the acid
number or carbon residue exceeds the supplier's limits.

## What kills thermal-oil pumps

| Cause | Mitigation |
|-------|-----------|
| Dry start | Interlock with expansion-tank low-level switch |
| Air ingress through seal | Maintain expansion tank N₂ blanket |
| Overheating bearings | Verify cooling water flow on the seal flush plan |
| Coked impeller | Replace fluid before coke residue spec is exceeded |

## Further reading

- [FBOT product page](https://www.fbbombas.com.br/produtos/serie-fbot)
- [Manuais técnicos — thermal oil](https://www.fbbombas.com.br/manuais-tecnicos)

## References

- API 685-2011 — Sealless Centrifugal Pumps for Petroleum, Petrochemical, and Gas Industry Process Service.
- Therminol & Dowtherm technical bulletins (fluid suppliers' degradation limits).
- ASTM D2882 — Standard Test Method for Indicating the Wear Characteristics of Petroleum and Non-Petroleum Hydraulic Fluids in Constant Volume Vane Pump (proxy for fluid wear).

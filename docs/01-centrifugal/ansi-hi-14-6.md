---
title: Hydraulic performance testing — ANSI/HI 14.6
description: How rotodynamic pumps are tested for acceptance and what the tolerance grades mean
---

# ANSI/HI 14.6 — hydraulic performance testing

ANSI/HI 14.6 (current edition: 2022) is the rotodynamic pump acceptance test
standard. When a buyer specifies "tested per HI 14.6 Grade 1B" in a purchase
order, this is what they are referring to.

## What gets tested

The test bench measures, at a defined speed and fluid temperature:

1. **Q** — flow rate, via calibrated flow meter
2. **H** — total head, via pressure transducers at suction and discharge flanges
3. **P** — input power, via torque cell or calibrated motor
4. **η** — efficiency, derived as `(ρ·g·Q·H) / P`
5. **NPSHr** — measured by progressively dropping suction pressure until head
   drops 3% (the "3% drop" criterion)

Several points are taken across the curve: typically 0%, 50%, 75%, 100%, 110%,
and 120% of rated flow.

## Acceptance grades

The standard defines tolerance bands the as-tested results must fall within:

| Grade | Application | Q tolerance | H tolerance | η tolerance |
|-------|-------------|-------------|-------------|-------------|
| **1U** | Critical / API 610 | ±5% | ±3% | -3% |
| **1B** | Industrial standard | ±8% | ±5% | -5% |
| **2B** | Commercial / utility | ±10% | ±8% | -8% |
| **3B** | Light duty | ±10% | ±8% | none |

Grade 1B is the typical acceptance target for industrial process duty.

Grade 1U is mandatory for **API 610** (refining and petrochemical) — see API
610 §8.3 for the additional vibration and bearing temperature limits that
stack on top of HI 14.6.

## What the buyer receives

A factory acceptance test (FAT) per HI 14.6 produces:

- A **test certificate** with serial number, test date, and operator signature
- **Numerical data** at each test point (Q, H, P, η, NPSHr)
- A **performance curve** plotted from the data
- Witness sign-off if the buyer attended (witnessed FAT)

Shipping a pump without an HI 14.6 certificate to a process plant is unusual —
ask for it explicitly when negotiating.

## What FB Bombas tests

Our hydraulic test bench in Cabreúva runs ANSI/HI 14.6 acceptance tests up to
the size envelope of our catalog. See [Por que FB Bombas](https://www.fbbombas.com.br/por-que-fb-bombas)
for the test capability matrix.

## Further reading

- [Centrifugal selection logic](./selection-guide.md)
- [Normalized pumps — ISO 2858 / ASME B73.1](./normalized-pumps.md)

## References

- ANSI/HI 14.6-2022 — Rotodynamic Pumps for Hydraulic Performance Acceptance Tests.
- API 610-2021 §8.3 — Performance, mechanical, and NPSH tests.
- ISO 9906:2012 — Rotodynamic pumps — Hydraulic performance acceptance tests — Grades 1, 2 and 3 (the international equivalent).

---
title: Centrifugal pump selection logic
description: How to read a pump curve, find the operating point, and avoid costly sizing mistakes
---

# Centrifugal pump selection — operating point logic

A centrifugal pump does not have a single "flow rate". It produces a curve of
head (`H`) versus flow (`Q`), and the **operating point** is where that curve
intersects the **system curve** of the piping it pushes fluid through.

```
Head (m)
  │  ╲
  │   ╲    pump curve
  │    ╲╭──╮
  │     ●  ← operating point
  │    ╱
  │   ╱     system curve
  │  ╱
  └────────────────── Flow (m³/h)
```

Get the intersection wrong and you operate the pump off its **Best Efficiency
Point (BEP)** — wasting energy, accelerating wear, and risking cavitation or
recirculation damage.

## The four numbers you must know

| Symbol | Meaning | Source |
|--------|---------|--------|
| `Q` | Required flow rate (m³/h) | Process duty |
| `H` | Required total head (m) | Static lift + friction losses |
| `NPSHa` | Net Positive Suction Head **available** (m) | System geometry + fluid vapor pressure |
| `NPSHr` | NPSH **required** by the pump (m) | Pump curve, given by manufacturer |

**Hard rule:** `NPSHa - NPSHr ≥ 1 m` (some standards say 0.6 m; we
recommend 1 m for industrial duty as a safety margin). Below this margin,
cavitation begins — bubble collapse in the impeller damages metal and erodes
performance permanently.

## Don't size to the rated point

A common mistake: select a pump where the duty point sits exactly on the
rated curve. Real systems drift:

- Strainers clog → friction rises → operating point shifts left
- Pipe scaling → friction rises slowly over years
- Process upsets → demand spikes 10-20% above nominal

The safe envelope is **70-110% of BEP flow**. Outside that band:

- **<70% BEP:** recirculation, radial loads on bearings, premature seal wear
- **>110% BEP:** cavitation onset, rapid efficiency drop, motor overload

## Worked example

> Pump 80 m³/h water at 30 °C, 32 m head, NPSHa = 6 m at the suction flange.

Looking at the [FBCN family](https://www.fbbombas.com.br/produtos/serie-fbcn)
matrix, model FBCN 80-200 hits this point near 1.450 rpm with BEP at 75 m³/h
and NPSHr ≈ 3.5 m. Margin = 6 - 3.5 = 2.5 m. Safe.

Same duty with NPSHa = 4 m (suction tank lower) — margin shrinks to 0.5 m.
Either raise the suction tank, switch to a lower-NPSHr model class, or accept
inducer-equipped variants.

## Further reading

- [Normalized centrifugal pumps — ISO 2858 / ASME B73.1](./normalized-pumps.md)
- [ANSI/HI 14.6 hydraulic performance testing](./ansi-hi-14-6.md)
- [FB Bombas centrifugal applications](https://www.fbbombas.com.br/aplicacoes/agua)

## References

- Karassik, I. J., et al. *Pump Handbook*, 4th ed. McGraw-Hill, 2008.
- API 610-2021 — Centrifugal pumps for petroleum, petrochemical and natural gas industries.
- Hydraulic Institute (HI) — ANSI/HI 9.6.3 *Rotodynamic Pumps — Guideline for Allowable Operating Region*.

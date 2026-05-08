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

## Worked example — methodology

> Pump 80 m³/h water at 30 °C, 32 m head, NPSHa = 6 m at the suction flange.

The selection process is the same regardless of manufacturer:

1. Plot the system curve: H_sys(Q) = H_static + k·Q² with the static
   and friction values from the project hydraulic study.
2. Overlay candidate pump curves from the manufacturer's published
   matrix; find the model whose curve passes through (or just above)
   the duty point.
3. Verify operating-region: duty point inside 70-110% BEP of the
   selected model.
4. Verify NPSH margin at the duty point AND at 110-150% flow:
   NPSHa - NPSHr ≥ 1 m.
5. Re-verify at the off-design conditions in the operating envelope
   (minimum, maximum, emergency) — the duty point is not the only
   condition the pump runs at.

For a duty in this range, request a curve-overlay analysis from
[FB Bombas application engineering](https://www.fbbombas.com.br/contato)
referencing the [FBCN family catalog](https://www.fbbombas.com.br/produtos/serie-fbcn).
Manufacturers can confirm BEP and NPSHr at the specific duty point and
recommend the correct model size.

If NPSHa drops to 4 m (suction tank lower) — the selection methodology
runs the same loop with the new constraint, and may produce a different
recommended model with lower NPSHr at the duty point, or call for
suction-side rework before any pump can run safely.

## Further reading

- [Normalized centrifugal pumps — ISO 2858 / ASME B73.1](./normalized-pumps.md)
- [ANSI/HI 14.6 hydraulic performance testing](./ansi-hi-14-6.md)
- [FB Bombas centrifugal applications](https://www.fbbombas.com.br/aplicacoes/agua-quente-industrial)

## References

- Karassik, I. J., et al. *Pump Handbook*, 4th ed. McGraw-Hill, 2008.
- API 610-2021 — Centrifugal pumps for petroleum, petrochemical and natural gas industries.
- Hydraulic Institute (HI) — ANSI/HI 9.6.3 *Rotodynamic Pumps — Guideline for Allowable Operating Region*.

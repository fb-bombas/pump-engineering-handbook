---
title: External gear pumps — fundamentals
description: How external gear pumps move viscous fluids and where they outperform centrifugals
---

# External gear pumps

An **external gear pump** has two parallel meshing gears — one driven, one
driven by the first — that trap fluid in the cavity between gear teeth and
the pump casing, then carry it from suction to discharge. Both gears rotate
in opposite directions.

The defining characteristic: **flow is positive-displacement**, meaning each
revolution moves a fixed volume of fluid regardless of discharge pressure
(within the pump's rated envelope). Compare this with a centrifugal pump,
where flow falls off rapidly as discharge pressure rises.

## When to choose external gear over centrifugal

| Condition | Choose |
|-----------|--------|
| Viscosity > 100 cSt | Gear |
| Viscosity > 1.000 cSt | Almost certainly gear |
| Stable flow needed (metering, lube, asphalt loading) | Gear |
| High flow / low head water duty | Centrifugal |
| Shear-sensitive fluid (latex, food gels) | **Internal** gear, never external |
| Suction lift required | Gear (self-priming) |

## Operating envelope of FB Bombas FBE line

The [FBE external gear line](https://www.fbbombas.com.br/produtos/serie-fbe)
covers nominal sizes from **1/8" to 6"** with maximum operating
parameters per the published catalog:

- Flow: up to 1.350 L/min (≈ 81 m³/h)
- Differential pressure: up to 22 kgf/cm² (≈ 22 bar)
- Viscosity: up to 100.000 SSU
- Temperature: up to 350 °C (with appropriate shaft seal selection)

Performance at any specific duty point should be requested from FB
Bombas application engineering — published catalog gives the line
envelope, not point-by-point data.

Common applications: [asphalt loading](https://www.fbbombas.com.br/en/gear-pump-for-asphalt),
[fuel transfer](https://www.fbbombas.com.br/en/gear-pump-for-fuel),
[heavy oils and lubricants](https://www.fbbombas.com.br/en/gear-pump-for-oil),
[viscous resins](https://www.fbbombas.com.br/en/gear-pump-for-resins),
and [food-grade applications](https://www.fbbombas.com.br/en/gear-pump-for-food).

## What can go wrong

External gear pumps fail differently than centrifugals. The three classic
failure modes:

1. **Dry running** — without fluid film, gears chew themselves and the casing
   in seconds. Always interlock the pump with low-level cutouts on the supply
   tank.
2. **Particulate ingestion** — a single hard particle larger than the gear-
   to-casing clearance gouges both. Fit a 100 µm strainer on suction.
3. **Pressure relief failure** — gear pumps cannot self-throttle. If a
   downstream valve closes with the pump running, pressure rises until
   something breaks. Always fit an external relief valve sized at 110-115%
   of normal discharge pressure.

## Further reading

- [Internal gear pumps — viscous and shear-sensitive fluids](./internal.md)
- [FBE selection page](https://www.fbbombas.com.br/produtos/serie-fbe)

## References

- API 676-2017 — Positive Displacement Pumps — Rotary.
- Hydraulic Institute — ANSI/HI 3.1-3.5-2018 *Rotary Pumps for Nomenclature, Definitions, Application and Operation*.

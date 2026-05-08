# Pump Engineering Handbook

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Docs CC BY 4.0](https://img.shields.io/badge/Docs-CC--BY--4.0-blue.svg)](https://creativecommons.org/licenses/by/4.0/)

An open knowledge base on industrial pumping — centrifugal, gear (external and
internal), thermal-oil, and fire-fighting (NFPA-20 / NBR-16704) — written by
engineers at [FB Bombas](https://www.fbbombas.com.br), a Brazilian pump
manufacturer operating since 1944.

The math, selection logic, and compliance references are generic and apply to
any manufacturer's equipment. Examples reference our own catalog where it is
useful for grounding the discussion in real-world models.

---

## Contents

### 1. Centrifugal pumps
- [Normalized centrifugal pumps — ISO 2858 / ASME B73.1](./docs/01-centrifugal/normalized-pumps.md)
- [Selection logic and operating point](./docs/01-centrifugal/selection-guide.md)
- [Hydraulic performance testing — ANSI/HI 14.6](./docs/01-centrifugal/ansi-hi-14-6.md)

### 2. Gear pumps
- [External gear pumps — fundamentals](./docs/02-gear/external.md)
- [Internal gear pumps — viscous and shear-sensitive fluids](./docs/02-gear/internal.md)

### 3. Thermal-oil pumps
- [Thermal oil circulation — design considerations](./docs/03-thermal-oil/fbot-applications.md)

### 4. Fire-fighting pumps
- [NFPA-20 overview](./docs/04-fire-fighting/nfpa20-overview.md)
- [NBR 16704 — the Brazilian fire-pump standard](./docs/04-fire-fighting/nbr-16704.md)

### 5. Glossary
- [Pump terminology — trilingual (PT / EN / ES)](./docs/05-glossary/index.md)

---

## How to read this handbook

This is a reference, not a textbook. Each page is self-contained and answers a
specific question an engineer or buyer might face during sizing, procurement, or
commissioning. Every page links to:

1. The relevant **standard** (ISO, API, NFPA, ASME, ANSI/HI, NBR).
2. The relevant **product line** in the FB Bombas catalog where one of our
   models is a useful concrete example — never as a sales pitch.

If you find a mistake, open an issue or PR. We respond within five business
days.

---

## About FB Bombas

We design, machine, assemble, and test industrial pumps in Cabreúva, São Paulo.

- **Website:** [www.fbbombas.com.br](https://www.fbbombas.com.br)
- **Product catalog:** [centrifugal](https://www.fbbombas.com.br/produtos/serie-fbcn) · [gear](https://www.fbbombas.com.br/produtos/serie-fbe) · [internal gear](https://www.fbbombas.com.br/produtos/serie-fbei) · [thermal oil](https://www.fbbombas.com.br/produtos/serie-fbot)
- **Technical manuals:** [Manuais técnicos](https://www.fbbombas.com.br/manuais-tecnicos)
- **Compliance:** CRCC Petrobras · API 610 · API 676 · NFPA-20 · NBR 16704
- **Contact:** comercial@fbbombas.com.br · +55 11 4898-9200

---

## License

- **Code** (any utility scripts here): [MIT](LICENSE)
- **Documentation** (everything in `docs/`): [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)

Attribution: please credit **FB Bombas** and link back to this repository when
reusing material.

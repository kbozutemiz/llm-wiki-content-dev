---
title: "HCl Vapor Soldering"
type: method
tags: [egain, liquid-metal, fabrication, soldering, microelectronics-integration, soft-electronics]
related: [egain-liquid-metal-alloys, gallium-oxide, biphasic-stretchable-electronics, naoh-oxide-removal, selective-wetting]
created: 2026-06-28
updated: 2026-06-28
---

# HCl Vapor Soldering

## Definition
A novel method for creating reliable electromechanical connections between liquid metal (EGaIn) interconnects and the metal pins of surface-mount microelectronic components, introduced by Ozutemiz et al. (2018). Hydrochloric acid (HCl) vapor is directed at the LM–component pin interface, where it simultaneously removes the gallium oxide (Ga₂O₃) skin from EGaIn and the native oxide from the component pin surface. The exposed bulk EGaIn, now high-surface-tension and chemically active, wets the pin metal and forms a mechanically and electrically robust "soldered" joint.

The function is directly analogous to solder flux in conventional PCB manufacturing: flux removes oxides to expose clean metal surfaces for solder wetting. HCl vapor plays the same role for LM "soldering."

## Key Thinkers
- [Kadri Bugra Ozutemiz](../authors/bugra-ozutemiz.md) — first author; developed and characterized the technique.
- [Carmel Majidi](../authors/carmel-majidi.md) — senior author; directed the research.
- K. Doudrick et al. (Langmuir 2014) — prior work characterizing HCl vapor–Ga₂O₃ interaction that this method builds on.

## Related Concepts
- [Gallium Oxide (Ga₂O₃)](../concepts/gallium-oxide.md) — the oxide that HCl vapor removes; its removal is the essential mechanism.
- [EGaIn / Liquid Metal Alloys](../concepts/egain-liquid-metal-alloys.md) — the LM whose surface is activated by HCl treatment.
- [Selective Wetting](../concepts/selective-wetting.md) — HCl activates selective wetting at the pin interface.
- [Intermetallic Compound Formation](../concepts/intermetallic-compound-formation.md) — Cu wetting layer must be present; CuGa₂ prevents LM dewetting during HCl application.
- [Biphasic Stretchable Electronics](../concepts/biphasic-stretchable-electronics.md) — HCl soldering is the final integration step in biphasic circuit assembly.
- [NaOH Treatment for Oxide Removal](../methods/naoh-oxide-removal.md) — complementary oxide removal method used earlier in the process (for LM deposition, not pin soldering).

## Process Details
- **HCl source**: 36% w/w aqueous HCl solution in a bottle; vapor is drawn off and applied via dropper or syringe pump.
- **Controlled delivery**: 20 mL vapor at 42 mL min⁻¹ flow rate, applied by syringe needle at ~2.5 mm standoff distance.
- **Environment**: Performed under fume hood (100 ft min⁻¹ flow rate).
- **Post-treatment**: Rinse with DI water and IPA; dry at 60 °C.
- **Prerequisite**: A metal wetting layer (Cu) must be present on the substrate — without it, HCl causes LM to dewet and distort the circuit.

## Measured Effects (Ozutemiz et al. 2018)
| Metric | Without HCl | With HCl |
|---|---|---|
| Immediate yield | ~55% (9/20 fail) | 100% |
| Resistance (day 1) | 60.6 ± 4.9 mΩ (unstable) | 48.2 ± 2.0 mΩ (stable) |
| Strain at failure | 57.7 ± 7.9% | 82.6 ± 13.3% |
| 2000-cycle survival | ~25% (1/4) | 100% (3/3) |
| Component self-alignment | No | Yes (via surface tension) |
| Interface geometry | Abrupt, pin-bottom contact | Smooth encapsulation of pin |

## Limitations
- Requires components tolerant of brief corrosive HCl vapor exposure.
- Incompatible with Al-contacted ICs (Ga corrosion of Al is severe).
- Currently manual or semi-manual; integration into automated assembly requires engineering.
- Fume hood required; not suitable for uncontrolled environments.

## Source Support
- [Ozutemiz et al. 2018 — EGaIn–Metal Interfacing](../source-notes/ozutemiz-2018-egain-metal-interfacing.md)

## Open Questions
- Can HCl vapor be replaced with less corrosive alternatives (e.g., organic acid vapors, plasma treatment) that achieve equivalent oxide removal?
- What is the minimum HCl vapor dose required for complete oxide removal across different component package sizes and pin materials?
- Can this process be automated and integrated into a standard pick-and-place + reflow workflow?

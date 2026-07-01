---
title: "Selective Wetting"
type: concept
tags: [egain, liquid-metal, wetting, fabrication, surface-chemistry, biphasic-electronics]
related: [egain-liquid-metal-alloys, gallium-oxide, biphasic-stretchable-electronics, naoh-oxide-removal, intermetallic-compound-formation]
created: 2026-06-28
updated: 2026-06-29
---

# Selective Wetting

## Definition
The property of gallium-based liquid metals (EGaIn, Galinstan) to preferentially wet metal surfaces (Cu, Au, Sn) while not adhering to elastomeric or polymer surfaces (e.g., [PDMS](../concepts/pdms.md)). This selectivity is the enabling mechanism for patterning LM circuits without conventional lithographic masking of the liquid itself: EGaIn is deposited over an entire substrate but adheres only where metal wetting layers have been defined.

Selective wetting is oxide-dependent:
- **With Ga₂O₃ skin (in air)**: EGaIn wets many surfaces non-selectively. Useful for stencil-based deposition but not for self-aligned selective patterning.
- **Without Ga₂O₃ (oxide removed by NaOH or HCl)**: Bulk EGaIn (high surface tension, ≈435 mN m⁻¹) wets only metals where strong chemical affinity and alloying reactions occur. Elastomers are non-wetted and LM beads off.

## Key Thinkers
- [Carmel Majidi](../authors/carmel-majidi.md) — central figure in developing biphasic architectures that exploit selective wetting.
- Michael Dickey — foundational characterization of EGaIn wetting behavior.

## Related Concepts
- [EGaIn / Liquid Metal Alloys](../concepts/egain-liquid-metal-alloys.md) — selective wetting is a fundamental property of EGaIn's surface chemistry.
- [Gallium Oxide (Ga₂O₃)](../concepts/gallium-oxide.md) — oxide state governs whether wetting is selective or non-selective.
- [Biphasic Stretchable Electronics](../concepts/biphasic-stretchable-electronics.md) — the fabrication architecture built around selective wetting.
- [NaOH Treatment for Oxide Removal](../methods/naoh-oxide-removal.md) — the process step that activates selective wetting.
- [Intermetallic Compound Formation](../concepts/intermetallic-compound-formation.md) — alloying reactions (e.g., CuGa₂) at the wetting layer interface drive and anchor LM deposition.

## Wetting Hierarchy
| Surface | Wetting (oxide removed) | Notes |
|---|---|---|
| Cu | Yes | Forms CuGa₂ intermetallic; strong adhesion |
| Au | Yes | Alloys with Ga; used as alternative wetting layer |
| Sn (IC pin coating) | Reactive/slow | Governed by reactive wetting kinetics |
| PDMS | No | High contact angle; LM beads off |
| SU-8, photoresist | No | Used as patterning masks |

## Role in Fabrication
1. A metal wetting layer (typically Cu or Au) is deposited and patterned on an elastomer substrate to define the desired circuit geometry.
2. EGaIn is introduced (by immersion, dropper, or printing) to the substrate after oxide removal.
3. EGaIn selectively deposits only on the metal wetting layer, self-patterning the LM circuit.
4. The result is an LM circuit that follows the wetting layer geometry exactly, down to ~40 μm linewidths.

## Source Support
- [Ozutemiz et al. 2018 — EGaIn–Metal Interfacing](../source-notes/ozutemiz-2018-egain-metal-interfacing.md)

## Open Questions
- What is the smallest achievable linewidth before LM bridging (excess LM spanning adjacent traces) becomes uncontrollable?
- Can selective wetting be exploited for 3D or multilayer LM circuit architectures?
- How does the wetting layer thickness affect LM adhesion and long-term intermetallic growth?

## Tags
`egain` `liquid-metal` `wetting` `fabrication` `surface-chemistry` `biphasic-electronics`

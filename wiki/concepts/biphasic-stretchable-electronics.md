---
title: "Biphasic Stretchable Electronics"
type: concept
tags: [egain, liquid-metal, fabrication, stretchable-electronics, biphasic, soft-electronics]
related: [egain-liquid-metal-alloys, selective-wetting, stretchable-electronics, hcl-vapor-soldering, sputter-deposition-elastomers]
created: 2026-06-28
updated: 2026-06-28
---

# Biphasic Stretchable Electronics

## Definition
A fabrication architecture for stretchable electronics in which a patterned solid metal thin-film (the "wetting layer") on an elastomer substrate serves as the template onto which liquid metal (EGaIn or Galinstan) is selectively deposited. The circuit is thus "biphasic": it consists of two conductor phases — the solid metal pattern defining the circuit geometry, and the liquid metal that coats it and provides the actual electrical path.

The key insight: the solid wetting layer (typically Cu or Au, ~100 nm thick) does the patterning work (leveraging well-established lithographic or laser-based techniques), while the LM provides stretchability. Neither phase alone achieves the combination of patterning precision and mechanical deformability that biphasic architecture enables.

## Key Thinkers
- [Carmel Majidi](../authors/carmel-majidi.md) — central developer of biphasic LM architectures at CMU.
- [O. Burak Ozdoganlar](../authors/o-burak-ozdoganlar.md) — co-developer; manufacturing methods for biphasic circuits.
- Li, Wu & Lee (Sens. Actuators B, 2015) — key prior work on biphasic approach using Au wetting layers.
- Hirsch et al. (Adv. Mater., 2016) — demonstrated Au–Ga biphasic stretchable circuits.

## Related Concepts
- [EGaIn / Liquid Metal Alloys](../concepts/egain-liquid-metal-alloys.md) — the liquid phase of the biphasic system.
- [Selective Wetting](../concepts/selective-wetting.md) — the mechanism enabling self-aligned LM deposition onto the wetting layer.
- [Gallium Oxide (Ga₂O₃)](../concepts/gallium-oxide.md) — oxide removal is required before selective wetting activates.
- [Intermetallic Compound Formation](../concepts/intermetallic-compound-formation.md) — CuGa₂ forms at the Cu–EGaIn interface; essential for LM adhesion to the wetting layer.
- [Sputter Deposition on Elastomers](../methods/sputter-deposition-elastomers.md) — the method for depositing the solid Cu/Au wetting layer on PDMS.
- [HCl Vapor Soldering](../methods/hcl-vapor-soldering.md) — the method for integrating microelectronics with biphasic circuits.
- [PDMS](../concepts/pdms.md) — the standard elastomer substrate for biphasic circuits.
- [Stretchable Electronics](../themes/stretchable-electronics.md) — the broader application theme.

## Advantages Over Other LM Fabrication Approaches
- **vs. microfluidic channel injection**: No channel molding required; open-surface circuits are easier to integrate with microelectronics.
- **vs. direct writing**: Higher throughput, better scalability, finer linewidths (down to ~40 μm demonstrated); compatible with standard PCB-like process flows.
- **vs. screen printing**: Better resolution; no paste viscosity management needed.
- **Key enabling feature**: Compatible with standard pick-and-place machines for microelectronics integration — positions LM-based stretchable circuits as a potential drop-in extension of conventional PCB manufacturing.

## Fabrication Sequence (Ozutemiz et al. 2018)
1. Cast and cure PDMS elastomer substrate.
2. Sputter deposit Cr adhesion layer (~20 nm) + Cu wetting layer (~100 nm) on PDMS.
3. Pattern Cu/Cr by UV laser micromachining (or shadow mask during deposition).
4. Immerse in NaOH solution; deposit NaOH-treated EGaIn droplets onto Cu traces — LM selectively wets Cu.
5. Rinse with DI water and IPA; dry.
6. Place surface-mount components on LM pads.
7. Apply HCl vapor to "solder" LM to component pins.
8. Pour and cure top PDMS encapsulant layer.

## Source Support
- [Ozutemiz et al. 2018 — EGaIn–Metal Interfacing](../source-notes/ozutemiz-2018-egain-metal-interfacing.md)

## Open Questions
- Can biphasic architectures be extended to multilayer circuits without losing the self-alignment and sealing advantages?
- What is the scalability ceiling for the UV laser patterning step relative to industrial PCB production rates?
- How does the Cu wetting layer thickness (and resulting CuGa₂ formation) affect long-term circuit resistance?

## Tags
`egain` `liquid-metal` `fabrication` `stretchable-electronics` `biphasic` `soft-electronics`

---
title: "EGaIn–Metal Interfacing for Liquid Metal Circuitry and Microelectronics Integration"
type: source-note
author: "Kadri Bugra Ozutemiz, James Wissman, O. Burak Ozdoganlar, Carmel Majidi"
date: 2018
source-type: article
tags: [egain, liquid-metal, stretchable-electronics, microelectronics-integration, hcl-soldering, biphasic-electronics, soft-electronics, pdms]
created: 2026-06-28
updated: 2026-06-29
---

# EGaIn–Metal Interfacing for Liquid Metal Circuitry and Microelectronics Integration

**Author:** Kadri Bugra Ozutemiz, James Wissman, O. Burak Ozdoganlar, Carmel Majidi
**Year:** 2018
**Source type:** Article — *Advanced Materials Interfaces*, Vol. 5, 1701596
**DOI:** 10.1002/admi.201701596
**Raw file:** [Ozutemiz_et_al-2018-EGaIn–Metal Interfacing...](../../raw/articles/Ozutemiz_et_al-2018-EGaIn–Metal%20Interfacing%20for%20Liquid%20Metal%20Circuitry%20and%20Microelectronics%20Integration/)

## Summary
This paper investigates the electromechanical interface between EGaIn liquid metal interconnects and the pins of conventional surface-mount microelectronic components embedded in soft elastomers. The central contribution is a novel HCl vapor "soldering" technique that removes the gallium oxide skin from EGaIn and pin oxide simultaneously, enabling immediate, stable, and mechanically robust electrical connections that would otherwise fail or take hours to form. Combined with a biphasic circuit fabrication approach (Cu wetting layer on PDMS + selective EGaIn deposition), the method enables fully functional stretchable circuits with packaged IC chips demonstrating <8% measurement error under stretch.

## Key Claims
- Without HCl treatment, EGaIn–IC pin interfaces have a ~45% immediate failure rate, high resistance variability, and slow conductivity onset; HCl yields immediate, stable connections with resistance comparable to conventional solder paste (48.2 ± 2.0 mΩ vs. 47.2 ± 0.4 mΩ).
- HCl vapor acts as solder flux: removes Ga₂O₃ from EGaIn and oxide from component pins, exposing bulk EGaIn to wet and "solder" pins — directly analogous to flux in conventional PCB manufacturing.
- HCl treatment induces self-alignment of misaligned components via EGaIn's high surface tension (≈435 mN/m); first demonstration of this effect for EGaIn–microelectronics interfacing.
- HCl-treated circuits achieve 82.6 ± 13.3% strain at failure vs. 57.7 ± 7.9% untreated; survive 2000 cycles at 5–40% strain while untreated samples fail within 20 cycles.
- Ga diffuses into Au/Pd surface layers of IC pins but is blocked by the Ni diffusion barrier; no deep IC corruption observed after 4–6 months — standard IC packaging is inherently EGaIn-compatible.
- Cu preferred over Au as wetting layer: cheaper, ubiquitous, alloys with EGaIn, better adhesion to Cr adhesion layer.
- Minimum LM interconnect linewidth demonstrated: 40 μm.
- Mechanical failure (elastomer rupture at LM–pin interface) always precedes electrical failure — the LM interconnect itself is not the weak point.
- Explicit limitations: single-layer circuits only; incompatible with through-hole components and Al-contacted ICs; components must tolerate brief HCl vapor exposure.

## Connections

**Concepts:** [EGaIn / Liquid Metal Alloys](../concepts/egain-liquid-metal-alloys.md) · [Gallium Oxide (Ga₂O₃)](../concepts/gallium-oxide.md) · [Selective Wetting](../concepts/selective-wetting.md) · [Biphasic Stretchable Electronics](../concepts/biphasic-stretchable-electronics.md) · [PDMS](../concepts/pdms.md) · [Island-Bridge Architecture](../concepts/island-bridge-architecture.md) · [Soft-Rigid Interface / Mechanical Mismatch](../concepts/soft-rigid-interface-mechanical-mismatch.md) · [Electromechanical Coupling](../concepts/electromechanical-coupling.md) · [Cyclic Fatigue in Soft Electronics](../concepts/cyclic-fatigue-soft-electronics.md) · [Intermetallic Compound Formation](../concepts/intermetallic-compound-formation.md) · [Deterministic/Serpentine Architectures](../concepts/deterministic-serpentine-architectures.md) · [Percolating Network Conductors](../concepts/percolating-network-conductors.md) · [Conductive Polymers](../concepts/conductive-polymers.md)

**Methods:** [HCl Vapor Soldering](../methods/hcl-vapor-soldering.md) · [NaOH Treatment for Oxide Removal](../methods/naoh-oxide-removal.md) · [Sputter Deposition on Elastomers](../methods/sputter-deposition-elastomers.md) · [Finite Element Analysis for Soft Electronics](../methods/fea-soft-electronics.md)

**Themes:** [Stretchable Electronics](../themes/stretchable-electronics.md)

**Authors:** [Kadri Bugra Ozutemiz](../authors/bugra-ozutemiz.md) · [Carmel Majidi](../authors/carmel-majidi.md) · [O. Burak Ozdoganlar](../authors/o-burak-ozdoganlar.md)

**Projects:** [Flexible Circuit Roadblocks](../projects/flexible-circuit-roadblocks/index.md)

**Related source notes:** [Naserifar et al. 2016 — Material Gradients in Stretchable Substrates](../source-notes/naserifar-2016-material-gradients.md) — this paper cites Naserifar et al. (ref [61]) as the basis for the FEA-guided "three-body" soft-rigid interface analysis it identifies as future work.

## Direct Quotes

> "Ga-based LM alloys, such as eutectic Ga–In (EGaIn; 75% Ga and 25% In, by weight) and Ga–In–Sn (Galinstan; 68% Ga, 22% In, 10% Sn), can be incorporated into elastomers and preserve their elastic properties at all length scales and in all loading conditions without requiring specialized geometries. These alloys provide high electrical conductivity (3.4 × 10⁶ S m⁻¹), low melting point (−19 °C for Galinstan, 15 °C for EGaIn), low viscosity (2 mPa s), low toxicity, and negligible vapor pressure."

> "Gently blowing HCl vapor removes the oxide layer on LM and on component pins, and brings materials in contact to initiate soldering between LM leads and component pins. [...] This vapor-controlled removal of the gallium oxide to expose the bulk GaIn alloy is analogous to the role of solder flux in conventional soldering."

> "Having a copper wetting layer on the substrate is essential for this step—alloying between the liquid metal and copper prevents dewetting and removal of LM when exposed to HCl vapor. Without having this wetting layer, applying the vapor results in distortion of the circuit and degradation of the LM–substrate interface."

> "We observed that Ga is penetrated into Au and Au–Ga layer on the pin surface remains intact through the cleaning and sectioning steps. We also observed that penetrated Ga diffused through Au layer all the way to the Ni layer. However, Ga penetration was seen to stop at the Ni layer and no Ga is observed in the remaining layers."

> "In all cases we observed that the loss of conductivity is governed by mechanical rupture of the elastomer rather than electrical failure of the LM leads or LM-pin connections."

## Open Questions
- What are the long-term (>6 months) effects of Ga diffusion at the Au/Ni interface of IC pins? Does the Au–Ga intermetallic grow over time?
- Can multilayer LM circuit architectures be achieved without sacrificing the self-alignment and encapsulation benefits of the current single-layer approach?
- What less-corrosive alternatives to HCl vapor could enable LM oxide removal without risking component sensitivity?
- Can the strain limit at the LM–pin interface be improved through geometric design (e.g., FEA-guided graded stiffness encapsulants)?
- What is the minimum achievable pitch/linewidth before LM bridging becomes uncontrollable in dense circuits?

## Tags
`egain` `liquid-metal` `stretchable-electronics` `microelectronics-integration` `hcl-soldering` `biphasic-electronics` `soft-electronics` `pdms` `wearable`

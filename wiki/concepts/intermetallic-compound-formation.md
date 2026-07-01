---
title: "Intermetallic Compound Formation"
type: concept
tags: [egain, liquid-metal, materials, interfaces, reliability, metallurgy]
related: [egain-liquid-metal-alloys, selective-wetting, gallium-oxide, soft-rigid-interface-mechanical-mismatch, biphasic-stretchable-electronics]
created: 2026-06-28
updated: 2026-06-28
---

# Intermetallic Compound Formation

## Definition
The formation of stoichiometric alloy compounds at the interface between liquid metal (EGaIn, Galinstan) and solid metal contacts (Cu, Au, Sn, Ni, Pd). Unlike simple surface wetting or adhesion, intermetallic formation involves chemical reaction and alloying that creates a distinct compound layer with properties different from either parent material.

In EGaIn-based electronics, intermetallic formation is simultaneously:
- **Beneficial**: anchors LM to metal wetting layers and component pins, preventing dewetting.
- **Potentially problematic**: excessive intermetallic growth could increase contact resistance or embrittle interfaces over long timescales.

## Key Thinkers
- Tang et al. (ACS Appl. Mater. Interfaces, 2017) — reported CuGa₂ formation and In dispersion at Cu–EGaIn interface.
- Ralphs et al. (ACS Appl. Mater. Interfaces, 2018) — detailed Cu–Ga system intermetallic behavior for Galinstan.
- Morley et al. (Rev. Sci. Instrum., 2008) — Ni diffusion barrier behavior for GaInSn–Cu systems.

## Related Concepts
- [EGaIn / Liquid Metal Alloys](../concepts/egain-liquid-metal-alloys.md) — all Ga-based LMs form intermetallics with common contact metals.
- [Selective Wetting](../concepts/selective-wetting.md) — intermetallic formation is the driving force for LM's chemical affinity with metal wetting layers.
- [Gallium Oxide (Ga₂O₃)](../concepts/gallium-oxide.md) — oxide removal is required for Ga to access contact metal surfaces and form intermetallics.
- [Biphasic Stretchable Electronics](../concepts/biphasic-stretchable-electronics.md) — CuGa₂ formation at the Cu wetting layer anchors LM and is essential for HCl-treatment efficacy.

## Key Reactions and Findings

### Cu–EGaIn Interface
- Primary reaction: Ga + 2Cu → CuGa₂ (intermetallic compound).
- In is dispersed into the LM solution without alloying with Cu.
- The CuGa₂ layer anchors EGaIn to the Cu wetting layer; critically, this alloying *prevents dewetting* when HCl vapor is applied. Without a Cu wetting layer, HCl treatment causes LM to retract and distort the circuit.

### Au and Pd–EGaIn Interface (IC pin surface layers)
- Ga alloys with Au and Pd surface layers of IC pins; Au–Ga and Pd–Ga intermetallics form.
- Ga diffuses through Au and Pd layers and is immobilized by intermetallic formation — this may be why Ga penetration stops even before reaching the Ni barrier.

### Ni–EGaIn Interface (Diffusion Barrier)
- Ni acts as an effective diffusion barrier: Ga penetration stops at the Ni layer.
- No Ga observed in Cu or deeper IC layers after 4–6 months at room temperature.
- Consistent with findings for EGaIn–Al (Hunter & Williams 1984) and GaInSn–Cu (Morley et al. 2008).

### Sn–EGaIn Interface (Component pin coating)
- Reactive wetting: EGaIn wets Sn-coated pins slowly over hours to days without HCl — driven by Ga–Sn reactivity (Kramer et al., Langmuir 2014).
- HCl bypasses this slow reactive wetting by direct oxide removal and forced contact.

## Source Support
- [Ozutemiz et al. 2018 — EGaIn–Metal Interfacing](../source-notes/ozutemiz-2018-egain-metal-interfacing.md)

## Open Questions
- Does the CuGa₂ layer at the wetting layer interface grow over time, and does growth increase circuit resistance?
- What is the long-term growth kinetics of the Au–Ga intermetallic layer at IC pin surfaces?
- Can intermetallic formation be exploited deliberately (e.g., to bond LM to new contact materials or create graded interfaces)?

## Tags
`egain` `liquid-metal` `materials` `interfaces` `reliability` `metallurgy`

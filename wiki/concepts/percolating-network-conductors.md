---
title: "Percolating Network Conductors"
type: concept
tags: [stretchable-electronics, composites, conductors, alternative-approaches, soft-electronics, carbon]
related: [stretchable-electronics, egain-liquid-metal-alloys, conductive-polymers, deterministic-serpentine-architectures, electromechanical-coupling]
created: 2026-06-28
updated: 2026-06-28
---

# Percolating Network Conductors

## Definition
Stretchable conductors formed by dispersing rigid conductive particles or fibers (metallic nanoparticles, nanowires, carbon nanotubes, graphene) throughout a soft elastomeric matrix at concentrations above the percolation threshold. Electrical conductivity arises from particle-to-particle contacts forming a continuous conducting network through the composite. As the composite is stretched, particles rearrange and contact geometries change, causing resistance to increase.

Common filler materials:
- **Metallic**: silver nanowires (AgNW), gold nanoparticles, carbon black.
- **Carbon-based**: carbon nanotubes (CNT), graphene, graphene oxide.
- **Hybrid**: combinations of metallic and carbon fillers.

## Key Thinkers
- Zhenan Bao (Stanford) — pioneered stretchable organic and composite electronics including AgNW and carbon-based percolating networks.
- Someya, Sekitani et al. (Tokyo) — early demonstrations of ultrathin flexible electronics using percolating networks.
- D.J. Lipomi et al. — transparent stretchable conductors based on carbon nanotube networks.

## Related Concepts
- [Stretchable Electronics](../themes/stretchable-electronics.md) — percolating networks are one of the three main competing approaches.
- [EGaIn / Liquid Metal Alloys](../concepts/egain-liquid-metal-alloys.md) — EGaIn is explicitly contrasted with percolating networks as ~3 orders of magnitude more conductive.
- [Conductive Polymers](../concepts/conductive-polymers.md) — another low-conductivity alternative.
- [Deterministic/Serpentine Architectures](../concepts/deterministic-serpentine-architectures.md) — a third competing approach using conventional thin-film metals.
- [Electromechanical Coupling](../concepts/electromechanical-coupling.md) — percolating networks show strongly nonlinear and often hysteretic resistance-strain relationships.

## Key Properties and Limitations
- **Conductivity**: Typically ~10³–10⁴ S m⁻¹, compared to ~10⁶–10⁷ S m⁻¹ for bulk metals and ~3.4 × 10⁶ S m⁻¹ for EGaIn. Roughly 3 orders of magnitude below metallic conductivity.
- **Electromechanical coupling**: Resistance typically increases steeply under strain (piezoresistive effect); behavior is often nonlinear and hysteretic, making calibration difficult for precision sensing.
- **Processing**: Can be applied by printing, coating, or mixing into elastomers — potentially scalable.
- **Percolation threshold**: Must achieve sufficient filler loading for a continuous conductive network; below threshold, material is insulating; above threshold, conductivity rises sharply but may plateau.
- **Long-term stability**: Particle migration and contact degradation under repeated strain can cause irreversible resistance drift.

## Advantages Over Liquid Metal
- No containment challenge: solid composite doesn't leak or flow.
- Compatible with printing and coating processes.
- Some formulations are optically transparent (CNT, graphene networks).
- No exotic materials handling required.

## Source Support
- [Ozutemiz et al. 2018 — EGaIn–Metal Interfacing](../source-notes/ozutemiz-2018-egain-metal-interfacing.md) — cited as a competing approach with conductivity ~3 orders of magnitude below metals.

## Open Questions
- At what applications does the conductivity gap between percolating networks and LM actually matter, and at what scale is it negligible?
- Can hybrid approaches (LM + AgNW networks) combine LM's high conductivity with the mechanical robustness of a matrix composite?

## Tags
`stretchable-electronics` `composites` `conductors` `alternative-approaches` `soft-electronics` `carbon`

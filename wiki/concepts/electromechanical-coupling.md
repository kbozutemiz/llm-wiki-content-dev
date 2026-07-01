---
title: "Electromechanical Coupling"
type: concept
tags: [stretchable-electronics, mechanics, electrical, egain, characterization, soft-electronics]
related: [egain-liquid-metal-alloys, soft-rigid-interface-mechanical-mismatch, cyclic-fatigue-soft-electronics, biphasic-stretchable-electronics, stretchable-electronics]
created: 2026-06-28
updated: 2026-06-28
---

# Electromechanical Coupling

## Definition
The relationship between mechanical deformation (strain, bending, compression) and electrical properties (resistance, capacitance, inductance) in stretchable or flexible electronic systems. In the context of liquid metal electronics, electromechanical coupling primarily describes how the electrical resistance of LM interconnects changes as the circuit is stretched.

For a uniform LM trace under uniaxial strain, resistance change is governed purely by geometry (Ohm's law + incompressibility):

> ΔR/R₀ ≈ (1 + 2ν)ε + higher-order terms

where ε is applied strain and ν is Poisson's ratio of the elastomer. At moderate strains, this gives a predictable, approximately linear resistance increase. At high strains (typically >40–60% for embedded-component circuits), the relationship deviates significantly from theory due to LM flow into delamination voids at the soft-rigid interface.

## Key Thinkers
- [Carmel Majidi](../authors/carmel-majidi.md) — characterized electromechanical response of LM circuits including derivation of theoretical models.
- [O. Burak Ozdoganlar](../authors/o-burak-ozdoganlar.md) — co-investigator on electromechanical testing methodology.

## Related Concepts
- [EGaIn / Liquid Metal Alloys](../concepts/egain-liquid-metal-alloys.md) — LM's liquid nature means geometry changes (not conductivity changes) govern resistance response.
- [Soft-Rigid Interface / Mechanical Mismatch](../concepts/soft-rigid-interface-mechanical-mismatch.md) — mechanical failure at the chip–elastomer interface disrupts ideal electromechanical behavior at high strains.
- [Cyclic Fatigue in Soft Electronics](../concepts/cyclic-fatigue-soft-electronics.md) — repeated cycling causes resistance drift and eventual failure; electromechanical coupling behavior evolves with cycle count.
- [Biphasic Stretchable Electronics](../concepts/biphasic-stretchable-electronics.md) — biphasic architecture produces the LM traces whose electromechanical response is characterized.

## Observed Behavior in LM Circuits (Ozutemiz et al. 2018)
- **Low strain (<40–60%)**: ΔR/R₀ follows theoretical prediction well for both HCl-treated and untreated samples.
- **High strain (>40–60%)**: Significant deviation from theory due to LM redistribution — LM flows from narrow leads into delamination voids forming near the component–elastomer interface. The volumes of LM in the leads and pads are comparable, so this redistribution meaningfully changes circuit resistance.
- **Cyclic behavior**: Resistance decreases slightly over the first few hundred cycles before stabilizing — attributed to progressive optimization of the LM–pin contact geometry.
- **Analog vs. digital sensors**: Resistance change in LM interconnects affects analog sensor output (signal varies with strain); digital sensors are immune because they transmit discrete data values.

## Source Support
- [Ozutemiz et al. 2018 — EGaIn–Metal Interfacing](../source-notes/ozutemiz-2018-egain-metal-interfacing.md)

## Open Questions
- Can the high-strain electromechanical behavior be accurately modeled by incorporating LM flow and void formation into the theoretical framework?
- What circuit design strategies (trace geometry, LM reservoir volumes, encapsulant modulus) minimize resistance drift under cyclic loading?
- For sensor applications requiring calibrated analog output under stretch, how can the resistance-strain relationship be compensated in software?

## Tags
`stretchable-electronics` `mechanics` `electrical` `egain` `characterization` `soft-electronics`

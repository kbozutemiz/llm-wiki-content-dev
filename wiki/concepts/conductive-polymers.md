---
title: "Conductive Polymers"
type: concept
tags: [stretchable-electronics, polymers, conductors, alternative-approaches, organic-electronics, soft-electronics]
related: [stretchable-electronics, egain-liquid-metal-alloys, percolating-network-conductors, deterministic-serpentine-architectures, electromechanical-coupling]
created: 2026-06-28
updated: 2026-06-28
---

# Conductive Polymers

## Definition
Organic polymers with intrinsic electrical conductivity resulting from a conjugated backbone (alternating single and double carbon bonds) that allows delocalized electron transport. Unlike composites (where conductivity is achieved by adding conductive fillers), conductive polymers have conductivity as an intrinsic material property achieved through chemical doping.

Common examples:
- **PEDOT:PSS** (poly(3,4-ethylenedioxythiophene) polystyrene sulfonate) — the most widely used in flexible/stretchable electronics.
- **Polyaniline (PANI)**
- **Polypyrrole (PPy)**
- **Polythiophene derivatives**

## Key Thinkers
- Zhenan Bao (Stanford) — leading researcher in stretchable and skin-inspired electronics using PEDOT:PSS and related materials.
- Alberto Salleo (Stanford) — organic/mixed ionic-electronic conductors.
- George Whitesides (Harvard) — early flexible electronic systems using conductive polymer components.

## Related Concepts
- [Stretchable Electronics](../themes/stretchable-electronics.md) — conductive polymers are one of the major approaches to achieving stretchable conductor functionality.
- [EGaIn / Liquid Metal Alloys](../concepts/egain-liquid-metal-alloys.md) — LM is contrasted with conductive polymers as offering superior conductivity and electromechanical properties.
- [Percolating Network Conductors](../concepts/percolating-network-conductors.md) — closely related alternative; both suffer from the conductivity gap relative to metals.
- [Electromechanical Coupling](../concepts/electromechanical-coupling.md) — conductive polymers often exhibit strong piezoresistive effects and conductivity degradation under strain.

## Key Properties and Limitations
- **Conductivity**: Typically 10¹–10³ S m⁻¹ for standard PEDOT:PSS; engineered formulations can reach ~10³–10⁴ S m⁻¹. Still ~3 orders of magnitude below metallic conductivity.
- **Mixed ionic-electronic conductivity**: Many conductive polymers also conduct ions, making them relevant for bioelectronics and electrochemical devices — but complicating pure electronic applications.
- **Processing**: Solution-processable; can be deposited by spin-coating, inkjet printing, or screen printing — strong scalability advantage.
- **Biocompatibility**: Generally considered biocompatible and biologically relevant — advantage for implantable and epidermal electronics.
- **Electromechanical stability**: Conductivity typically decreases under strain due to disruption of the conjugated backbone and polymer chain alignment; generally poor electromechanical stability compared to LM.
- **Environmental stability**: Prone to degradation from moisture, oxygen, and UV light; encapsulation required for longevity.

## Advantages Over Liquid Metal
- No containment challenge: solid-phase material, no leakage.
- Biocompatible and ion-conducting — relevant for bioelectronics.
- Solution-processable: compatible with roll-to-roll and inkjet printing.
- Can be made transparent (thin films).
- Functionalization possible through polymer chemistry.

## Source Support
- [Ozutemiz et al. 2018 — EGaIn–Metal Interfacing](../source-notes/ozutemiz-2018-egain-metal-interfacing.md) — cited as a competing approach with poor electromechanical properties.

## Open Questions
- Can hybrid approaches combining conductive polymers (for biocompatible interfaces) with LM (for high-conductivity interconnects) create better overall soft-electronic systems?
- What is the minimum conductivity required for the interconnect layer in soft-robotic and wearable applications — does the polymer conductivity gap actually matter in practice?

## Tags
`stretchable-electronics` `polymers` `conductors` `alternative-approaches` `organic-electronics` `soft-electronics`

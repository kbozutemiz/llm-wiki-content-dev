---
title: "NaOH Treatment for Oxide Removal"
type: method
tags: [egain, liquid-metal, fabrication, oxide-removal, wet-chemistry, soft-electronics]
related: [egain-liquid-metal-alloys, gallium-oxide, selective-wetting, biphasic-stretchable-electronics, hcl-vapor-soldering]
created: 2026-06-28
updated: 2026-06-28
---

# NaOH Treatment for Oxide Removal

## Definition
A wet-chemical method for removing the gallium oxide (Ga₂O₃) skin from EGaIn surfaces and the native copper oxide from Cu wetting layers, enabling clean metal-to-metal contact and selective LM deposition. Sodium hydroxide (NaOH) solution (typically 3% w/w) is used either as a bath into which the substrate is immersed, or as a pretreatment applied directly to EGaIn droplets before deposition.

NaOH reacts with Ga₂O₃ to dissolve it, exposing bulk EGaIn with its high surface tension and metal-selective wetting behavior. It also removes the thin copper oxide layer that forms on the Cu wetting layer surface, allowing EGaIn to wet Cu directly.

## Related Concepts
- [Gallium Oxide (Ga₂O₃)](../concepts/gallium-oxide.md) — the oxide NaOH removes from EGaIn surfaces.
- [Selective Wetting](../concepts/selective-wetting.md) — NaOH treatment activates selective wetting by exposing bulk EGaIn.
- [EGaIn / Liquid Metal Alloys](../concepts/egain-liquid-metal-alloys.md) — the material whose surface is treated.
- [Biphasic Stretchable Electronics](../concepts/biphasic-stretchable-electronics.md) — NaOH treatment is a critical step in biphasic LM circuit fabrication.
- [HCl Vapor Soldering](../methods/hcl-vapor-soldering.md) — the complementary oxide removal method used later in the process for IC pin soldering.

## Process Details (Ozutemiz et al. 2018)
- **Solution**: 3% w/w NaOH (diluted from 30% stock with DI water).
- **Substrate immersion**: Elastomeric substrate is fully immersed in NaOH bath horizontally.
- **LM deposition**: NaOH-treated EGaIn droplets are immediately applied to the submerged substrate by dropper, allowing selective deposition onto Cu traces.
- **LM pretreatment**: EGaIn itself is also treated in the NaOH bath before application — both the substrate surface (Cu) and the LM surface are oxide-free at the moment of contact.
- **Cleaning**: After LM deposition, substrate is dipped horizontally in DI water then IPA; dried at 60 °C.
- **Excess LM removal**: If bridging occurs between traces, the substrate is dipped vertically into a fresh NaOH-treated LM bath, which pulls excess LM back into the bath.

## Role in Fabrication Sequence
NaOH treatment is Step 3 in the biphasic fabrication workflow:
1. Cast PDMS substrate.
2. Sputter Cr/Cu wetting layer and pattern.
3. **NaOH treatment + EGaIn deposition** ← this step.
4. Place components.
5. HCl vapor soldering.
6. Encapsulate with PDMS.

## Contrast with HCl Vapor Soldering
| | NaOH Treatment | HCl Vapor Soldering |
|---|---|---|
| Phase | Wet (liquid bath) | Dry (vapor) |
| Target | Cu wetting layer + bulk EGaIn surface | EGaIn at pin interface + pin oxide |
| Stage | Before component placement | After component placement |
| Function | Enable selective LM deposition | Enable LM–pin bonding |
| Risk | Bridging if excess LM applied | Component HCl sensitivity |

## Source Support
- [Ozutemiz et al. 2018 — EGaIn–Metal Interfacing](../source-notes/ozutemiz-2018-egain-metal-interfacing.md)

## Open Questions
- Can NaOH treatment be replaced or supplemented with less hazardous alternatives for scalable production?
- What is the effect of NaOH concentration and immersion time on Cu wetting layer surface quality and LM deposition uniformity?
- Does residual NaOH on the substrate surface affect long-term circuit performance or elastomer adhesion?

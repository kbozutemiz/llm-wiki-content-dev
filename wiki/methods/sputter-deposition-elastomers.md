---
title: "Sputter Deposition on Elastomers"
type: method
tags: [fabrication, thin-film, deposition, elastomers, pdms, soft-electronics, biphasic-electronics]
related: [biphasic-stretchable-electronics, egain-liquid-metal-alloys, selective-wetting, stretchable-electronics, soft-rigid-interface-mechanical-mismatch]
created: 2026-06-28
updated: 2026-06-28
---

# Sputter Deposition on Elastomers

## Definition
Physical vapor deposition (PVD) via sputtering to deposit thin metal films directly onto soft elastomeric substrates (most commonly PDMS). Because metals do not adhere well to elastomers, a thin adhesion layer (typically chromium, Cr) is deposited first, followed by the functional metal layer (typically copper, Cu, or gold, Au). The resulting bilayer thin-film defines the wetting layer geometry for biphasic LM circuit fabrication.

## Related Concepts
- [PDMS](../concepts/pdms.md) — the elastomer substrate onto which metal films are sputtered; poor metal–PDMS adhesion necessitates the Cr layer.
- [Biphasic Stretchable Electronics](../concepts/biphasic-stretchable-electronics.md) — sputter deposition creates the solid wetting layer that defines circuit geometry.
- [Selective Wetting](../concepts/selective-wetting.md) — the sputtered Cu or Au surface is where EGaIn selectively deposits.
- [EGaIn / Liquid Metal Alloys](../concepts/egain-liquid-metal-alloys.md) — the LM that deposits on the sputtered wetting layer.
- [Soft-Rigid Interface / Mechanical Mismatch](../concepts/soft-rigid-interface-mechanical-mismatch.md) — poor adhesion between thin metal films and elastomers is itself a form of mechanical mismatch; delamination of the sputtered layer is a failure mode.

## Process Details (Ozutemiz et al. 2018)
- **Substrate**: PDMS (Sylgard 184, 10:1 oligomer:curing agent, cured at 65 °C).
- **Adhesion layer**: Cr, ~20 nm, deposited at 30 W, 20 mTorr.
- **Functional layer**: Cu, ~100 nm, deposited at 30 W, 5 mTorr.
- **System**: Perkin-Elmer 8L sputter system.
- **Purpose of Cr**: Chromium bonds chemically to both PDMS and Cu, bridging the adhesion gap between the elastomer and metal.
- **Cu vs. Au choice**: Cu was selected over Au (used in earlier work) for lower cost, ubiquity in electronics manufacturing, and better adhesion to the Cr layer.

## Patterning After Deposition
After sputter deposition, the Cr/Cu bilayer is patterned to define circuit traces. Two approaches demonstrated:
1. **UV laser micromachining (UVLM)**: Direct ablation removes unwanted Cr/Cu, leaving defined traces. Resolution: down to ~40 μm linewidth.
2. **Shadow mask/stencil**: A laser-cut stencil mask is placed over the substrate during sputtering, so metal deposits only in the desired pattern. No post-deposition patterning needed; lower resolution.

## Key Challenges
- **Metal–elastomer adhesion**: PDMS is notoriously difficult to bond metal films to; Cr adhesion layer is essential but can still delaminate under large strains or repeated cycling.
- **Thermal budget**: PDMS has a relatively low thermal tolerance; sputter deposition parameters must avoid excessive substrate heating.
- **Residual stress**: Thin metal films on elastomers develop residual stresses during deposition; these can cause film buckling, cracking, or delamination before any external strain is applied.
- **Surface cleanliness**: PDMS outgasses silicone oligomers that can contaminate the sputter chamber and degrade film adhesion.

## Source Support
- [Ozutemiz et al. 2018 — EGaIn–Metal Interfacing](../source-notes/ozutemiz-2018-egain-metal-interfacing.md)

## Open Questions
- What is the maximum strain that a Cr/Cu bilayer on PDMS can sustain before delamination — and does this set a ceiling on circuit stretchability independent of the LM?
- Can alternative deposition methods (e-beam evaporation, ALD, electrodeposition) provide better adhesion or thinner functional layers?
- How does the sputtered Cu layer thickness affect intermetallic (CuGa₂) growth rate and long-term circuit resistance?

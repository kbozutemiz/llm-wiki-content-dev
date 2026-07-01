---
title: "PDMS (Polydimethylsiloxane)"
type: concept
tags: [pdms, elastomer, substrate, soft-materials, microfabrication, stretchable-electronics]
related: [graded-stiffness-substrate, sputter-deposition-elastomers, biphasic-stretchable-electronics, interfacial-adhesion-energy, soft-rigid-interface-mechanical-mismatch]
created: 2026-06-29
updated: 2026-06-29
---

# PDMS (Polydimethylsiloxane)

## Definition
Polydimethylsiloxane (PDMS) is a silicone elastomer that is the dominant soft substrate material in flexible and stretchable electronics, soft robotics, and microfluidics. It is a two-part system (base oligomer + curing agent) that cross-links on curing into a transparent, biocompatible, chemically stable elastomer. The most widely used commercial formulation is **Sylgard 184** (Dow Corning).

PDMS is valued for: optical transparency, biocompatibility, low cost, ease of molding and spin-coating, chemical inertness, gas permeability, and — critically — a **tunable Young's modulus** set by the base-to-curing-agent mixing ratio.

## Key Properties
| Property | Value / Note |
|---|---|
| Young's modulus | ~0.1–3 MPa (tunable via mixing ratio) |
| E at 5:1 ratio | 1.98 MPa (stiffer) |
| E at 20:1 ratio | 0.26 MPa (softer) |
| Standard ratio | 10:1 base:curing agent |
| Transparency | Optically clear |
| Biocompatibility | High |
| Cure | Thermal (e.g., 65–80 °C) |

## Modulus Tuning via Mixing Ratio
A central process technique: the elastomer base-to-curing-agent ratio controls cross-link density and therefore stiffness. A higher base fraction (e.g., 20:1) yields a softer, more compliant material; a lower ratio (e.g., 5:1) yields a stiffer one. Because all variants are the same polymer chemistry, two different-modulus PDMS regions **bond to each other extremely strongly** (PDMS–PDMS work of adhesion 250–300 J m⁻²) — a property exploited in [graded stiffness substrates](../concepts/graded-stiffness-substrate.md) to build a stiffness gradient without introducing a weak material interface.

## Key Thinkers
- [Philip R. LeDuc](../authors/philip-leduc.md) — used dual-ratio PDMS to build stiffness gradients for chip embedding.
- [Carmel Majidi](../authors/carmel-majidi.md) — PDMS as substrate for liquid-metal stretchable circuits.
- [O. Burak Ozdoganlar](../authors/o-burak-ozdoganlar.md) — PDMS microfabrication and precision processing.

## Related Concepts
- [Graded Stiffness Substrate](../concepts/graded-stiffness-substrate.md) — built from two PDMS mixing ratios with strong mutual bonding.
- [Sputter Deposition on Elastomers](../methods/sputter-deposition-elastomers.md) — metal wetting layers are sputtered onto PDMS (requires Cr adhesion layer due to poor metal–PDMS adhesion).
- [Biphasic Stretchable Electronics](../concepts/biphasic-stretchable-electronics.md) — PDMS is the standard substrate for biphasic liquid-metal circuits.
- [Interfacial Adhesion Energy](../concepts/interfacial-adhesion-energy.md) — PDMS–PDMS adhesion is ~10⁴× stronger than Si–PDMS adhesion.
- [Soft-Rigid Interface / Mechanical Mismatch](../concepts/soft-rigid-interface-mechanical-mismatch.md) — PDMS (kPa–MPa) against Si (170 GPa) embodies the mismatch problem.

## Role Across the Wiki's Sources
- **Naserifar et al. 2016**: Two PDMS ratios (5:1 and 20:1) form the stiffness gradient; modulus measured via Instron.
- **Ozutemiz et al. 2018**: PDMS (Sylgard 184, 10:1) is the substrate for EGaIn biphasic circuits; Cr/Cu sputtered on top; oxygen-plasma activated for sealing.

## Source Support
- [Naserifar et al. 2016 — Material Gradients in Stretchable Substrates](../source-notes/naserifar-2016-material-gradients.md)
- [Ozutemiz et al. 2018 — EGaIn–Metal Interfacing](../source-notes/ozutemiz-2018-egain-metal-interfacing.md)

## Open Questions
- What is the practical modulus range achievable through mixing-ratio tuning alone before mechanical or curing properties degrade?
- How do PDMS surface properties (hydrophobic recovery, oligomer migration) affect long-term adhesion and device reliability?
- How does PDMS compare to alternative elastomers (Ecoflex, polyurethane) for graded-substrate and liquid-metal applications?

## Tags
`pdms` `elastomer` `substrate` `soft-materials` `microfabrication` `stretchable-electronics`

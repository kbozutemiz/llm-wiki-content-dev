---
title: "Energy Release Rate"
type: concept
tags: [fracture-mechanics, delamination, mechanics, design-metric, soft-rigid-interface, stretchable-electronics]
related: [interfacial-adhesion-energy, soft-rigid-interface-mechanical-mismatch, graded-stiffness-substrate, strain-shielding, fea-soft-electronics]
created: 2026-06-29
updated: 2026-06-29
---

# Energy Release Rate

## Definition
The energy release rate, denoted **G** (units: J m⁻²), is a fracture-mechanics quantity describing the energy available to drive the growth of a crack per unit area of new crack surface. It represents the mechanical *driving force* for crack propagation (here, delamination at a material interface).

A crack grows when G reaches a critical value — the **fracture energy** (or critical energy release rate) **Γ**, which is the material/interface *resistance* to crack growth. The delamination criterion is therefore:

> Crack propagates when **G ≥ Γ**

In stretchable electronics, G is computed for cracks (incipient delaminations) at the interface between rigid embedded components and the soft substrate. Comparing the computed G to the interface's known adhesion energy (Γ) predicts whether delamination will occur under a given strain.

## Key Thinkers
- [Philip R. LeDuc](../authors/philip-leduc.md) — applied energy release rate as a design metric for chip-embedded stretchable substrates.
- [Gary K. Fedder](../authors/gary-fedder.md) — co-developed the energy-release-rate-guided design approach.
- Classical fracture mechanics lineage (Griffith; Li, Shih & Needleman 1985, cited) — foundational theory of crack-driving energy balance.

## Related Concepts
- [Interfacial Adhesion Energy](../concepts/interfacial-adhesion-energy.md) — the resistance term (Γ) against which G is compared; together they determine delamination.
- [Soft-Rigid Interface / Mechanical Mismatch](../concepts/soft-rigid-interface-mechanical-mismatch.md) — G quantifies the delamination risk this mismatch creates.
- [Graded Stiffness Substrate](../concepts/graded-stiffness-substrate.md) — the gradient design is evaluated and optimized by minimizing G at the critical interface.
- [Strain Shielding](../concepts/strain-shielding.md) — reducing local interfacial strain lowers G.
- [Finite Element Analysis for Soft Electronics](../methods/fea-soft-electronics.md) — the computational method used to calculate G.

## Key Behavior and Findings (Naserifar et al. 2016)
- **Computation method**: G is determined by computing the strain energy before and after a small crack extension and dividing the difference by the new crack area (via FEA with mesh-convergence verification).
- **Quadratic strain dependence**: G increases approximately quadratically with applied strain — so modest reductions in local strain produce large reductions in delamination risk.
- **Design-parameter dependence**: G = f(a, E₁, E₂, ε, L₁, L₂, h₁, h₂, h₃), where a = crack length, ε = applied strain, and the L/h terms are gradient geometry.
- **Representative values** (Si chip 1×1×0.05 mm, 20% strain):
  | Sample | Configuration | G [J m⁻²] |
  |---|---|---|
  | #1 | PDMS (5:1) only | 10.99 |
  | #2 | PDMS (20:1) only | 1.493 |
  | #3 | Gradient (20:1 primary + 5:1 intermediate) | 0.689 |
- **Interface comparison**: G at the Si–PDMS interface is ~2× higher than at the PDMS–PDMS interface for comparable geometry — but the PDMS–PDMS interface tolerates vastly higher G because its Γ is ~4 orders of magnitude larger.
- **Geometry effect**: Chip corners are the highest-G locations and the delamination initiation sites; rounding corners reduces G.

## Why It Matters as a Design Metric
Energy release rate converts an intuitive reliability concern (delamination) into a computable, optimizable quantity. It allows designers to (i) compare candidate substrate architectures quantitatively, (ii) identify which interface will fail first, and (iii) optimize geometric parameters (gradient length, layer thickness, chip shape) before fabrication.

## Source Support
- [Naserifar et al. 2016 — Material Gradients in Stretchable Substrates](../source-notes/naserifar-2016-material-gradients.md)

## Open Questions
- How reliable are computed G values given the wide reported scatter in critical adhesion energies (Γ) for soft-rigid interfaces?
- Can energy-release-rate-based optimization be extended to dynamic/cyclic loading where fatigue crack growth (rather than monotonic) governs?
- How does G behave for liquid-metal interconnect interfaces (cf. Ozutemiz 2018) versus solid Si–polymer interfaces?

## Tags
`fracture-mechanics` `delamination` `mechanics` `design-metric` `soft-rigid-interface` `stretchable-electronics`

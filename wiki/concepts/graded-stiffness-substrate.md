---
title: "Graded Stiffness Substrate"
type: concept
tags: [stretchable-electronics, material-gradient, delamination, soft-rigid-interface, mechanics, cmos-integration]
related: [soft-rigid-interface-mechanical-mismatch, strain-shielding, energy-release-rate, interfacial-adhesion-energy, island-bridge-architecture]
created: 2026-06-29
updated: 2026-06-29
---

# Graded Stiffness Substrate

## Definition
A stretchable substrate design strategy in which one or more intermediate materials of graduated stiffness are placed between a rigid embedded component (e.g., a silicon chip) and the soft primary substrate, so that mechanical stiffness transitions gradually rather than abruptly across the soft-rigid boundary. The gradient redistributes mechanical strain — moving the peak strain away from the vulnerable rigid–soft interface — thereby reducing the driving force for delamination.

The gradient can be:
- **Discrete** — one or a few intermediate layers, each with a stiffness between its neighbors (the approach demonstrated by Naserifar et al. 2016).
- **Continuous** — a smoothly varying stiffness profile achieved through process innovation (identified as future work).

## Key Thinkers
- [Philip R. LeDuc](../authors/philip-leduc.md) — co-developed the intermediate-material gradient approach for chip-embedded stretchable substrates.
- [Gary K. Fedder](../authors/gary-fedder.md) — co-developed the approach; brings MEMS/CMOS integration perspective.
- Naser Naserifar — first author; designed and validated the two-PDMS gradient system.

## Related Concepts
- [Soft-Rigid Interface / Mechanical Mismatch](../concepts/soft-rigid-interface-mechanical-mismatch.md) — the gradient substrate is a direct mitigation strategy for the mismatch problem.
- [Strain Shielding](../concepts/strain-shielding.md) — the mechanism by which the gradient works: intermediate stiffness shields the critical interface from peak strain.
- [Energy Release Rate](../concepts/energy-release-rate.md) — the fracture-mechanics metric used to quantify the gradient's benefit.
- [Interfacial Adhesion Energy](../concepts/interfacial-adhesion-energy.md) — the gradient relocates failure to a polymer–polymer interface with far higher adhesion energy.
- [Island-Bridge Architecture](../concepts/island-bridge-architecture.md) — the gradient substrate stabilizes the rigid "island" sites in this architecture.
- [PDMS](../concepts/pdms.md) — the model material system; modulus tuned by mixing ratio to create the gradient.

## How It Works (Naserifar et al. 2016)
1. A stiffer intermediate elastomer (E₂) is placed in direct contact with the rigid silicon chip.
2. A softer primary elastomer (E₁ < E₂) occupies the outer domain.
3. Under stretch, the soft outer material absorbs most of the strain; the stiffer intermediate material near the chip strains far less.
4. Peak strain — and thus peak energy release rate — is moved off the Si–polymer interface and onto the polymer–polymer interface.
5. Because polymer–polymer adhesion vastly exceeds Si–polymer adhesion, the system tolerates far higher global strain before failure.

## Key Design Parameters
- **E₂/E₁ ratio**: Higher ratios lower the energy release rate (E₂/E₁ = 100 outperforms 10). In the experimental PDMS system, E₂/E₁ ≈ 7.6 (1.98 MPa / 0.26 MPa).
- **L₂/L ratio** (intermediate length / total length): A small fraction is optimal — L₂/L = 0.05 gave the highest failure strain (140%). Both extremes (L₂/L = 0 and = 1, i.e., single materials) perform poorly.
- **Chip corner geometry**: Rounded or circular chips reduce energy release rate versus square chips.
- **Layer thicknesses** (h₁, h₂, h₃): Enter the energy release rate function and affect optimal design.

## Quantitative Result
| Configuration | Failure strain |
|---|---|
| Single stiff PDMS (5:1) | ~20% |
| Single soft PDMS (20:1) | ~30% |
| Two-material gradient (L₂/L = 0.05) | 140% |

A ~6× improvement in failure strain from adding a single intermediate layer.

## Source Support
- [Naserifar et al. 2016 — Material Gradients in Stretchable Substrates](../source-notes/naserifar-2016-material-gradients.md)

## Open Questions
- Can a continuous stiffness gradient eliminate the residual polymer–polymer failure interface entirely?
- How do optimal gradient parameters scale with chip size, aspect ratio, and number of embedded chips?
- Can graded substrates be combined with stretchable interconnect technologies (serpentine, liquid metal) without reintroducing interface failures at the interconnect crossing?

## Tags
`stretchable-electronics` `material-gradient` `delamination` `soft-rigid-interface` `mechanics` `cmos-integration`

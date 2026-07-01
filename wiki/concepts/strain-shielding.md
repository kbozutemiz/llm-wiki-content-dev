---
title: "Strain Shielding"
type: concept
tags: [mechanics, stretchable-electronics, strain-management, delamination, soft-rigid-interface, material-gradient]
related: [graded-stiffness-substrate, soft-rigid-interface-mechanical-mismatch, energy-release-rate, island-bridge-architecture, electromechanical-coupling]
created: 2026-06-29
updated: 2026-06-29
---

# Strain Shielding

## Definition
Strain shielding (also called strain redistribution or local strain suppression) is a mechanical design principle in which stiffer material elements are placed so as to divert mechanical strain *away* from a vulnerable region — typically a strain-sensitive component or a weak interface — so that the protected region experiences far less deformation than the globally applied strain. The stiffer element carries proportionally less strain (for a given stress, strain scales inversely with modulus), "shielding" the adjacent sensitive zone.

In stretchable electronics, strain shielding protects (i) rigid components from cracking, and (ii) weak material interfaces from delamination, by ensuring the applied strain is preferentially absorbed elsewhere in the structure.

## Key Thinkers
- [Philip R. LeDuc](../authors/philip-leduc.md) — used intermediate stiffness layers to shield the Si–polymer interface from peak strain.
- [Gary K. Fedder](../authors/gary-fedder.md) — co-developed the strain-redistribution substrate design.

## Related Concepts
- [Graded Stiffness Substrate](../concepts/graded-stiffness-substrate.md) — the substrate architecture that implements strain shielding via a stiffness gradient.
- [Soft-Rigid Interface / Mechanical Mismatch](../concepts/soft-rigid-interface-mechanical-mismatch.md) — strain shielding is a mitigation for interface delamination caused by the mismatch.
- [Energy Release Rate](../concepts/energy-release-rate.md) — reducing local interfacial strain (via shielding) lowers the energy release rate quadratically.
- [Island-Bridge Architecture](../concepts/island-bridge-architecture.md) — rigid islands intrinsically shield their housed electronics; substrate shielding extends protection to the island interface.
- [Electromechanical Coupling](../concepts/electromechanical-coupling.md) — shielding strain-sensitive interconnects also stabilizes their electrical response under deformation.

## Mechanisms and Implementations
- **Stiffness gradient within the substrate** (Naserifar et al. 2016): A stiffer intermediate elastomer adjacent to the chip strains less, moving peak strain to the outer soft region and the polymer–polymer interface. Strain at the Si interface dropped ~6× versus a single-material substrate.
- **Stiff patches / local reinforcement** (prior approaches): Embedding stiff PET or SU8 patches around devices to locally suppress strain. Distinguished from the gradient approach because patches sit at the surface (no embedded interface bearing normal stress) whereas the gradient operates within the substrate around a fully embedded chip.
- **Thin polymer encasements**: Encasing interconnects in relatively stiff thin films (e.g., polyimide) to suppress device-local strain — used in stretchable batteries (PI/Cu/PI laminates).

## Why It Works
Because energy release rate scales approximately quadratically with local strain, even a moderate reduction in interfacial strain yields a large reduction in delamination driving force. Strain shielding is thus a high-leverage strategy: redirecting strain a short distance away from a weak interface disproportionately improves reliability.

## Source Support
- [Naserifar et al. 2016 — Material Gradients in Stretchable Substrates](../source-notes/naserifar-2016-material-gradients.md)

## Open Questions
- What is the optimal spatial profile of stiffness (step, linear, exponential) for maximal strain shielding at minimal added stiffness?
- How does strain shielding trade off against overall system compliance — does over-shielding stiffen the system too much for its application?
- Can strain shielding be made adaptive or tunable (e.g., via stiffness-changing materials) for variable loading conditions?

## Tags
`mechanics` `stretchable-electronics` `strain-management` `delamination` `soft-rigid-interface` `material-gradient`

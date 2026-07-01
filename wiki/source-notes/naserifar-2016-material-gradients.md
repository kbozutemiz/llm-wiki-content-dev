---
title: "Material Gradients in Stretchable Substrates toward Integrated Electronic Functionality"
type: source-note
author: "Naser Naserifar, Philip R. LeDuc, Gary K. Fedder"
date: 2016
source-type: article
tags: [stretchable-electronics, delamination, material-gradient, energy-release-rate, soft-rigid-interface, pdms, cmos-integration, fracture-mechanics]
created: 2026-06-29
updated: 2026-06-29
---

# Material Gradients in Stretchable Substrates toward Integrated Electronic Functionality

**Author:** Naser Naserifar, Philip R. LeDuc, Gary K. Fedder
**Year:** 2016
**Source type:** Article (Communication) — *Advanced Materials*, Vol. 28, pp. 3584–3591
**Raw file:** [Material Gradients in Stretchable Substrates...](../../raw/articles/Naserifar_et_al-2016/)

## Summary
This paper addresses the dominant failure mode in chip-embedded stretchable electronics: delamination at the rigid silicon–soft polymer interface under strain. The authors introduce a single intermediate elastomer layer — stiffer than the primary substrate but softer than silicon — that creates a stiffness gradient redirecting peak strain away from the vulnerable Si–polymer interface. This reduces the fracture-mechanics energy release rate at that interface and shifts eventual failure to the polymer–polymer interface, where adhesion is roughly four orders of magnitude stronger. The result is a sixfold improvement in failure strain (from ~20% to 140%), validated by coupled finite-element analysis and tensile experiments using PDMS of two mixing ratios.

This source is the quantitative companion to [Ozutemiz et al. 2018](../source-notes/ozutemiz-2018-egain-metal-interfacing.md), which cites it (ref. [61]) as the basis for FEA-guided understanding of strain distribution, stress concentration, and delamination at the soft-rigid interface in chip-embedded elastomers.

## Key Claims
- Delamination at the Si–polymer interface — not electrical failure or interconnect rupture — is the primary failure mode when embedding rigid chips in stretchable substrates.
- Si–PDMS interfacial adhesion energy (0.05–0.4 J m⁻²) is roughly **four orders of magnitude weaker** than PDMS–PDMS adhesion (250–300 J m⁻²); the strategy exploits this by relocating the critical interface to a polymer–polymer boundary.
- A single intermediate stiffness layer reduces the energy release rate at the Si interface by enough to raise failure strain from ~20% (single stiff PDMS) to 140% — a ~6× improvement.
- Strain at the silicon interface in the gradient substrate is ~6× lower than in a single-material substrate (FEA, maximum principal elastic strain).
- The optimal intermediate-layer fraction is small and counterintuitive: L₂/L = 0.05 (5% of substrate length) gives the highest failure strain (140%).
- Energy release rate scales approximately **quadratically** with applied strain; small reductions in local interfacial strain yield large delamination-resistance gains.
- Higher Young's-modulus ratio (E₂/E₁) between intermediate and primary materials lowers the energy release rate; E₂/E₁ = 100 outperforms E₂/E₁ = 10 across all intermediate lengths.
- Delamination initiates at chip corners; rounded or circular chips reduce the energy release rate versus square chips.
- PDMS modulus is tuned via base-to-curing-agent mixing ratio: 5:1 → 1.98 MPa; 20:1 → 0.26 MPa — enabling two "different" materials that still bond strongly because they are the same polymer.
- Cyclic loading to 100 cycles at 50% maximum strain produced no detectable delamination at either interface.
- Approach targets embedding "thick" (>10 µm) silicon chips mimicking real CMOS stacks, in contrast to ultrathin-silicon flexibility strategies.

## Connections

**Concepts:** [Graded Stiffness Substrate](../concepts/graded-stiffness-substrate.md) · [Energy Release Rate](../concepts/energy-release-rate.md) · [Interfacial Adhesion Energy](../concepts/interfacial-adhesion-energy.md) · [Strain Shielding](../concepts/strain-shielding.md) · [Island-Bridge Architecture](../concepts/island-bridge-architecture.md) · [Soft-Rigid Interface / Mechanical Mismatch](../concepts/soft-rigid-interface-mechanical-mismatch.md) · [Cyclic Fatigue in Soft Electronics](../concepts/cyclic-fatigue-soft-electronics.md) · [PDMS](../concepts/pdms.md) · [Deterministic/Serpentine Architectures](../concepts/deterministic-serpentine-architectures.md)

**Methods:** [Finite Element Analysis for Soft Electronics](../methods/fea-soft-electronics.md) · [Spin Coating](../methods/spin-coating.md) · [Handle-Wafer Transfer](../methods/handle-wafer-transfer.md)

**Themes:** [Stretchable Electronics](../themes/stretchable-electronics.md)

**Authors:** [Philip R. LeDuc](../authors/philip-leduc.md) · [Gary K. Fedder](../authors/gary-fedder.md)

**Projects:** [Flexible Circuit Roadblocks](../projects/flexible-circuit-roadblocks/index.md)

**Related source notes:** [Ozutemiz et al. 2018 — EGaIn–Metal Interfacing](../source-notes/ozutemiz-2018-egain-metal-interfacing.md) — cites this paper for soft-rigid interface failure mechanics.

## Direct Quotes

> "One major challenge is the significant mismatch in mechanical properties of silicon-based electronics (Young's modulus, E = 170 GPa) and soft materials mimicking those of the human body (Young's modulus, E = 100 kPa)." (p. 3584)

> "Our work introduces a stiffness gradient within the stretchable substrate that moves the peak strain away from the rigid/elastomeric interface." (p. 3586)

> "Investigators have reported values in the range of 0.05–0.4 J m⁻² for the adhesion energy of Si–PDMS interfaces. The work of adhesion for a PDMS–PDMS interface is reported in the range of 250–300 J m⁻². Therefore, the PDMS–PDMS bonding is stronger than Si–PDMS bonding by four orders of magnitude." (p. 3589)

> "With this approach, 140% strain before failure is achievable, while similar structures without intermediate soft material fail at ≈20% strain." (p. 3590)

> "The presented method of moving the critical interface to the PDMS–PDMS interface enables exploitation of the natural adhesion between similar polymers." (p. 3589)

## Open Questions
- Can a continuous stiffness gradient (rather than discrete layers) be fabricated, and would it eliminate the PDMS–PDMS interface as a failure site entirely?
- How does the optimal L₂/L ratio change with chip size, chip aspect ratio, and substrate thickness?
- How does the gradient approach interact with functional interconnects (e.g., serpentine PI-Cu, or liquid-metal traces) routed across the Si–polymer boundary?
- Does the 100-cycle fatigue result hold to the thousands/millions of cycles required for wearable products?
- Can this gradient strategy be combined with liquid-metal interconnect approaches (cf. Ozutemiz 2018) to address both interconnect and chip-anchoring failure simultaneously?

## Tags
`stretchable-electronics` `delamination` `material-gradient` `energy-release-rate` `soft-rigid-interface` `pdms` `cmos-integration` `fracture-mechanics`

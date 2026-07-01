---
title: "Cyclic Fatigue in Soft Electronics"
type: concept
tags: [stretchable-electronics, mechanics, failure, fatigue, reliability, soft-electronics]
related: [soft-rigid-interface-mechanical-mismatch, electromechanical-coupling, egain-liquid-metal-alloys, biphasic-stretchable-electronics, stretchable-electronics]
created: 2026-06-28
updated: 2026-06-29
---

# Cyclic Fatigue in Soft Electronics

## Definition
The progressive mechanical and electrical degradation of soft and stretchable electronic circuits under repeated loading cycles (stretching, bending, compression). Unlike monotonic failure (strain-to-failure), cyclic fatigue describes how circuits fail over time at strain levels well below the single-cycle failure threshold — a critical consideration for wearable and implantable applications where circuits must endure thousands to millions of cycles over their operational lifetime.

In LM-based soft electronics, the dominant fatigue mechanism is crack initiation and propagation at the soft-rigid interface (chip–elastomer boundary), rather than degradation of the LM interconnect itself.

## Key Thinkers
- [Carmel Majidi](../authors/carmel-majidi.md) — published cyclic fatigue data for LM circuits with and without HCl treatment.
- [O. Burak Ozdoganlar](../authors/o-burak-ozdoganlar.md) — co-investigator on cyclic testing methodology.

## Related Concepts
- [Soft-Rigid Interface / Mechanical Mismatch](../concepts/soft-rigid-interface-mechanical-mismatch.md) — the primary site of fatigue crack initiation in LM circuits with embedded components.
- [Electromechanical Coupling](../concepts/electromechanical-coupling.md) — resistance drift over cycles is the electrical signature of fatigue progression.
- [EGaIn / Liquid Metal Alloys](../concepts/egain-liquid-metal-alloys.md) — LM circuits without embedded components show better cyclic durability than those with rigid chips.
- [HCl Vapor Soldering](../methods/hcl-vapor-soldering.md) — HCl treatment dramatically improves fatigue resistance by improving interface geometry.

## Key Findings (Ozutemiz et al. 2018)
- Protocol: 2000 cycles at 5–40% strain (0.1 Hz, sawtooth waveform).
- **HCl-treated with embedded component**: All 3 samples completed 2000 cycles without failure.
- **Untreated with embedded component**: All 3 initial samples failed within 20 cycles; of 4 additional replacement samples, only 1 survived 2000 cycles.
- **HCl-treated without component**: All samples survived 2000 cycles.
- Failure mode: crack propagation at LM–component interface, growing with each cycle until complete failure.
- Resistance trend: All surviving samples show a slight decrease in resistance over the first few hundred cycles, stabilizing thereafter — attributed to progressive seating of the LM–pin contact.
- Caveat: 2000 cycles is a preliminary data point; a complete S-N fatigue study has not been conducted.

## Implications for Commercialization
Cyclic fatigue performance is a critical reliability metric for any wearable or soft-robotic application. The stark difference between HCl-treated and untreated circuits (2000 vs. <20 cycles) means that microelectronics integration method is not merely a processing convenience but a direct determinant of product lifetime.

## Corroborating Evidence: Graded-Substrate Chip Embedding (Naserifar et al. 2016)
A graded-stiffness substrate embedding a rigid silicon chip was cycled 100 times to 50% maximum strain with **no detectable delamination** at either the Si–PDMS or PDMS–PDMS interface. This reinforces the central pattern: when the soft-rigid interface is mechanically protected (here by a [graded stiffness substrate](../concepts/graded-stiffness-substrate.md), in Ozutemiz et al. by HCl-vapor encapsulation of pins), cyclic durability improves dramatically. As with the LM circuits, the caveat is that 100 cycles is a preliminary figure well short of product-lifetime requirements.

## Source Support
- [Ozutemiz et al. 2018 — EGaIn–Metal Interfacing](../source-notes/ozutemiz-2018-egain-metal-interfacing.md) — 2000-cycle testing of LM circuits; HCl treatment critical for survival.
- [Naserifar et al. 2016 — Material Gradients in Stretchable Substrates](../source-notes/naserifar-2016-material-gradients.md) — 100-cycle, 50%-strain testing of graded-substrate chip embedding with no delamination.

## Open Questions
- What is the actual fatigue life (in cycles) of HCl-treated LM circuits — does performance hold beyond 2000 cycles?
- How does fatigue performance scale with strain amplitude? With frequency?
- Do LM circuits without embedded rigid components (pure LM traces in elastomer) have a fundamentally different fatigue mechanism?
- What encapsulant or interface design modifications could extend cyclic fatigue life toward millions of cycles needed for commercial wearables?

## Tags
`stretchable-electronics` `mechanics` `failure` `fatigue` `reliability` `soft-electronics`

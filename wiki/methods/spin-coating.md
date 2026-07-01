---
title: "Spin Coating"
type: method
tags: [fabrication, thin-film, pdms, deposition, microfabrication, stretchable-electronics]
related: [pdms, handle-wafer-transfer, graded-stiffness-substrate, sputter-deposition-elastomers, biphasic-stretchable-electronics]
created: 2026-06-29
updated: 2026-06-29
---

# Spin Coating

## Definition
A thin-film deposition technique in which a liquid precursor (e.g., uncured PDMS, photoresist, polymer solution) is dispensed onto a substrate that is then rotated at high speed. Centrifugal force spreads the liquid into a uniform film whose thickness is controlled by spin speed, time, and precursor viscosity. After spinning, the film is cured (thermally or by UV) to solidify. Spin coating is a workhorse of microfabrication and a primary method for building layered elastomer structures in soft electronics.

## Related Concepts
- [PDMS](../concepts/pdms.md) — the most common material spin-coated in soft electronics; thickness set by spin parameters and mixing ratio (viscosity).
- [Handle-Wafer Transfer](../methods/handle-wafer-transfer.md) — spin coating is typically performed on a rigid handle wafer before release and transfer.
- [Graded Stiffness Substrate](../concepts/graded-stiffness-substrate.md) — built by sequential spin-coating of PDMS layers of different mixing ratios and thicknesses.
- [Sputter Deposition on Elastomers](../methods/sputter-deposition-elastomers.md) — complementary deposition step (metal) on spin-coated elastomer substrates.

## Procedure (Naserifar et al. 2016)
The two-material gradient substrate was built by sequential spin-coating on handle wafers:
1. Spin-coat 10 µm PDMS (5:1) on a handle wafer.
2. Transfer the silicon chip onto this layer.
3. Spin-coat a second 60 µm PDMS (5:1) layer over the chip; cure at 80 °C for 4 h.
4. Etch the composite into a 1 mm-diameter circle; release from the handle wafer.
5. Transfer onto a second handle wafer pre-coated with 10 µm PDMS (20:1).
6. Spin-coat an additional 80 µm PDMS (20:1) to embed the intermediate structure; cure 4 h at 80 °C.

The result: a chip surrounded by a stiff intermediate PDMS (5:1) shell, embedded in a soft PDMS (20:1) primary substrate, with the soft material covering the intermediate structure by ~10 µm on top and bottom.

## Key Parameters
- **Spin speed / time**: Primary controls of film thickness (higher speed → thinner film).
- **Precursor viscosity**: For PDMS, set by mixing ratio and temperature; affects achievable thickness range.
- **Layer stacking**: Sequential spin-coat + cure cycles build multilayer structures with controlled per-layer thickness (here, 10–80 µm layers).

## Strengths
- Precise, repeatable control of film thickness over a wide range (sub-µm to tens of µm).
- Excellent uniformity over a wafer.
- Compatible with multilayer build-up and with handle-wafer transfer workflows.

## Limitations
- Limited to relatively flat substrates; topography degrades uniformity.
- Wafer-scale process; not directly a large-area/roll-to-roll method.
- Edge bead and radial thickness variation at wafer edges.

## Source Support
- [Naserifar et al. 2016 — Material Gradients in Stretchable Substrates](../source-notes/naserifar-2016-material-gradients.md)

## Open Questions
- Can sequential spin-coating produce a near-continuous stiffness gradient (many thin graded layers) rather than discrete steps?
- How does spin-coating translate to scalable, large-area manufacturing of graded substrates?

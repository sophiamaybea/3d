# 9 East 63rd — Adobe Substance-ready material specification

This document translates the Adobe concept board into practical physically based material targets for a future Substance 3D Painter/Designer pass. The live web build currently recreates the same direction procedurally in GLSL so it can run instantly in-browser.

## 1. Smoked walnut

- Base colour range: `#1D100B` → `#593322`
- Metallic: `0.00`
- Roughness target: `0.54`
- Normal: very fine open-pore structure, directional with grain
- Height: subtle, approximately 0.02–0.08 relative intensity
- Variation: broad low-frequency colour drift plus tight directional grain
- Avoid: orange varnish, glossy furniture-store finish, exaggerated procedural knots

## 2. Honed warm marble

- Base colour range: `#D5CFC7` with warm grey/taupe veins around `#86766D`
- Metallic: `0.00`
- Roughness target: `0.32`
- Normal/height: restrained, veins should read primarily through colour and micro-normal rather than deep displacement
- Reflectance: broad soft highlights rather than a polished mirror surface
- Avoid: high-contrast black spider-web veins, wet-looking gloss

## 3. Aged bronze

- Base colour: approximately `#826044`
- Metallic: `0.86–1.00`
- Roughness target: `0.36`
- Patina: sparse, low-saturation brown/green oxidation concentrated at edges and recessed detail
- Edge response: slightly smoother on handled/high-contact areas
- Avoid: bright gold, uniform copper, heavy theatrical verdigris

## 4. Warm mineral plaster

- Base colour range: `#BCB0A0` → `#EFE6D9`
- Metallic: `0.00`
- Roughness target: `0.90`
- Surface: extremely low-amplitude mineral variation, no obvious repeating noise
- Avoid: Venetian-plaster gloss or rustic stucco texture

## 5. Oxblood lacquer / textile accent

- Base colour: `#4C101A`
- Lacquer roughness: `0.22–0.30`
- Textile roughness: `0.85–0.92`
- Saturation should stay restrained in neutral light
- Use only as a punctuation colour, not a dominant surface

## Adobe concept board

https://firefly.adobe.com/boards/id/urn:aaid:sc:EU:cc985095-909a-478d-bdd0-241f512adce5

## Accuracy note

These are conceptual restoration materials. They are not claims about the townhouse's current finishes. A true Substance export pass should be applied after measured geometry and final architectural specifications are available.

# Spatial Property Walkthrough POC

Browser-native Gaussian-splat walkthrough prototype for turning authorised property listing media into a first-person spatial experience.

## Current prototype

- Three.js scene + Spark Gaussian Splat renderer
- Real `.spz` splat asset rendered in-browser
- Desktop pointer-lock + WASD movement
- Mobile movement/look controls
- Separate movement/collision envelope
- Query-string splat override: `?splat=https://.../property.spz`
- Debug floor shell: `?debug=1`

The default scene uses Spark's public demo `fireplace.spz`. It is **not** represented as the target property. The production workflow replaces it with a reconstruction generated from media the owner/agent is authorised to use.

## Production pipeline

1. Collect original listing photographs, 360 captures, floor plan, and dimensions from the owner/agent.
2. Solve camera poses with COLMAP, or VGGT-1B-Commercial for sparse/unposed images.
3. Train/export Gaussian splat with Nerfstudio Splatfacto/gsplat.
4. Clean splat in SuperSplat.
5. Convert/compress with `splat-transform` to SPZ/SOG/streamed SOG.
6. Generate a collision shell from the floor plan or `splat-transform --collision-mesh`.
7. Reconstruct key PBR materials in Adobe Substance Sampler/Painter where a clean architectural mesh is used.
8. Replace the demo `SPLAT_URL` and demo bounds with the property assets.

## Deployment

Static site. No build step required. Suitable for Vercel.

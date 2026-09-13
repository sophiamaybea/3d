# 9 East 63rd — Interactive Property Concept

A cinematic real-estate microsite and self-guided Three.js concept walkthrough for **9 E 63rd St, New York, NY 10065**.

## Design thesis

**Not a finished house. A finished address.**

The public listing describes a 25-foot-wide historic townhouse currently configured as mixed use, with two medical suites, a parlor-floor residence, a third/fourth-floor duplex, a fifth-floor apartment, and multiple rear terraces. Rather than misrepresent the property with a fabricated photogrammetry tour, this site turns those verified facts into a clearly labelled **conceptual spatial walkthrough**.

## Stack

- React 18 (browser ESM)
- Three.js
- custom GLSL procedural material shaders
- GSAP + ScrollTrigger
- pointer-lock first-person navigation (WASD + mouse)
- Adobe-generated concept material direction / Firefly Board
- semantic HTML + JSON-LD
- static deployment, no backend required

## Important accuracy note

The Three.js walk is an approximate concept model, **not a measured survey, Matterport reconstruction or depiction of existing finishes**. The spatial envelope is inferred from the listing's 25-foot width, 8,700 sq ft total area, and described floor programme. Current photography and authoritative facts remain on the source listing.

## Source listing

https://www.zillow.com/homedetails/9-E-63rd-St-New-York-NY-10065/447094218_zpid/

## Branch

The build lives on `e63-townhouse` so the repository's original `main` branch remains intact.

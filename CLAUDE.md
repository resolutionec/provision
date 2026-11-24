# Project notes for Claude

The Pro-Vision Optical website is a single `index.html` with hash routes, a Three.js (r160) hand-built 3D model of Model A03039, and Lenis smooth scroll. It deploys via GitHub Pages from `main`.

**Read `docs/3d-configurator-guide.md` before touching the 3D model, materials, viewer or motion.** It records every setting and the mobile-rendering lessons:
- no `transmission` for crystal acetate;
- keep inlays ≥ 0.09 mm proud;
- camera near 8 / far 1200;
- logarithmic depth buffer;
- polygonOffset on metal.

Conventions:
- Fonts: League Spartan (headings) and Courier Prime (text). Cream `#f4f0e8` background. Light mode only.
- Default colourway: Bone / Gold. Frame + Metal options only; the lens is fixed to grey.
- Don't trace or copy other brands' frame designs. Pro-Vision's own designs are fine.
- Verify visual changes by rendering in headless Chrome (desktop 1280 and mobile 390) before publishing. Check for horizontal overflow.
- After each change: commit, push to `origin main`, and republish the claude.ai preview artifact.

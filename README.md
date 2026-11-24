# Pro-Vision Optical — gallery website

A website for Pro-Vision Optical (OEM & ODM eyewear, Shenzhen), presented as an art gallery. It's built from the approved wireframe set 4a–4g.

## Pages (hash routes in a single `index.html`)
| Route | Page |
|---|---|
| `#home` | Entrance, with a live 3D Model A03039 and a colour configurator |
| `#room-acetate` · `#room-titanium` · `#room-metal` · `#room-accessory` | Collection rooms (Optical / Sun filters) |
| `#object-a03039` | Object page: annotated 3D study (hover or tap a callout to highlight that part), sample photographs, OEM/ODM enquiry |
| `#atelier` · `#process` · `#journal` · `#visit` | Supporting rooms. Visit builds an enquiry email to sales@provision-opt.com |

## 3D model
A03039 is modelled by hand in Three.js (r160, loaded from jsDelivr) from the three reference photos in `img/`. It isn't a scan. Its parts are named (brow bar, end-piece, temple, lens), so the callouts can highlight them.

Colourways: frame (Black, Havana, Smoke crystal, Bone) × metal (Palladium, Gold, Gunmetal); lens fixed to grey. Default is Bone / Gold.

Full configurator settings, export formats and rendering lessons: **[docs/3d-configurator-guide.md](docs/3d-configurator-guide.md)**.

If WebGL is unavailable, the stage falls back to the product photograph.

## Type & colour
League Spartan for headings, Courier Prime for text, and a warm cream gallery wall (`#f4f0e8`). Light mode only.

## Still to supply
- Product pages and photos for the other works (the placeholder cards read "Awaiting installation")
- Workshop photographs, the president's portrait, and the factory film
- Pro-Vision's own copy for Atelier and Process (the current text is a draft)

## Run locally
Open `index.html` through any static server, e.g. `npx serve .`.

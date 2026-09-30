# Product page images — Reeded glass static cling window film

Model: Nano Banana Pro (`nano_banana_pro`). Gallery images 1:1, banners 16:9.
Budget: 48 credits (2k = 2 cr, 4k = 4 cr) → 1 hero at 4k + 22 images at 2k.

## Method (Nano Banana Pro best practices)

- Narrative, specific description: subject → scene → composition → lens → light.
- Product described identically in every prompt (fixed PRODUCT block) and with its real
  physics: translucent not opaque, vertical ribs, shapes become vertical stripes,
  colors/light pass, no glue, static cling on wet glass. Nothing the film can't do.
- Two phases: phase 1 generates a macro of the film texture; phase 2 passes it as a
  reference image ("@image1 = film texture only, not the room") to lock rib width,
  finish and refraction across the whole gallery.
- No text, logos or watermarks in the images: the store sells in several EU languages,
  copy goes in the theme/overlay, not baked into the photo.
- Nora images use @image1–3 (her references) + @image4 (film texture).

**PRODUCT**

> The product is a reeded-glass-effect static cling window film: a thin (about 0.2 mm), flexible, clear PVC film with a frosted-clear finish whose surface is molded into evenly spaced, parallel vertical ribs roughly 1 cm wide. Applied to the inside of a flat clear glass pane with the ribs running vertically, it makes the glass look like real architectural reeded (fluted) glass. It is translucent, never opaque: daylight passes through almost fully, while everything behind the glass is broken into soft vertical stripes, so shapes and people become unrecognizable but colors and light stay visible. It has no glue and holds to the glass by static cling.

**STYLE**

> Photorealistic e-commerce photography for a product page, natural and credible, shot on a full-frame camera. True-to-life colors, physically accurate refraction through the ribs, clean composition with breathing room. No text, no logos, no watermarks, no brand names.

**TEXTURE REF (phase 2 prefix)**

> @image1 is a reference ONLY for the window film: match its rib width, spacing, clear-frosted finish and the way it refracts what is behind it. Do not copy its framing, background or objects.

## Shots

| #  | Shot                         | Ratio | Res | Variants |
| -- | ---------------------------- | ----- | --- | -------- |
| 01 | Macro texture (phase 1)      | 1:1   | 2k  | 1        |
| 02 | Hero bathroom window (ph. 1) | 1:1   | 4k  | 1        |
| 03 | Before / after split window  | 1:1   | 2k  | 2        |
| 04 | Thin & flexible sheet        | 1:1   | 2k  | 1        |
| 05 | Install 1 — spray water      | 1:1   | 2k  | 1        |
| 06 | Install 2 — squeegee         | 1:1   | 2k  | 1        |
| 07 | Install 3 — trim edge        | 1:1   | 2k  | 1        |
| 08 | Removable, no residue        | 1:1   | 2k  | 1        |
| 09 | Kitchen cabinet doors        | 1:1   | 2k  | 2        |
| 10 | Shower screen                | 1:1   | 2k  | 2        |
| 11 | Interior glass door          | 1:1   | 2k  | 1        |
| 12 | Street-facing window privacy | 1:1   | 2k  | 2        |
| 13 | Striped light on wall        | 1:1   | 2k  | 1        |
| 14 | Studio roll shot             | 1:1   | 2k  | 1        |
| 15 | Nora applying the film       | 1:1   | 2k  | 2        |
| 16 | Banner living room           | 16:9  | 2k  | 1        |
| 17 | Banner bathroom              | 16:9  | 2k  | 1        |

Final shot list with Higgsfield job IDs is in the matching `.json`; each prompt = [TEXTURE REF] + PRODUCT + scene + STYLE (Nora shots use her identity block from set 01).

## Caveat

Rib width (≈1 cm) and finish are assumed. When the supplier sample arrives, regenerate the
key shots with a photo of the real film as the reference so the page shows exactly what ships.

# UGC video #1 — reeded glass window film (30s, 9:16)

Built with the official Higgsfield `ugc-review-video` workflow (talking-head demo, no testimonial).

- Creator reference: `assets/creators/creator-blonde-01.png` → Higgsfield media `b53804b2-47ff-4505-bc89-04e3365857ea`
- Product reference (film texture): job `ff582d6b-6b98-4394-a740-db440ade1f69`
- Language: English (EU-wide), no product claims beyond what is shown on screen
- Structure: 2 boards × 15s — HOOK+SETUP, APPLY+CLOSER

## Script (verbatim)

1. "Window facing straight into the building across the street? Yeah, watch this. Spray the glass, peel the backing off, and lay the film on while it's still wet."
2. "Then one pass with the squeegee, middle out. Look — everything outside is just soft stripes now, and the daylight still pours right in. And this corner peels back up whenever you're done with it."

## Pipeline / job IDs

| Step | Model | Job |
| --- | --- | --- |
| Board 1 raw | gpt_image_2 21:9 | `01aea26d-581e-49a7-ba62-37493a51088c` |
| Board 1 de-slop | seedream_v5_pro | `bdef5952-8d14-4252-b6ce-07f1629adf9c` |
| Board 2 raw | gpt_image_2 21:9 | `2804404e-08bc-4c69-a6d3-9293313ac08b` |
| Board 2 de-slop | seedream_v5_pro | `22c98480-aaf7-428a-b531-22c3f17aa262` |
| Clip 1 (15s) | seedance_2_5 omni_reference + audio | `127328a8-ea79-4553-967a-a8b65e72ac95` |
| Clip 2 (15s) | seedance_2_5 omni_reference + audio | `d8988769-795c-4470-b1e0-0a81a7262ef3` |

Clip prompts: `clip1.txt`, `clip2.txt`.

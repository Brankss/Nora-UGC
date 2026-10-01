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

## Final cut — video #1

- Assembled 30.1s MP4 (hard-cut concat, stream copy): Higgsfield media `d222fe79-3fd9-47c6-ade0-4afc78ebf1fc`
  → https://d2ol7oe51mr4n9.cloudfront.net/user_38O4FsThNaTNGmKzYo6UK4OuQNn/d222fe79-3fd9-47c6-ade0-4afc78ebf1fc.mp4
- Audio check (Whisper): both clips match the script word for word.

# Variants for A/B hook testing (15s, 720p, single board FULL_ARC)

| Video | Hook | Board (de-slop) | Clip | Prompt |
| --- | --- | --- | --- | --- |
| #2 Neighbor POV | caught mid-toothbrush, neighbor's window 2 m away | `53ee29b8-d538-49bb-81af-89bf2c02cef0` | `9f3e3681-2418-4c88-92ca-6e7d81348d0d` | `v2-neighbor-clip.txt` |
| #3 ASMR | silent satisfying process, whispered lines | `a88c5cf3-c449-4649-b8d7-80b9a2b23f36` | `aaf5a584-6a4b-4582-ae09-1463e81b1fc2` | `v3-asmr-clip.txt` |

## QA results (frame contact sheets + Whisper transcripts)

| Video | Status | Notes |
| --- | --- | --- |
| #1 (30s, 1080p) | ✅ ready | Identity consistent, script verbatim. Minor: tank top shifts grey→black and lips a bit redder in clip 2; first cut of clip 2 shows glass still clear while squeegeeing. |
| #2 Neighbor POV (15s, 720p) | ⚠️ blocked | Seedance rendered the voice in **Chinese** despite the English script. Fix = Higgsfield `dubbing` to `eng` on job `9f3e3681-2418-4c88-92ca-6e7d81348d0d` (failed: out of credits). |
| #3 ASMR (15s, 720p) | ✅ ready | English whisper verbatim, strong macro beats, consistent identity. |

Final URLs:
- #1 → https://d2ol7oe51mr4n9.cloudfront.net/user_38O4FsThNaTNGmKzYo6UK4OuQNn/d222fe79-3fd9-47c6-ade0-4afc78ebf1fc.mp4
- #3 → https://d8j0ntlcm91z4.cloudfront.net/user_38O4FsThNaTNGmKzYo6UK4OuQNn/hf_20261001_011239_aaf5a584-6a4b-4582-ae09-1463e81b1fc2.mp4

Lesson: for Seedance 2.5 add an explicit language line to the Audio block ("spoken in English, American accent") — the script alone did not lock the language on clip #2.

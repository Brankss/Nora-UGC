# Nora — Soul ID reference set (v1)

Goal: 20 reference images to train Nora's character (Soul ID) on Higgsfield.
3 original references + 17 generated with the prompts below.

## Generation settings

| Setting        | Value                                   |
| -------------- | --------------------------------------- |
| Model          | Nano Banana Pro (`nano_banana_pro`)     |
| Resolution     | 2k                                      |
| Aspect ratio   | 3:4                                     |
| Batch size     | 1 per prompt                            |
| References     | Nora ref 1, 2, 3 (`image_references`)   |
| Higgsfield     | project "Nora UGC"                      |

## Prompting rules used (from research)

- On Higgsfield, point to the references with `@image1`, `@image2`, `@image3` (in the
  order they are attached), say they show the same person and lock identity explicitly
  ("keep her identity 100% identical to @image1, @image2 and @image3").
- Use the exact same identity block in every prompt. Re-describing the face in
  different words, or words like "new"/"different", invites identity drift.
- Write in natural descriptive sentences (subject, action, setting, composition,
  lighting, camera), not keyword lists.
- Fight the "AI-perfect" look: unretouched smartphone photo, real skin texture,
  no beauty filter, not a studio/ad shot.
- Soul ID training wants variety: angles (front, 3/4 L/R, profiles, high/low),
  distance (headshot → full body), expressions (neutral, smile, laugh, talking),
  lighting (soft/harsh, indoor/outdoor, flash), outfits and backgrounds.
  Always one person, sharp face, eyes visible, no sunglasses/hats, no heavy makeup.

## Prompt structure

`prompt = IDENTITY + " " + SCENE + " " + REALISM`

**IDENTITY**

> @image1, @image2 and @image3 are reference photos of the same young woman, Nora. Show exactly this woman in the scene below and keep her identity 100% identical to @image1, @image2 and @image3: same face shape and bone structure, same thick dark eyebrows, same brown eyes, same nose, lips and jawline, same warm olive skin tone with her natural freckles and small beauty marks, same long dark-brown wavy hair. Do not beautify, slim or alter her features. She is the only person in the photo.

**REALISM**

> Photorealistic, unretouched smartphone photo: real skin texture with visible pores, fine peach fuzz and a natural dewy glow, no airbrushing, no beauty filter, no plastic skin. Minimal everyday makeup like in @image1, @image2 and @image3 (brushed-up brows, mascara, sheer pink lips). Her face is sharp and in focus, never covered by hands, hair or objects: no sunglasses, no hat. No text, no watermark, not a studio or advertising shot.

## Coverage map

| #  | Framing          | Angle            | Expression        | Light                     |
| -- | ---------------- | ---------------- | ----------------- | ------------------------- |
| 01 | headshot         | front            | neutral           | soft window               |
| 02 | head & shoulders | 3/4 left         | soft smile        | soft side window          |
| 03 | head & shoulders | 3/4 right        | relaxed           | soft morning              |
| 04 | close-up         | left profile     | neutral           | soft window               |
| 05 | head & shoulders | right profile    | slight smile      | golden hour outdoor       |
| 06 | waist-up selfie  | front, high      | laughing (teeth)  | golden hour backlight     |
| 07 | waist-up selfie  | front            | talking           | daylight in car           |
| 08 | waist-up         | 3/4, off-camera  | sleepy smile      | morning window            |
| 09 | half body mirror | front            | confident smile   | bathroom vanity           |
| 10 | full body mirror | front            | slight smile      | afternoon daylight        |
| 11 | full body        | front, walking   | soft smile        | overcast street           |
| 12 | head & shoulders | front            | relaxed           | harsh midday sun          |
| 13 | close-up selfie  | front, high      | big smile         | night phone flash         |
| 14 | full body seated | high angle       | calm              | warm lamp, evening        |
| 15 | waist-up         | low angle        | small smile       | bright studio daylight    |
| 16 | waist-up selfie  | front            | excited           | side window               |
| 17 | waist-up         | 3/4              | calm small smile  | overcast café window      |

## Scenes

### 01 — Front headshot, neutral
Scene: close-up headshot, straight-on front view at eye level, head and top of shoulders in frame. She looks directly into the lens with a calm, neutral expression, lips closed and relaxed. Hair down, tucked behind both ears so her full face and hairline are visible. She wears a plain white crew-neck t-shirt. Background: a plain off-white wall at home. Soft, even daylight from a large window in front of her, no harsh shadows. Shot by a friend on an iPhone rear camera at 2x zoom, vertical 3:4 framing.

### 02 — Three-quarter left, soft smile
Scene: head-and-shoulders portrait, her head turned about 45 degrees to her left (three-quarter view), eyes looking back at the lens, soft closed-mouth smile. Hair down over one shoulder. She wears a black fitted crew-neck t-shirt. Background: a plain light-grey wall. Soft diffused window daylight from the side, gentle natural shadow on the far cheek. Shot on an iPhone rear camera at 2x, vertical 3:4 framing.

### 03 — Three-quarter right, relaxed
Scene: head-and-shoulders portrait, her head turned about 45 degrees to her right (three-quarter view), chin slightly down, eyes to the lens, relaxed neutral expression with the hint of a smile. Hair down, falling in front of one shoulder. She wears a heather-grey hoodie. Background: a plain white bedroom wall with the blurred corner of a white wardrobe. Soft morning window light. Shot on an iPhone rear camera at 2x, vertical 3:4 framing.

### 04 — Left profile close-up
Scene: close-up of her full side profile facing left, head perfectly in profile so her forehead, nose, lips, chin and jawline form a clean silhouette. Neutral expression, looking straight ahead, not at the camera. Hair tucked behind her ear, showing her ear with a small gold hoop earring. She wears a cream ribbed knit top. Background: a plain warm-white wall. Soft window daylight falling on her face. Shot on an iPhone rear camera at 2x, vertical 3:4 framing.

### 05 — Right profile, golden hour street
Scene: head-and-shoulders shot of her right side profile, facing right, gazing into the distance with a slight relaxed smile. Hair down, a few strands moving in a light breeze. She wears a white linen shirt. Location: a quiet European city street at golden hour, warm low sun lighting her profile, background softly out of focus with old buildings. Shot on an iPhone rear camera at 1x, vertical 3:4 framing.

### 06 — Laughing selfie, park at golden hour
Scene: front-camera selfie at arm's length, slightly above eye level, waist-up. She is laughing genuinely with an open mouth showing her teeth, eyes crinkled, looking into the lens. Hair down and a bit messy from the wind. She wears a white t-shirt under an oversized light-wash denim jacket. Location: a city park on a warm evening, grass and trees blurred behind her, golden-hour backlight creating a warm rim on her hair and soft light on her face. iPhone front camera look, vertical 3:4 framing.

### 07 — Talking to camera in the car (UGC talking head)
Scene: front-camera selfie frame, like a paused TikTok talking-head video. She sits in the driver's seat of a parked car with the seatbelt on, filming herself at arm's length at eye level. She is mid-sentence, mouth slightly open while talking, eyebrows raised, one hand gesturing near her chest, looking straight into the lens. Hair down. She wears a black zip-up hoodie. Bright natural daylight through the windshield lights her face evenly, car interior and headrest visible behind her. iPhone front camera look, vertical 3:4 framing.

### 08 — Kitchen morning, claw clip
Scene: waist-up candid photo in her kitchen in the morning. She leans against the counter holding a ceramic coffee mug with both hands at chest height, looking slightly off-camera with a soft sleepy smile. Hair pulled up loosely in a tortoiseshell claw clip with a few loose face-framing strands. She wears an oversized light-blue striped button-up shirt. Background: white cabinets, a window and a few plants, softly blurred. Bright soft morning daylight from the window beside her. Shot by a friend on an iPhone rear camera at 1x, vertical 3:4 framing.

### 09 — Bathroom mirror selfie, half body
Scene: bathroom mirror selfie, half body from the hips up. She holds her iPhone low at chest height with one hand so her entire face is clearly visible in the mirror, looking at her reflection with a small confident smile. Hair down. She wears a white ribbed tank top and grey sweatpants. Bathroom: white tiles, a sink with a few skincare bottles, warm overhead vanity light mixed with a little daylight, mirror with faint water spots. Vertical 3:4 framing.

### 10 — Full-body bedroom mirror selfie
Scene: full-body mirror selfie in her bedroom, head to toe visible in a tall standing mirror. She holds the iPhone at chest level off to the side so her face is not covered, weight on one leg in a relaxed natural pose, slight smile, looking at the mirror. Outfit: black fitted baby tee, straight-leg mid-wash jeans, white sneakers. Hair down. Bedroom: white wardrobe doors, a bed with light linen, dark wood floor, a bit lived-in. Soft afternoon daylight from a window. Vertical 3:4 framing.

### 11 — Full body, walking in the city
Scene: full-body photo taken by a friend from a few meters away, head to toe in frame. She walks toward the camera on a cobblestone sidewalk in an Italian city, mid-step, looking at the lens with a natural soft smile. Outfit: beige trench coat open over a white t-shirt, dark straight jeans, black loafers, small black shoulder bag. Hair down, moving slightly. Overcast daytime, soft even light, muted colors, shop fronts and parked scooters slightly blurred behind her. Shot on an iPhone rear camera at 1x, vertical 3:4 framing.

### 12 — Harsh midday sun, seaside
Scene: head-and-shoulders photo at the seaside at midday. Strong direct sunlight from above and to the side creates crisp, defined shadows under her nose and chin and bright highlights on her cheekbones; her eyes are open and clearly visible. Relaxed expression, lips closed, looking at the lens. Hair down, a little windswept. She wears a simple black tank top and a thin gold necklace. Background: blue sea and bright sky, slightly overexposed. Shot on an iPhone rear camera at 1x, vertical 3:4 framing.

### 13 — Night selfie with phone flash
Scene: close-up selfie at night with the phone's direct flash on, face and shoulders in frame, slightly above eye level. She smiles widely showing her teeth, looking into the lens. The hard flash gives bright specular highlights on her forehead, nose and cheeks and a quick falloff into a dark background, typical of a flash photo. Hair down. She wears a black square-neck top and small gold hoop earrings. Background: a dimly lit bar with warm blurred string lights. Slight grain, vertical 3:4 framing.

### 14 — Full body on the sofa, high angle, evening
Scene: full-body photo taken from slightly above by a friend standing in front of the sofa (high angle). She sits cross-legged on a beige sofa, her whole body visible, looking up at the camera with a calm, soft expression. Outfit: chunky cream knit sweater and grey lounge pants, bare feet. Hair down. Cozy living room in the evening, lit by a warm table lamp beside her and a dim ceiling light, warm tones, a throw blanket and a mug on the side table. Slight low-light grain. Shot on an iPhone rear camera at 1x, vertical 3:4 framing.

### 15 — Pilates studio, low angle, ponytail
Scene: waist-up photo taken from a slightly low angle, camera below her chin level looking up at her. She stands in a bright pilates studio after class holding a water bottle, cheeks slightly flushed, a small natural smile, looking at the lens. Hair in a sleek high ponytail, face fully visible. She wears a matching sage-green sports top and high-waist leggings with a light zip-up jacket open over it. Background: reformer machines and large windows, bright white daylight. Shot on an iPhone rear camera at 1x, vertical 3:4 framing.

### 16 — Excited product-review selfie
Scene: front-camera selfie at her desk, waist-up, like a frame from a TikTok product review. She holds up a small plain white unbranded skincare jar next to her face without covering it, eyebrows raised and mouth open in an excited "oh my god" expression, looking straight into the lens. Hair down, tucked behind one ear. She wears a soft lilac crewneck sweatshirt. Background: her bedroom desk with a laptop, a small plant and a lamp, softly blurred. Soft natural daylight from a window to her side. iPhone front camera look, vertical 3:4 framing.

### 17 — Café window, three-quarter
Scene: candid waist-up photo taken by a friend across the table in a café. She sits by the window in three-quarter view with an open paperback book in her hands and glances up from it toward the lens with a calm, small smile. Hair down. She wears a black fine-knit turtleneck. Soft overcast daylight from the big window lights the side of her face, café interior blurred behind her, a cappuccino on the wooden table. Shot on an iPhone rear camera at 2x, vertical 3:4 framing.

# Sovereign Lens

> Modular 5-layer system for AI photo generation — documentary realism to luxury commercial.
> Combine one option from each layer to build a complete, precise prompt.
>
> by **Logue** · [@AlexZio00](https://x.com/AlexZio00)

---

## Overview

Sovereign Lens is a structured prompt architecture for AI image generation (Midjourney, DALL-E, Stable Diffusion, Flux, etc.). Instead of writing prompts from scratch, you select one option from each of five layers — base style, camera type, subject type, scene preset, and fine-tuning options — and stack them into a single coherent prompt.

The system draws a hard line between two modes: **documentary/film** (capturing reality as found) and **commercial/advertising** (constructed perfection for sale). Every layer reflects this distinction. Mixing the two produces incoherent results; staying on one side produces images with a consistent, professional look.

Layer 5 options are optional fine-tuning. Layers 1–4 are the core stack.

---

## Layer 1 — Universal Base

Always include one of the two bases. This is the foundation that defines the overall image philosophy.

### Base A — Documentary / Film

> Use when the goal is to record, archive, or capture.

Generate as a real photograph. Exclude: CGI, game-engine rendering, excessive HDR, oversaturated color grading, artificial symmetry, travel-brochure aesthetics, plastic textures, heavy sharpening, and fake cinematic over-grading.

The scene should feel like a well-timed candid shot by a real photographer — not a directed set piece. Light comes from real sources. Material texture, atmospheric depth, spatial distance, and shadow behavior are all physically plausible. Leave in micro-imperfections, natural noise, lens character, and the limits of exposure.

**Decision rule: if the image is meant to record something → Base A.**

---

### Base B — Advertising / Commercial

> Use when the goal is to sell, promote, or brand.

Generate as a high-end commercial photograph. Precise lighting, clean surface rendering, sharp detail, ordered composition, sophisticated and refined color palette, brand-campaign feel. Represent as a fully polished, directed image.

Exclude: grain, documentary feel, candid or accidental framing, soft imperfections, archival or faded tones, rough texture.

**Decision rule: if the image is meant to sell something → Base B.**

---

## Layer 2 — Camera Type

Select the optical character of the image. This controls focal length, depth of field, rendering signature, and grain/noise behavior.

| Code | Description |
|------|-------------|
| **C1** | 35mm analog film — Fujifilm Classic Negative style. Strong grain, soft contrast, subtle halation, slightly faded highlights, gentle shadow rolloff. Restrained color palette. |
| **C2** | 35mm analog film — Kodak Portra 400 style. Soft warm skin tones, creamy highlights, mild grain. Especially strong for portraits. |
| **C3** | 35mm black and white film. High contrast, deep blacks, bright whites, defined grain. Ilford HP5 or Kodak Tri-X 400 feel. |
| **C4** | Canon RF 35mm f/1.8 — digital rendering. Realistic lens character, moderate depth of field, subtle sensor noise. |
| **C5** | Sony FE 85mm f/1.4 GM — portrait rendering. Creamy bokeh, shallow depth of field, full subject-background separation. |
| **C6** | Wide-angle 16–35mm — landscape/architecture. Wide field of view, deep depth of field, emphasizes scale of environments and structures. |
| **C7** | Studio commercial/fashion. Professional three-point lighting, clean specular reflections, premium brand-campaign mood. |

---

## Layer 3 — Subject Type

Select the subject category and the intended treatment. This governs how the subject is lit, styled, and post-processed.

| Code | Description |
|------|-------------|
| **S1** | Street portrait / candid — natural snapshots, unposed expressions, ambient light. No fashion-editorial or beauty retouching. |
| **S2** | Portrait / editorial — catchlights, preserved skin texture, Rembrandt lighting or natural window light. |
| **S3** | Fashion / advertising portrait — high-end editorial, luxury brand campaign aesthetic. |
| **S4** | Landscape / architectural documentary — atmosphere and the trace of time in the space. No tourism-brochure framing. |
| **S5** | Landscape / architectural premium — luxury hotel or real estate brochure style. Refined and aspirational. |
| **S6** | Aerial / elevated viewpoint — realistic altitude and scale. No drone-fantasy exaggeration. |
| **S7** | Product / luxury — studio lighting, premium brand environment. |
| **S8** | Product / lifestyle — natural light, everyday background, lived-in environment. |

---

## Layer 4 — Scene Presets

Select a scene context. Each preset packages a specific time of day, location type, lighting condition, and mood. These are ready-made environments — plug in a subject and shoot.

| Code | Scene | Core Details |
|------|-------|--------------|
| **P1** | Korean palace / hanok — night | Traditional architecture at night, gentle ambient lighting, quiet night air. 4200K–4800K color temperature. |
| **P2** | Palace night event | Torchlight and lanterns, historical palace atmosphere, documentary event photography feel. |
| **P3** | Urban night snap | Mixed streetlight and tungsten sources, wet asphalt, neon and signage light. f/1.8–f/2.8, ISO 800–1600. |
| **P4** | Railroad crossing — motion | Night-time crossing with warning lights, motion-blurred train. Foreground sharp; train only in blur. |
| **P5** | Vehicle light trails | Long-exposure night, flowing vehicle light streaks. No exaggerated or stylized light effects. |
| **P6** | Rainy day | Wet pavement, puddle reflections, overcast sky. Cold grey ambient feel. |
| **P7** | Dawn / early morning still | Pre-dawn, fog, cold and clear air. No saturated color palette. |
| **P8** | Golden hour / sunset | Backlit golden hour, long extended shadows. No excessive orange or pink color grading. |
| **P9** | Vintage travel documentary | Strong grain, faded color palette, archival mood. |
| **P10** | Korean hanok alley — evening | Depth of narrow alley, wood and stone texture, nostalgic atmosphere. |
| **P11** | Multiple exposure | Two subjects layered semi-transparently, analog film texture. No Photoshop-style compositing look. |
| **P12** | Black and white mood | Strong chiaroscuro contrast, film noir or documentary black and white. |

---

## Layer 5 — Options (Fine-Tuning)

Add any combination of these at the end of your prompt. All are optional. Use only what serves the specific image.

### Composition
- Rule of thirds
- Leading lines
- Frame within frame
- Negative space dominant
- Centered symmetry (use sparingly with Base A)
- Dutch angle
- Bird's eye view / worm's eye view

### Light
- Hard directional light, single source
- Soft diffused light, overcast
- Backlit / contre-jour
- Side light, raking across texture
- Practical sources only (lamps, candles, screens)
- Available light, no fill
- Mixed color temperature sources

### Texture & Detail
- Emphasize surface material texture
- Fine grain visible at full resolution
- Lens vignette, natural falloff
- Subtle chromatic aberration
- Slight front or rear focus shift
- Natural flare from practical light source

### Exclusion Guards
- No artificial skin smoothing
- No AI-typical symmetry artifacts
- No fantasy color grading
- No lens flare added artificially
- No stylized vignette overlay
- No text or watermarks in frame

### Subject Modifiers (portraits)
- Eyes sharp, background soft
- Both eyes in focus
- Profile angle
- Three-quarter turn
- Expression: neutral / candid / contemplative
- Looking off-frame

---

## Quick Reference Tables

### Style Selector

| Goal | Base | Camera | Notes |
|------|------|--------|-------|
| Street / candid documentary | A | C1, C2, C3, C4 | Avoid C7 |
| Editorial portrait | A or B | C2, C5 | B for fashion, A for editorial |
| Luxury product / brand | B | C7 | Always Base B |
| Landscape / architecture | A | C6 | Base B for real estate |
| Aerial photography | A or B | C6 | No drone-fantasy |
| Black and white film | A | C3 | P12 for strong mood |
| Night street photography | A | C4 | P3 or P4 |

### Camera Guide

| Focal Length | Best Use | Code |
|--------------|----------|------|
| 16–35mm wide | Landscape, architecture, environment | C6 |
| 35mm | Street, documentary, travel | C1, C4 |
| 85mm | Portraits, shallow focus | C5 |
| Studio | Commercial, fashion, product | C7 |
| Film (multi) | Analog look, grain, color shift | C1, C2, C3 |

### Scene × Subject Matrix

| | S1 Candid | S2 Portrait | S3 Fashion | S4 Landscape | S5 Premium | S7 Product |
|---|---|---|---|---|---|---|
| **P1 Palace night** | A-C1 | A-C2 | - | A-C6 | B-C6 | - |
| **P3 Urban night** | A-C4 | A-C5 | B-C7 | - | - | - |
| **P8 Golden hour** | A-C1 | A-C2 | B-C5 | A-C6 | B-C6 | - |
| **P7 Dawn still** | A-C1 | - | - | A-C6 | - | - |
| **P9 Vintage travel** | A-C1 | A-C2 | - | A-C6 | - | - |

---

## Combination Examples

These are the eight reference combinations from the original system, translated and formatted as prompt stacks.

---

**1. Korean palace night event**

> Base A + C1 + S4 + P2

Gyeongbokgung Palace at night. Torchlight and paper lanterns illuminate the courtyard. Visitors in traditional dress move through the scene — some blurred, some still. Documentary film quality, Fujifilm Classic Negative, 35mm grain, 4500K warm-cold mixed ambient. No tourism framing. Feels like archival coverage of an actual historical event.

---

**2. Urban night portrait — street candid**

> Base A + C4 + S1 + P3

A figure pauses under a streetlight on wet pavement at night. Neon and tungsten signage in the background. Canon RF 35mm f/1.8 rendering. Natural depth of field, ISO 1200 noise visible. Expression unstaged. No retouching, no artificial fill.

---

**3. Palace aerial view**

> Base A + C6 + S6 + P1

Gyeongbokgung from altitude — traditional tiled rooflines spread below, the palace compound bounded by the city. Night ambient from cultural lighting, 4400K. Wide-angle 16mm rendering, deep depth of field, realistic altitude scale. No idealized drone color grade.

---

**4. Golden hour portrait — backlit editorial**

> Base A + C2 + S2 + P8

Subject in natural backlight during golden hour. Long shadows extend forward. Kodak Portra 400 rendering — warm skin tones, creamy highlight rolloff. Catchlights from the sun. Skin texture preserved. No beauty retouching. Slightly underexposed shadow side, natural.

---

**5. Rainy night railroad crossing**

> Base A + C3 + S4 + P4 + P6

Night railroad crossing in rain. Warning lights active. Train passing — motion blur on the train only, crossing gate and foreground wet pavement sharp. Black and white, Ilford HP5 grain, high contrast. Cold wet air. Puddle reflections in foreground.

---

**6. Vintage perfume product advertisement**

> Base B + C2 + S7 + P9

Perfume bottle shot with vintage travel documentary color treatment. Faded warm tones, soft grain overlay, archival color palette. Studio product lighting underneath — bottle detail remains sharp and premium. Luxury brand feel inside a nostalgic, worn aesthetic. No harsh digital clarity.

---

**7. Multiple exposure — palace and pine tree**

> Base A + C1 + S4 + P11

Gyeongbokgung palace roofline and a pine tree double-exposed on a single frame. Semi-transparent layering, analog film quality. Both subjects legible but blended. Natural grain throughout. Not a digital composite — feels like an in-camera or darkroom technique.

---

**8. Black and white market portrait**

> Base A + C3 + S1 + P12

Elderly vendor at a traditional market. Strong chiaroscuro contrast, deep blacks, bright reflected highlights on product surfaces. Ilford HP5 or Tri-X 400 grain character. Expression candid — mid-motion or glancing away. High contrast shadows cut across the face and hands.

---

## Limitations

**What this system does not control:**

- AI model capabilities vary. The same prompt stack produces different results across Midjourney, DALL-E, Flux, and Stable Diffusion — treat output as directional, not deterministic.
- "Exclude X" instructions are probabilistic, not guaranteed. AI models may still generate excluded elements. Rerun or add stronger exclusion language if needed.
- Scene presets assume the model has sufficient training data on each environment (e.g., Korean palace architecture). For less common subjects, add supplementary description.
- Layer 5 options can conflict — for example, "hard directional light" and "soft diffused light" should not appear together. Read your own stack before submitting.

**What Base A / Base B do not mean:**

- Base A is not "lo-fi" and Base B is not "sharp." Both can be technically excellent images. The difference is intent and aesthetic philosophy, not resolution or quality.
- Do not mix A and B in the same prompt. The two philosophies conflict at the foundational level and produce inconsistent results.

**Layer 4 is not location-specific:**

Scene presets describe atmosphere and lighting conditions, not a named location. P1 is "Korean palace night atmosphere" — it does not lock you to Gyeongbokgung. The preset applies to any traditional Korean architectural space at night.

---

## How to Build a Prompt

1. Choose Base A or Base B (never both)
2. Choose one camera code (C1–C7)
3. Choose one subject code (S1–S8)
4. Choose one or two scene presets (P1–P12) if applicable
5. Append any Layer 5 options that serve the image
6. Write a one-sentence scene description at the start

**Template:**

```
[Scene description in one sentence.]
[Base A or Base B text block]
[Camera code description]
[Subject code description]
[Scene preset description]
[Layer 5 options if any]
```

For best results, paste the relevant full text of each layer rather than just the codes. AI models respond to descriptive language, not shorthand labels.

---

## Output Language

This prompt system is written in English. The AI model will respond in the language of the final prompt you submit.

To generate prompts in a specific language, write your scene description in that language. The layer descriptions can remain in English — most image-generation models handle mixed-language prompts correctly, and English technical photography terms (grain, bokeh, ISO, f-stop, etc.) are universally recognized.

Add `Output image description in Korean.` or similar at the end if you need the model to explain its output in a specific language.

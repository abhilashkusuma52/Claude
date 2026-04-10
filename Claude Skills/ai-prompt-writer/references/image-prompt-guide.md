# Image Generation Prompt Guide

## Anatomy of a Great Image Prompt

```
[Subject] [doing/being what] + [Setting/Environment] + [Art Style] + [Medium] +
[Lighting] + [Color Palette] + [Mood/Atmosphere] + [Composition/Camera] + [Quality tags]
```

---

## Midjourney

### Basic Structure
```
/imagine [subject], [style], [medium], [lighting], [color palette], [mood], --ar [ratio] --v 6
```

### Key Parameters
| Parameter | Values | Purpose |
|---|---|---|
| `--ar` | 16:9, 4:3, 1:1, 9:16 | Aspect ratio |
| `--v` | 5, 6, 6.1 | Model version (use 6 for latest) |
| `--style` | raw, scenic | raw = photorealistic |
| `--q` | 0.5, 1, 2 | Quality (rendering time) |
| `--s` | 0–1000 | Stylization strength |
| `--no` | unwanted elements | Negative prompt |
| `--chaos` | 0–100 | Variation between results |
| `--seed` | any number | Reproducibility |

### Example Prompts

**Portrait (Photorealistic):**
```
A 35-year-old South Asian woman with warm brown eyes, wearing a deep teal silk saree,
standing in a sunlit traditional courtyard, golden hour lighting, soft bokeh background,
Canon 85mm portrait lens, editorial fashion photography, ultra-detailed skin texture,
--ar 4:5 --style raw --v 6
```

**Product Photography:**
```
Luxury perfume bottle on a black marble surface, dramatic studio lighting with a single
spotlight, deep shadows, gold and black color palette, commercial product photography,
ultra sharp focus, 8K resolution --ar 1:1 --style raw --v 6
```

**Landscape / Art:**
```
Ancient Indian temple at dusk, rice fields reflecting orange sky, mist rising from water,
impressionist painting style, painterly brushstrokes, warm earth tones, cinematic wide shot
--ar 16:9 --v 6
```

**Logo / Graphic:**
```
Minimalist logo design for a luxury clothing brand called "Elegance", gold foil on black,
Art Deco style, geometric symmetry, premium feel, vector art style, isolated on white
--ar 1:1 --v 6 --no shadows, texture, gradients
```

---

## DALL·E 3 (ChatGPT / API)

### Key Differences from Midjourney
- No parameter syntax — write in natural language
- Describe mood, atmosphere, and intent explicitly
- Cannot use celebrity names — describe appearance instead
- Handles complex scene composition well
- Strong at text in images (logos, signs, labels)

### Structure
```
[Style declaration] of [subject + action] in [setting]. The image has [lighting description].
[Color palette]. [Mood/atmosphere]. [Camera or composition notes if relevant].
```

### Example Prompts

**Photorealistic Portrait:**
```
A photorealistic photograph of an elegantly dressed South Asian woman in her 30s wearing
a deep teal silk saree with gold embroidery, standing in a sunlit marble corridor. The
lighting is warm golden hour. The background is softly blurred. Shot with a portrait lens,
editorial fashion magazine style.
```

**Brand/Marketing Image:**
```
A luxury product advertisement image showing premium fabric swatches — silk, velvet, and
chiffon — arranged artfully on a pure white surface with gold jewelry accents. Overhead
flat-lay photography. Warm, aspirational mood. Ultra-clean and minimal composition.
Professional commercial photography style.
```

**Illustration:**
```
A detailed digital illustration of a traditional Indian marketplace at festival time.
Colorful lanterns hang overhead. Vendors display silks, spices, and jewelry. People in
traditional clothing walk through. Warm and vibrant colors. Style: detailed watercolor
illustration with slight impressionist influence.
```

---

## Stable Diffusion

### Structure
```
Positive prompt: [subject], [style tags], [quality tags]
Negative prompt: [things to exclude]
```

### Quality Tags (Positive)
```
masterpiece, best quality, ultra-detailed, sharp focus, 8k resolution, photorealistic,
professional photography, studio quality, highly detailed
```

### Common Negative Prompt
```
lowres, bad anatomy, bad hands, extra fingers, missing fingers, blurry, pixelated,
watermark, text, logo, ugly, deformed, out of frame, cropped, worst quality
```

### Weighting Syntax
- Increase weight: `(term:1.4)` — boosts that element
- Decrease weight: `(term:0.7)` — reduces that element
- Group: `(term1 term2:1.2)`

### Example

**Portrait:**
```
Positive: (masterpiece:1.4), (best quality:1.2), photorealistic, 1woman, South Asian,
elegant saree, teal silk, golden embroidery, soft studio lighting, bokeh background,
editorial fashion photography, ultra-detailed skin, sharp eyes

Negative: (lowres:1.3), bad anatomy, extra fingers, blurry, watermark, text, ugly,
deformed, bad proportions, out of frame
```

---

## Universal Image Prompt Tips

### Lighting Options
- `golden hour lighting` — warm, soft, magical
- `dramatic studio lighting` — bold contrast, shadows
- `soft natural window light` — gentle, lifestyle feel
- `cinematic lighting` — film look, high contrast
- `overcast diffused light` — even, flat, fashion
- `backlit / rim lighting` — subject silhouetted, glowing edges
- `neon lighting` — vibrant, urban night scene

### Art Style Options
- `photorealistic` / `hyperrealistic`
- `oil painting` / `impressionist oil painting`
- `watercolor illustration`
- `digital art` / `concept art`
- `editorial fashion photography`
- `anime` / `Studio Ghibli style`
- `Art Deco` / `Art Nouveau`
- `minimalist flat design`
- `3D render` / `CGI`
- `pencil sketch` / `charcoal drawing`

### Camera / Composition Terms
- `close-up portrait` / `medium shot` / `full-body shot`
- `overhead flat-lay` / `bird's eye view`
- `low angle shot` / `worm's eye view`
- `wide angle` / `telephoto`
- `rule of thirds composition`
- `symmetrical composition`
- `bokeh background` / `shallow depth of field`
- `85mm lens` / `50mm lens` / `wide angle 24mm`

### Color Palette Terms
- `warm earth tones` — browns, oranges, creams
- `cool monochromatic` — grays, blues, silvers
- `jewel tones` — deep emerald, sapphire, ruby
- `pastel palette` — soft, muted, light
- `black and gold` — luxury, premium
- `vibrant saturated colors` — bold, energetic
- `muted desaturated` — moody, editorial

---

## Brand / Saree Photography (Kusuma's Elegance Reference)

For consistent brand photography prompts:

```
Full-length editorial fashion photograph of a [DESCRIPTION] woman wearing [SAREE DESCRIPTION],
standing against a pure beige background, white marble flooring, soft even studio lighting,
full-body framing from head to toe including footwear, sharp focus throughout, luxury fashion
photography style, no shadows on background, clean and minimal composition --ar 4:5 --style raw --v 6
```

Always include: beige background, white flooring, full-length framing, soft even lighting.

# Single-Culture Prompting

## Goal

Help users and systems generate prompts that produce outputs grounded in a specific cultural tradition, avoiding generic flattening, neighboring-culture confusion, and fantasy drift.

---

## Prompt construction logic

A good single-culture prompt specifies:

1. **Culture or tradition** — the specific tradition, not a broad geographic label
2. **Motif family** — the type of motif (geometric, floral, faunal, figural, border, etc.)
3. **Material context** — what medium the motif appears in (carved stone, painted ceramic, silk textile, manuscript, etc.)
4. **Compositional behavior** — how the motif is arranged (border, field, central emblem, register, panel)
5. **Period or style context** — when relevant, to avoid anachronism or fantasy drift

Optional but useful:
6. **Exclusion language** — what to leave out (no fantasy elements, no neighboring-culture blending, no glowing effects)
7. **Surface quality** — matte, glossy, weathered, polished, pigmented

---

## What to specify explicitly

| Element | Why it matters |
|---|---|
| Culture or tradition | Prevents generic "world ornament" output |
| Motif family | Anchors the visual content |
| Material | Shapes the surface, color, and texture |
| Composition | Controls layout and structure |
| Period | Prevents anachronism |
| Exclusions | Blocks common drift patterns |

---

## What to avoid

- **"Inspired by"** — this is a license to drift. Prefer direct reference: "in the style of Iznik ceramic painting" over "inspired by Islamic art"
- **Broad geographic labels** — "Asian pattern," "African design," "Middle Eastern art" — these are too wide to produce anything specific
- **Vague aesthetic terms** — "ornate," "elegant," "mystical," "ancient" — these do not describe visual form
- **Mood words as primary descriptors** — "serene," "powerful," "spiritual" — these are emotional, not formal
- **Assuming the model knows what you mean** — it does not. Specify material, composition, and motif family every time

---

## Example prompt fragments

### Egyptian
- `carved limestone relief in the style of New Kingdom tomb decoration, horizontal register composition with processional figures, mineral pigment palette (ochre, blue frit, white gypsum, black carbon), matte plaster surface`
- `Egyptian lotus-and-papyrus alternating border on a painted column capital, flat color fields, firm outlines`
- `winged sun disk pectoral in gold with lapis lazuli and carnelian inlay, bilateral symmetry, on dark ground`

### Japanese
- `Japanese Edo-period textile pattern, seigaiha (blue ocean waves) repeat on indigo-dyed cotton, stencil-dyed finish`
- `asymmetric ink-wash painting of pine branches with negative space, on silk scroll, Muromachi period style`
- `gold maki-e lacquer surface with chrysanthemum-and-stream motif, dark lacquer ground`

### Islamic
- `Moroccan zellige cut-tile mosaic, 8-fold star tessellation, earth-tone glaze palette (white, green, blue, honey), matte ceramic surface`
- `Persian Safavid manuscript illumination border with vegetal arabesque in gold and lapis on cream paper`
- `Ottoman Iznik ceramic tile panel with tulip-and-carnation motifs, cobalt blue and tomato red on white ground`

### Mesoamerican
- `Maya Late Classic carved limestone lintel with figural scene, deep-channel relief, traces of red pigment`
- `Aztec monumental basalt sculpture surface with radiating calendar glyphs, concentric ring composition`
- `Mixtec codex page with flat polychrome figures, black outlines, screenfold format on bark paper`

### European
- `Insular manuscript page border, Celtic interlace knotwork in ink and pigment on vellum, similar to Book of Kells`
- `Gothic stone tracery window, pointed-arch mullions with quatrefoil subdivisions, limestone`
- `Renaissance grotesque candelabra panel with vine scrolls, hybrid figures, and architectural elements, painted fresco`

### Slavic
- `Ukrainian Petrykivka floral painting, stylized flowers and berries in saturated red, blue, and green on black ground`
- `Russian Khokhloma lacquer, red and gold vegetal scrollwork on black lacquer ground, curved wooden surface`
- `cross-stitch embroidery border on linen, red thread, Ukrainian geometric diamond-and-cross pattern`

---

## Repair strategies

If a single-culture prompt is producing drifted or generic results:

1. **Add material.** "Carved limestone" or "silk brocade" or "painted ceramic" — material anchors the output.
2. **Add composition.** "Horizontal registers" or "radial medallion" or "asymmetric branch composition" — composition prevents generic layout.
3. **Add exclusions.** "No fantasy elements," "No glowing effects," "No metallic chrome surfaces."
4. **Replace broad terms.** "Egyptian art" → "New Kingdom tomb painting." "Japanese style" → "Edo-period woodblock print."
5. **Name the motif.** "Lotus-and-papyrus border" not "Egyptian border." "Seigaiha wave repeat" not "Japanese waves."
6. **Reduce aesthetic intensity.** If the output looks too dramatic, add "matte surface," "period-appropriate materials," "no cinematic lighting."

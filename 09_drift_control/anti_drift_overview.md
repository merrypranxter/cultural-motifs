# Anti-Drift Overview

## Problem definition

Drift is the tendency for cultural motif descriptions, prompts, and generative outputs to lose specificity and collapse into vague, flattened, or fantasy-coded versions of the original traditions.

Drift is the central failure mode this repository is designed to prevent.

---

## Why drift happens

Drift happens because:

1. **Training data bias** — generative AI models are trained on datasets where cultural motifs are frequently mislabeled, mixed, or described in vague terms. The model's default outputs reflect these biases.

2. **Lazy language** — users and agents reach for broad aesthetic labels ("ancient," "exotic," "ornate") instead of specific formal descriptions. Vague input produces vague output.

3. **Neighboring culture conflation** — adjacent or related traditions get merged because the differences seem small. Maya becomes "Aztec." Japanese becomes "Asian." Russian folk becomes "medieval European."

4. **Fantasy contamination** — AI systems generate pseudo-historical imagery that looks vaguely like a tradition but matches no actual examples. This is especially common with Egyptian, Celtic, Viking, and Mesoamerican content.

5. **Decorative soup** — multiple traditions get blended into one generic "world ornament" aesthetic. Everything becomes symmetrical, gold, ornate, and culturally rootless.

6. **Symbolic overclaiming** — motifs get assigned universal or mystical meanings that flatten their actual cultural specificity. "This spiral represents the eternal cycle of life" applied to every spiral everywhere.

---

## Typical bad outputs

- "Ancient Egyptian temple" that looks like a sci-fi set with glowing hieroglyphs
- "Japanese pattern" that is actually a generic floral with no connection to any Japanese textile or painting tradition
- "Celtic knotwork" that is actually generic interlace with no formal connection to Insular manuscript or stone carving conventions
- "Islamic geometric art" that is a random geometric pattern with no actual star-polygon construction logic
- "Aztec design" that mixes Maya, Aztec, and fantasy elements with skull overemphasis
- "Sacred geometry" that combines Islamic tessellation, Hindu mandala, and Platonic solid imagery into meaningless mush
- "Tribal pattern" that is a generic zigzag or diamond grid with no connection to any actual tradition

---

## How to identify drift

A file, prompt, or output has drifted when:

- it uses vague aesthetic labels instead of specific motif names
- it conflates two or more distinct traditions
- it sounds like a gift-shop plaque or a fantasy lore entry
- it assigns universal meaning to a culture-specific motif
- it could apply to any culture equally well (i.e., it has lost all specificity)
- it uses forbidden terms: "tribal," "exotic," "oriental," "ancient vibe," "ethnic ornament," "mystic geometry"
- the visual output matches no actual examples from the named tradition

---

## How to repair drift

1. **Name the culture or tradition specifically.** Replace "ancient pattern" with "Egyptian lotus-and-papyrus border" or "Aztec stepped-fret relief."

2. **Name the motif family specifically.** Replace "ornamental design" with "star-polygon tessellation" or "acanthus scroll frieze."

3. **Name the material context.** Replace "decorated surface" with "carved limestone relief" or "silk brocade" or "cut-tile mosaic."

4. **Name the compositional behavior.** Replace "decorative border" with "running meander border" or "interlace band" or "stepped-fret frame."

5. **Remove vague modifiers.** Delete "ancient," "mystical," "sacred," "tribal," "exotic" unless they refer to something specific and documented.

6. **Add exclusion language where needed.** "Do not include fantasy elements," "Do not mix with [other tradition]," "Do not add glowing effects."

7. **Check against real examples.** If the output doesn't look like anything that actually exists in the named tradition, the prompt has drifted.

---

## Safer alternatives

Instead of vague prompts, use structured prompts that specify:

- culture or region
- motif family
- material context
- composition type
- what to exclude

See `10_prompt_system/` for detailed prompt construction guidance.

# Overgeneralization Failure

## Problem definition

Overgeneralization is the drift pattern where distinct cultural motif traditions are described or generated as if they were interchangeable variants of one universal ornamental system.

This is one of the most common and damaging failure modes in AI-generated cultural content.

---

## Why this drift happens

- **Broad category labels** — terms like "ancient art," "traditional patterns," "world ornament," and "ethnic design" encourage the model to average across traditions rather than distinguish them.
- **Visual similarity at a distance** — geometric patterns from different traditions can look superficially similar. Without specific formal analysis, they get merged.
- **Training data aggregation** — datasets often group motifs by broad visual type ("geometric," "floral") rather than by tradition, encouraging cross-cultural conflation.
- **User intent ambiguity** — users often want "something that looks like X" without specifying which version of X from which tradition. The system fills the gap with a generic average.
- **Symbolism inflation** — when broad symbolic meanings (life, death, eternity, protection) are applied to motifs from every tradition, the motifs become interchangeable carriers of the same vague ideas.

---

## Typical bad outputs

- A "geometric pattern" that blends Islamic star-polygon logic with Celtic interlace and Japanese asanoha into something that matches none of them
- A "dragon" that has Chinese whiskers, European bat wings, and a Mesoamerican feathered body
- A "floral border" that blends Islamic arabesque, European rinceau, and Chinese peony scroll into generic vine filler
- A "temple interior" that combines Egyptian columns, Islamic muqarnas, Hindu deity niches, and Gothic pointed arches
- An "ancient manuscript page" that uses vaguely Celtic interlace borders with vaguely Islamic geometric fills and vaguely Egyptian hieroglyphic figures

---

## How to identify the failure

The output has overgeneralized when:

- it contains elements from multiple traditions without naming or separating them
- it matches no single real tradition well
- it could be described as "world ornament" or "pan-cultural decoration"
- the prompt uses broad terms like "traditional," "ancient," "ethnic," or "ornate" without a culture-specific anchor
- removing the culture label from the output description would not change what it looks like

---

## How to repair it

1. **Anchor to one tradition.** Specify the culture, region, and period. "Ottoman Iznik ceramic tile pattern" not "Islamic pattern." "Maya carved limestone relief" not "Mesoamerican art."

2. **Specify formal traits from that tradition.** Use motif names, symmetry types, material contexts, and compositional structures specific to the named tradition.

3. **Exclude conflicting elements.** "Do not include European heraldic forms." "No winged dragons." "Do not combine with Celtic interlace."

4. **Check the output against real examples.** If the result doesn't look like something that exists in the named tradition, the prompt is still too broad.

5. **If comparison is intentional, make it explicit and controlled.** "Show an Islamic 8-fold tessellation next to a Japanese asanoha pattern for comparison" — not "blend Islamic and Japanese geometric patterns."

---

## Safer alternatives

- Replace "ancient pattern" → "Egyptian New Kingdom tomb painting border"
- Replace "traditional design" → "Uzbek suzani embroidery with pomegranate medallions"
- Replace "ethnic ornament" → "Yoruba adire resist-dyed indigo textile pattern"
- Replace "geometric art" → "Moroccan zellige 8-fold star tessellation"
- Replace "dragon" → "Chinese five-clawed long in cloud-and-wave field"

The fix is always the same: replace the vague category with a specific tradition, motif, material, and composition.

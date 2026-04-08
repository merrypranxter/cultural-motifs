# Anti-Slop Prompting

## Goal

Identify and eliminate the most common prompt language patterns that produce generic, culturally flattened, or fantasy-drifted outputs — and replace them with specific, grounded alternatives.

---

## Prompt construction logic

Slop is the result of vague, unanchored prompt language that gives the generative system permission to average across its training data. Anti-slop prompting works by:

1. Replacing broad aesthetic terms with specific formal descriptions
2. Replacing mood words with material and compositional instructions
3. Adding exclusion language to block common drift patterns
4. Anchoring every prompt in a named tradition, material, and composition

---

## What to specify explicitly

Every anti-slop prompt should include:

| Element | What it prevents |
|---|---|
| Named tradition | Prevents "world ornament" averaging |
| Named motif family | Prevents random decorative fill |
| Named material | Prevents generic shiny/gold/chrome surfaces |
| Named composition | Prevents random layout |
| Exclusions | Prevents fantasy and neighboring-culture drift |

---

## What to avoid

### Forbidden prompt phrases (these produce slop)

| Slop phrase | Why it fails | Better alternative |
|---|---|---|
| "ancient pattern" | No tradition, no motif, no material | "Egyptian lotus-and-papyrus border on painted limestone" |
| "tribal design" | Erases all specificity | "Maori tā moko curvilinear tattoo forms" or "Navajo diamond-and-zigzag woven textile" |
| "exotic ornament" | Meaningless aesthetic label | Name the tradition and motif family |
| "oriental pattern" | Collapses all of Asia | "Chinese blue-and-white porcelain floral" or "Japanese asanoha textile repeat" |
| "sacred geometry" | Conflates multiple unrelated traditions | "Islamic 10-fold star tessellation" or "Hindu mandala with lotus petal ring" |
| "mystical symbols" | Fantasy-coded, unanchored | Name the specific motif and tradition |
| "ethnic design" | Vague and othering | Name the ethnic group and their specific motif tradition |
| "inspired by [culture]" | License to drift | "In the style of [specific tradition/medium/period]" |
| "ornate and elegant" | Mood words, not form | "Dense vegetal arabesque field fill" or "acanthus scroll with egg-and-dart border" |
| "ancient civilization aesthetic" | Conflates everything old | Name the civilization, period, and medium |

### Forbidden modifier stacks

These modifier combinations reliably produce slop:

- "ancient mystical sacred geometric" — this is four vague words stacked
- "ornate elegant royal ceremonial" — mood words, not visual description
- "tribal ethnic folk traditional" — four synonyms for "not European, don't care which"

---

## Example prompt fragments

### Before (slop) → After (repaired)

**Slop:** `Beautiful ancient Egyptian design with gold and turquoise sacred symbols`
**Repaired:** `Egyptian New Kingdom pectoral design: winged scarab centerpiece with gold, lapis lazuli, and carnelian inlay, bilateral symmetry, dark background, based on Tutankhamun-era jewelry`

**Slop:** `Japanese zen garden pattern, peaceful and serene`
**Repaired:** `Raked gravel (karesansui) dry garden, concentric circle patterns around placed stones, grey-white gravel, overhead view, Ryoan-ji style`

**Slop:** `Islamic sacred geometry, colorful and intricate`
**Repaired:** `Moroccan zellige cut-tile mosaic, 10-fold star tessellation, matte glazed ceramic, palette of white, cobalt blue, green, and honey yellow, flat surface, no 3D effects`

**Slop:** `Celtic tribal knotwork, mystical and ancient`
**Repaired:** `Insular manuscript interlace panel, ribbon knotwork with animal-head terminals, ink and pigment on vellum, based on Book of Kells carpet page`

**Slop:** `Aztec tribal skull pattern`
**Repaired:** `Aztec tzompantli (skull rack) relief panel, carved basalt, rows of skulls in profile on horizontal bars, monumental architectural context`

**Slop:** `Colorful Indian pattern`
**Repaired:** `Mughal jali screen pattern: perforated marble with hexagonal geometric lattice, based on Fatehpur Sikri examples`
or: `Rajasthani block-printed cotton textile, red and indigo, small-scale floral repeat, resist-dyed`

---

## Repair strategies

### Step 1: Identify the vague elements
Read the prompt and circle anything that could apply to more than one tradition. Those are the slop points.

### Step 2: Replace each vague element with a specific one
- Vague culture → specific tradition
- Vague motif → specific motif family
- Vague material → specific medium and surface
- Vague composition → specific layout type
- Mood words → formal descriptors

### Step 3: Add exclusions
- "No fantasy elements"
- "No glowing or neon effects"
- "No chrome or metallic surfaces unless historically documented"
- "Do not combine with [other tradition]"
- "Period-accurate materials only"

### Step 4: Test against reality
Would the result look like something that actually exists or existed in the named tradition? If not, the prompt still has slop in it.

### Step 5: Reduce if necessary
If the prompt is still producing bad results after repair, simplify. A shorter, more specific prompt often works better than a long, hedge-everything prompt. Focus on: one tradition, one motif, one material, one composition.

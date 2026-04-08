# FILE TEMPLATES

## Template A — region overview file

Use for:
- 03_regions_and_cultures/*/overview.md

Sections:
1. Purpose
2. Scope
3. Core visual traits
4. Common motif families
5. Composition grammar
6. Material and surface tendencies
7. Symbolic tendencies
8. Common confusion risks
9. Prompting / genart implications

---

## Template B — culture-specific motif file

Use for:
- japanese.md
- maya.md
- russian.md
- motifs.md
- symbols_and_beings.md

Sections:
1. Purpose
2. Main motifs or categories
3. How the motifs are typically used visually
4. Symbolic roles or associations
5. Materials / surfaces / contexts
6. What this is not
7. Prompting notes

---

## Template C — cross-cultural motif family file

Use for:
- serpents_dragons_and_feathered_beings.md
- knotwork_meanders_and_interlace.md
- floral_vine_and_tree_systems.md

Sections:
1. Purpose
2. Why these forms are being grouped together
3. Shared visual logic
4. Major cultural variants
5. Important symbolic differences
6. Common confusion risks
7. Prompting / retrieval notes

---

## Template D — anti-drift file

Use for:
- anti_drift.md
- anti_drift_overview.md
- fantasy_mishmash_failure.md

Sections:
1. Problem definition
2. Why this drift happens
3. Typical bad outputs
4. How to identify the failure
5. How to repair it
6. Safer alternatives

---

## Template E — prompt-system file

Use for:
- single_culture_prompting.md
- careful_hybridization.md
- anti_slop_prompting.md

Sections:
1. Goal
2. Prompt construction logic
3. What to specify explicitly
4. What to avoid
5. Example prompt fragments
6. Repair strategies

---

## Template F — JSON object pattern for motif entries

Suggested fields:
- id
- label
- region
- subregion_or_culture
- category
- visual_traits
- symbolic_roles
- materials_contexts
- confusion_risks
- prompt_tags

Keep arrays concise and stable.

---

## Template G — CSV comparison table

Suggested columns:
id,culture_or_region,motif_family,visual_form,symbolic_role,material_context,confusion_risk,prompt_tags

One row per motif-family/culture combination.

# Repo Structure

This document explains the folder structure of the Cultural Motifs Repo and what each section is for.

The structure is designed to balance three needs:

1. **cultural specificity**
2. **cross-cultural comparison**
3. **machine usability**

---

## Top-level files

### `README.md`
Repository overview, purpose, standards, and contributor guidance.

### `REPO_STRUCTURE.md`
Explanation of the folder structure and the purpose of each directory.

### `AGENT_BUILD_PLAN.md`
Execution plan for repository-building agents.

### `AGENT_GENERATION_RULES.md`
Rules for generating files safely and consistently.

### `FILE_TEMPLATES.md`
Stable templates for repeated file types.

---

## `00_scope_and_method/`

This folder defines how the repo thinks.

### Files

- `repo_purpose.md`
- `usage_modes.md`
- `cultural_respect_and_accuracy.md`
- `terminology_rules.md`
- `scope_boundaries.md`
- `uncertainty_and_evidence.md`

### Purpose

This section establishes:
- what the repo is for
- what it is not for
- terminology to avoid
- how to write conservatively when evidence is uneven
- how to distinguish analysis from overclaiming

Without this section, the repo tends to drift into decorative anthropology cosplay.

---

## `01_foundation/`

This folder defines the basic analytical framework.

### Files

- `what_is_a_motif.md`
- `motif_dimensions.md`
- `symbolic_function_vs_visual_form.md`
- `motif_scale_levels.md`
- `visual_analysis_method.md`

### Purpose

This section answers:
- what counts as a motif
- what kinds of traits are worth documenting
- how motifs behave differently at the scale of icon, border, panel, surface, garment, building, or scene
- how to separate visual description from symbolic interpretation

This is the repo’s grammar layer.

---

## `02_taxonomy/`

This folder organizes motifs by major formal classes.

### Files

- `motif_taxonomy_overview.md`
- `geometry_motifs.md`
- `flora_motifs.md`
- `fauna_motifs.md`
- `deity_guardian_and_spirit_motifs.md`
- `cosmology_motifs.md`
- `architecture_motifs.md`
- `border_frame_and_panel_motifs.md`
- `textile_and_surface_motifs.md`
- `ceremonial_object_motifs.md`

### Purpose

This section provides the cross-repo taxonomy used by both markdown analysis and structured data.

It allows motifs to be grouped by category while still being traced back to specific regions and traditions.

---

## `03_regions_and_cultures/`

This is the main body of the repository.

### Current region folders

- `egyptian/`
- `mesoamerican/`
- `east_asian/`
- `south_asian/`
- `southeast_asian/`
- `islamic_world/`
- `slavic_and_eurasian/`
- `european/`

### Purpose

This section documents motifs in their cultural or regional context.

It is the repo’s main specificity layer.

Each region folder should contain:
- overview
- motif files
- beings / symbols / objects where relevant
- palette / materials
- anti-drift

### Why this section matters

If the repo only had motif-family files, everything would get flattened.
If the repo only had region folders, comparison would become clumsy.

This section anchors the repo in actual traditions.

---

## `04_cross_cultural_motif_families/`

### Files

- `serpents_dragons_and_feathered_beings.md`
- `birds_suns_moons_and_stars.md`
- `guardian_figures.md`
- `masks_faces_and_deities.md`
- `knotwork_meanders_and_interlace.md`
- `tessellations_lattices_and_repeat_grids.md`
- `stepped_forms_pyramids_and_cosmic_axes.md`
- `floral_vine_and_tree_systems.md`

### Purpose

This section compares motif families that recur across multiple traditions.

It is **not** meant to erase cultural distinctions.
It is meant to compare:
- shared formal logic
- differing symbolic roles
- differing material uses
- differing compositional behaviors

This section is useful for:
- prompt design
- retrieval systems
- motif comparison
- generative abstraction

---

## `05_formal_visual_logic/`

### Files

- `symmetry_types.md`
- `repetition_and_tiling.md`
- `radial_vs_band_vs_field_composition.md`
- `sacred_centering.md`
- `hieratic_scale_and_rank.md`
- `density_and_negative_space.md`
- `abstraction_levels.md`

### Purpose

This section tracks visual behavior at the compositional level.

It helps answer questions like:
- how dense is the surface treatment?
- is the motif used as a border, field, axis, or emblem?
- what kind of symmetry is dominant?
- does the system prefer centered hierarchies, distributed fields, or stacked zones?

This section is especially useful for shaders, generative layout systems, and retrieval tags.

---

## `06_materials_color_and_surface/`

### Files

- `palette_logic_overview.md`
- `pigments_dyes_and_stones.md`
- `metals_enamel_and_gilding.md`
- `carved_relief_logic.md`
- `tile_ceramic_and_mosaic_logic.md`
- `textile_embroidery_and_weave_logic.md`
- `lacquer_ink_paper_and_parchment.md`
- `age_wear_and_restoration_drift.md`

### Purpose

This section tracks how motifs are expressed through materials and surfaces.

It helps distinguish:
- carved vs painted vs woven vs tiled logic
- matte vs reflective systems
- stone vs textile vs manuscript behavior
- authentic surface tendencies vs modern decorative drift

---

## `07_symbolic_roles_and_meaning/`

### Files

- `cosmology_and_creation.md`
- `protection_and_guardianship.md`
- `royalty_power_and_divinity.md`
- `fertility_growth_and_life_cycles.md`
- `death_underworld_and_transition.md`
- `luck_trickery_and_threshold_beings.md`
- `warfare_order_and_authority.md`
- `domestic_folk_and_ritual_use.md`

### Purpose

This section groups symbolic roles that recur across cultures.

It should remain cautious and explicit about variation.
It is useful for:
- meaning-oriented prompting
- comparison
- thematic indexing

This section should never imply that all similar motifs share the same meaning.

---

## `08_folklore_and_specific_beings/`

### Files

- `kitsune.md`
- `dragons_by_region.md`
- `phoenix_and_firebirds.md`
- `sphinx_and_guardian_hybrids.md`
- `feathered_serpents.md`
- `saints_spirits_and_ancestor_figures.md`
- `trickster_figures.md`

### Purpose

This section tracks specific beings, creatures, and mythic figure types that appear across or within traditions.

It is useful because many users search for specific figures rather than abstract categories.

---

## `09_drift_control/`

### Files

- `anti_drift_overview.md`
- `what_this_repo_is_not.md`
- `neighboring_style_confusions.md`
- `fake_archaeology_failure.md`
- `fantasy_mishmash_failure.md`
- `decor_slop_failure.md`
- `overgeneralization_failure.md`
- `diagnostic_checklist.md`
- `repair_strategies.md`

### Purpose

This is the repo’s anti-bullshit firewall.

It documents:
- common misuse patterns
- neighboring style confusions
- fantasy drift
- decor drift
- broad vibe-language failure
- repair methods

If this section is weak, the entire repo becomes easier to misuse.

---

## `10_prompt_system/`

### Files

- `prompt_formula_short.md`
- `prompt_formula_long.md`
- `single_culture_prompting.md`
- `comparative_prompting.md`
- `careful_hybridization.md`
- `anti_slop_prompting.md`
- `motif_injection_templates.md`
- `scene_builder_templates.md`

### Purpose

This section translates the analysis into prompt logic.

It explains:
- what to specify
- what to avoid
- how to maintain specificity
- how to compare without flattening
- how to build hybrid prompts carefully

This is the deployment layer for image, video, text, and design prompting.

---

## `11_shader_and_genart_translation/`

### Files

- `symmetry_engines.md`
- `tiling_and_repeat_logic.md`
- `border_generators.md`
- `glyph_and_icon_placement.md`
- `relief_emboss_and_inlay_simulation.md`
- `mosaic_tile_logic.md`
- `textile_repeat_logic.md`
- `region_sensitive_parameter_sets.md`

### Purpose

This section translates motif systems into procedural logic.

It is useful for:
- shader artists
- generative art systems
- p5 / GLSL / touchdesigner / node-based systems
- UI controls for motif generation

This section should focus on behavior, not pseudo-history.

---

## `12_app_integration/`

### Files

- `style_spec_schema.md`
- `retrieval_tags.md`
- `composable_motif_blocks.md`
- `ui_filter_categories.md`
- `recommendation_logic.md`

### Purpose

This section explains how the repo can plug into software systems.

It should support:
- structured retrieval
- filtering
- motif recommendations
- comparison views
- modular style blocks

---

## `13_structured_data/`

### Files

- `style_spec.json`
- `culture_index.json`
- `motif_library.json`
- `motif_families.json`
- `symbolic_roles.json`
- `color_material_profiles.json`
- `anti_drift_rules.json`
- `prompt_templates.json`
- `comparison_table.csv`

### Purpose

This section provides machine-readable support files.

These files should be:
- valid
- stable
- concise
- mirrored to the markdown taxonomy

This section is not meant to replace the markdown.
It is meant to support programmatic use.

---

## `14_examples/`

### Files

- `example_prompts.md`
- `example_scene_breakdowns.md`
- `example_hybrids_good_vs_bad.md`
- `example_shader_translation_notes.md`

### Purpose

This section demonstrates how to use the repo’s logic in practice.

Examples should show:
- good prompting
- bad prompting
- careful comparison
- drift repair
- generative translation

---

## Structural principle

The repo works best when these three layers stay in balance:

1. **specificity**
   - region folders
   - culture files
   - material context

2. **comparison**
   - cross-cultural motif families
   - symbolic-role categories
   - formal visual logic

3. **deployment**
   - prompting
   - shaders
   - structured data
   - app integration

If one layer overwhelms the others, the repo gets stupid.

---

## Recommended build order

1. top-level control docs
2. scope and foundation
3. taxonomy
4. region overviews
5. region subfiles
6. cross-cultural motif family files
7. drift-control files
8. prompt-system files
9. structured data
10. examples

This order ensures that the repo gets a spine before it gets decorative bulk.

# AGENT BUILD PLAN

## Objective

Expand the cultural motifs repository in a controlled way using the existing repo structure, rules, and exemplar files.

## Generation order

Generate files in this order:

1. core control documents if missing
2. foundation files
3. taxonomy files
4. region overview files
5. region subfiles
6. cross-cultural motif family files
7. drift-control files
8. prompt-system files
9. structured data files
10. examples and optional expansion files

## First-pass priority

Prioritize the following file types first:
- overview files
- motif files
- anti-drift files
- prompt-system files
- structured data indexes

These create the repository's load-bearing skeleton.

## Region generation strategy

For each region folder:
1. create overview.md
2. create the region's motif-specific files
3. create palette/materials file
4. create anti_drift.md

Do not skip anti-drift.

## Cross-cultural generation strategy

Cross-cultural files must compare motif families without pretending they mean the same thing in every culture.
These files should emphasize:
- formal similarities
- symbolic differences
- compositional differences
- confusion risks

## Structured data generation strategy

Structured data should be derived from:
- taxonomy files
- region files
- cross-cultural files
- drift-control files

Do not invent giant uncontrolled schemas.
Keep them compact, stable, and obviously useful.

## Quality control checks

Before finalizing any generated file, check:
- is the culture or region being described specifically enough?
- did the file confuse visual form with symbolic meaning?
- did the file use lazy umbrella wording?
- did the file accidentally sound like fantasy lore?
- does the structure match comparable files already in the repo?

## Failure conditions

The following are considered failures:
- flattening cultures into one style blob
- invented symbolism stated as fact
- vague decorative language instead of actual analysis
- "world pattern" tone
- poor markdown structure
- invalid JSON or CSV

## Repair behavior

If a generated file is too vague or drifted:
1. narrow the scope
2. reduce claims
3. separate visual and symbolic content
4. add a confusion-risks section
5. align with the nearest valid exemplar

# CHAR-001 Reference Generation Workflow

## Objective

Create the canonical visual reference package without allowing identity drift.

## Order

1. Master Portrait
2. Neutral Front
3. 3/4 Left
4. 3/4 Right
5. Profile
6. Full Body
7. Expression Sheet
8. Wardrobe Sheet

## Gate 0: identity brief

Before generation, lock:

- character ID
- character version
- physical identity
- permanent features
- baseline wardrobe
- visual target
- negative constraints

## Gate 1: Master Portrait

The Master Portrait is the visual anchor.

Requirements:

- neutral expression
- direct or controlled camera orientation
- natural skin texture
- clear facial geometry
- consistent lighting
- no distracting accessories
- no stylization that prevents identity comparison

Do not approve a Master Portrait with visible identity ambiguity.

## Gate 2: Multi-angle references

Generate views from the approved Master Portrait.

Each new view must be compared against the anchor.

Reject if facial structure, hair identity, permanent features or apparent age drift.

## Gate 3: Full-body and wardrobe

Validate body proportions and clothing separately from facial identity.

## Gate 4: Expression sheet

Expressions may vary.

Identity may not.

Required expressions:

- neutral
- happy
- concerned
- afraid
- angry
- sad
- relieved

## Gate 5: Canonical lock

Only after all references pass QA:

- set package status to APPROVED
- record asset IDs
- record model/workflow/version
- record provenance
- update character status from DRAFT to APPROVED

## Regeneration rule

Never regenerate the entire package because one reference failed.

Regenerate the smallest failed unit and re-run identity QA.

## Cost gate

Generation may only use an approved free/local workflow.

Any workflow with uncertain or variable cost is BLOCKED.

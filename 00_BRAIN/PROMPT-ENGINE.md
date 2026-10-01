# Prompt Engine

## Purpose

Generate production prompts from structured canonical data.

Prompts are compiled outputs, not the source of truth.

## Input layers

1. Global visual identity
2. Character identity
3. Character reference assets
4. Location identity
5. Scene intent
6. Shot specification
7. Acting/performance
8. Camera/cinematography
9. Lighting/color
10. Quality constraints
11. Negative constraints
12. Model-specific adapter

## Principle

The same Shot Spec should be usable with different generation models through model adapters.

Never rewrite canon simply to satisfy a model.

## Character prompt construction

A character prompt should reference:

- character_id
- approved reference assets
- immutable physical identity
- current expression
- current pose
- wardrobe state
- emotional state

## Negative constraints

Where supported, reject or suppress:

- face drift
- identity change
- age change
- extra fingers/limbs
- deformed anatomy
- duplicate subjects
- unwanted text
- logos
- watermarks
- temporal artifacts
- morphing

## Versioning

Record:

- prompt_version
- model
- model_version
- workflow_version
- parameters
- input reference IDs

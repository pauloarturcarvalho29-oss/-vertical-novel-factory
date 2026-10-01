# Image Workflow

## Purpose

Provide a reproducible local image-generation workflow for character references and cinematic keyframes.

## Required properties

- local/free execution
- deterministic or seed-controlled generation where supported
- reference-image conditioning
- explicit resolution controls
- reproducible parameters
- provenance capture

## Pipeline

Character Spec
→ Reference Brief
→ Generation Workflow
→ Candidate Images
→ Identity QA
→ Approved Asset
→ Asset Manifest

## Character consistency

The workflow must support reference-driven generation.

Text-only regeneration is insufficient for canonical character continuity.

## Quality

Prefer the highest practical source resolution supported by the hardware.

Do not upscale a weak generation and call it a high-quality master.

## Cost

FREE / LOCAL only unless explicit user approval changes the policy.

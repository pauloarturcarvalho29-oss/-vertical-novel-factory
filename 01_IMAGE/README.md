# Image Generation

This module converts approved Character Specs, Scene Specs and Shot Specs into consistent still images, character references, keyframes and other visual assets.

## Initial strategy

- Orchestrator: ComfyUI
- Primary use: character references, keyframes and still assets
- Video generation consumes approved keyframes rather than relying on uncontrolled long-form generation
- Exact model/version/license must be recorded before production use

## Quality gates

1. Character identity matches canonical references.
2. Location and props match the scene.
3. Composition satisfies the Shot Spec.
4. No unwanted text, logos or artifacts.
5. Asset provenance is complete.

## Required output

Every approved image receives an asset ID and provenance record in the asset manifest.

## Cost policy

Free/open-source first. No paid API or service may enter the pipeline without explicit approval.

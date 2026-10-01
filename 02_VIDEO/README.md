# Video Generation

This module converts approved visual assets and Shot Specs into short vertical video shots.

## Initial strategy

- Orchestration: ComfyUI
- Candidate models: Wan family and LTX family, subject to exact version/license verification
- Generate short shots and assemble them in EDIT rather than depending on long continuous generations
- Preserve character and environment references across shots

## Target

Master: 1080x1920, 9:16.

## Quality gates

1. Character identity is preserved.
2. Motion follows the Shot Spec.
3. Camera movement is intentional.
4. No severe temporal artifacts.
5. Shot duration and framing are correct.
6. Provenance records are complete.

## Cost policy

Free/open-source first. Paid or uncertain-cost services require explicit approval.

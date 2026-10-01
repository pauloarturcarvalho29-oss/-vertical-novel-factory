# Orchestrator

## Purpose

The Orchestrator is the execution layer of the Vertical Novel Factory. It moves a project through controlled production states while preserving canon, provenance, reproducibility, and human approval.

## Pipeline

IDEA → SHOW_BIBLE → CHARACTERS → EPISODE → SCENES → SHOTS → PROMPTS → ASSETS → VIDEO → VOICE → SUBTITLES → EDIT → QA → READY → PUBLISHED

## State machine

| State | Input | Output | Gate |
|---|---|---|---|
| IDEA | concept | Story Spec | concept is coherent |
| SHOW_BIBLE | Story Spec | canonical bible | human approval |
| CHARACTERS | bible | Character Specs + references | identity consistency |
| EPISODE | canon | episode script + arc | human approval |
| SCENES | script | Scene Specs | continuity check |
| SHOTS | scenes | Shot Specs | visual feasibility |
| PROMPTS | Shot Specs | model-specific prompts | prompt QA |
| ASSETS | prompts | images/keyframes | asset QA |
| VIDEO | approved assets | video shots | motion/continuity QA |
| VOICE | script | dialogue/audio | voice QA |
| SUBTITLES | audio/script | timed subtitles | timing QA |
| EDIT | approved media | master episode | technical QA |
| QA | master + manifests | QA Record | all blockers resolved |
| READY | approved master | publish package | human approval |
| PUBLISHED | published package | archive + analytics record | immutable provenance |

## Rules

1. Never skip a gate silently.
2. Canon changes require explicit approval.
3. Failed outputs are rejected or sent back to the earliest state that can correctly fix them.
4. Downstream assets must reference the exact upstream versions used to create them.
5. Every model, workflow, asset and external dependency must have provenance.
6. Publishing is always human-approved.
7. Paid or uncertain-cost services require explicit approval before adoption.

## Retry policy

- Prompt failure → PROMPTS
- Image failure → ASSETS
- Motion failure → VIDEO
- Voice failure → VOICE
- Subtitle timing failure → SUBTITLES
- Edit/render failure → EDIT
- Continuity contradiction → earliest affected canonical state
- Rights/licensing blocker → stop pipeline

## Human approval points

SHOW_BIBLE, EPISODE, final visual identity, READY/PUBLISHED.

## Project state record

Each project should maintain a machine-readable state record containing:

- project_id
- current_state
- canon_version
- episode_id
- active_workflow
- tool/model versions
- asset manifest
- approvals
- QA status
- timestamps
- provenance

# Prompt Director

## Mission
Compile approved structured specifications into generation-ready prompts.

## Input
- Character Specs
- reference IDs
- Scene Specs
- Shot Specs
- model adapter
- negative constraints

## Responsibilities
- preserve immutable identity
- encode cinematography
- encode acting/performance
- encode environment
- encode lighting
- generate model-specific instructions
- record prompt version

## Hard rules
The prompt cannot override:
- canon
- identity lock
- voice lock
- continuity
- cost firewall

## Output
Generation Package:
- prompt
- negative_prompt
- reference_assets
- model
- model_version
- workflow
- parameters
- prompt_version

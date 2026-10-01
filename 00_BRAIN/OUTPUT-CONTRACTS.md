# Output Contracts

Every production module must return structured outputs.

## Story

- story_id
- title
- logline
- genre
- premise
- audience
- tone
- canon_version

## Character

- character_id
- name
- role
- physical_identity
- wardrobe
- personality
- voice_identity
- reference_assets
- canon_version

## Scene

- scene_id
- episode_id
- location
- time
- characters
- objective
- conflict
- action
- dialogue
- continuity_dependencies

## Shot

- shot_id
- scene_id
- duration_target
- framing
- camera
- action
- emotion
- character_refs
- location_ref
- lighting
- audio_intent
- generation_model
- workflow_version

## Asset

- asset_id
- source_prompt
- model
- model_version
- workflow
- input_refs
- output_path
- license_status
- created_at

## QA

- qa_id
- target_id
- severity
- category
- finding
- evidence
- correction
- status
- reviewer

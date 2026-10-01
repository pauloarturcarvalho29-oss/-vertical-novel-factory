# Asset Manifest

Every production asset must be traceable.

## Required fields

- asset_id
- asset_type
- project_id
- episode_id
- scene_id
- shot_id
- character_ids
- source_prompt
- prompt_version
- model
- model_version
- workflow
- workflow_version
- input_asset_ids
- output_path
- creation_timestamp
- license_status
- cost_status
- qa_status
- approved_by

## Cost status

Allowed:

- FREE
- FREE-TIER
- LOCAL
- BLOCKED
- APPROVAL_REQUIRED

Never record a paid asset as approved without explicit authorization.

## Provenance principle

A final shot must be traceable back to its references, prompt, workflow and generation model.

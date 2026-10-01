# Brain Schemas

The brain uses structured records so creative decisions can be reproduced and validated.

## Story Spec
- project_id
- title
- premise
- genre
- audience
- tone
- themes
- season_arc
- episode_goal
- hook
- conflict
- escalation
- resolution_or_cliffhanger

## Character Spec
- character_id
- canonical_name
- role
- age_range
- appearance
- wardrobe
- personality
- motivations
- fears
- relationships
- voice_profile
- visual_reference_ids
- continuity_constraints

## Scene Spec
- scene_id
- episode_id
- purpose
- location
- time
- characters
- action
- emotion
- dialogue
- camera
- composition
- lighting
- sound
- duration_seconds
- transition
- continuity_dependencies

## Shot Spec
- shot_id
- scene_id
- duration_seconds
- framing
- camera_motion
- subject_action
- environment
- dialogue
- audio
- image_prompt
- video_prompt
- negative_constraints
- required_references

## QA Record
- asset_id
- stage
- checks
- failures
- warnings
- reviewer
- decision
- timestamp

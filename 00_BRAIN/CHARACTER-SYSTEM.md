# Character System

## Purpose

Create a persistent, versioned identity for every fictional character.

A character is represented by a structured identity package, not by a prompt alone.

## Canonical package

Each character must have:

- character_id
- canonical_name
- role
- age
- physical_identity
- face_identity
- body_identity
- hair_identity
- permanent_features
- wardrobe
- accessories
- expression_range
- personality
- acting_profile
- relationships
- voice_id
- reference_assets
- canon_version
- status

## Reference package

Minimum reference set:

1. Master portrait
2. Neutral front
3. 3/4 left
4. 3/4 right
5. Profile
6. Full body
7. Expression sheet
8. Wardrobe sheet

The system should prefer approved reference assets over textual descriptions when generating downstream assets.

## Identity hierarchy

When sources disagree:

1. approved canonical character record
2. approved reference package
3. current scene specification
4. previous approved shot
5. generation prompt

The prompt cannot redefine identity.

## Versioning

Changes to canonical identity require a new character version and explicit approval.

Example:

CHAR-001 v1.0 → approved
CHAR-001 v1.1 → approved change
CHAR-001 v1.0 remains archived for historical continuity

## Blocking conditions

Reject the asset when there is significant:

- face drift
- body drift
- age drift
- hair drift
- permanent-feature drift
- unexplained wardrobe contradiction


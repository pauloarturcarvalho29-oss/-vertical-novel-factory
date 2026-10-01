# Character Identity Lock

This document defines the strongest continuity constraint in the project.

## Principle

A character is an identity package, not a text prompt.

Every canonical character must have a reference package containing:

- master portrait
- neutral front
- 3/4 left
- 3/4 right
- profile
- full body
- expression sheet
- wardrobe sheet
- hair/accessory sheet
- color references
- character ID

## Immutable identity attributes

The following cannot change between generations without an explicit canonical change:

- facial structure
- eye structure
- nose
- mouth
- jaw
- skin characteristics
- age
- body proportions
- hair identity
- permanent marks

## Controlled variables

These may change only when the Shot Spec permits them:

- facial expression
- pose
- gaze
- body position
- wardrobe, when script continuity permits
- lighting
- makeup for an explicitly established scene
- camera angle
- lens/FOV
- depth of field

## Identity QA

Each generated asset must be checked against the canonical reference.

Severity:

- BLOCKER: visibly different identity
- MAJOR: meaningful drift in facial/body features
- MINOR: small non-story-changing deviation

BLOCKER and MAJOR identity failures cannot enter the final edit.

## Reference priority

When there is a conflict:

1. canonical character record
2. approved character reference package
3. current scene specification
4. previous approved shot
5. generation prompt

The prompt never overrides canon.

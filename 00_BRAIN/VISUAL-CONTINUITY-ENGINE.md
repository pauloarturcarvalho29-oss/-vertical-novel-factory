# Visual Continuity Engine

## Purpose

Prevent scene-to-scene visual contradictions.

## Continuity state

Track per episode:

- character appearance
- wardrobe
- hair
- accessories
- props
- injuries
- emotional state
- location
- geography
- time
- weather
- lighting
- camera axis
- screen direction
- eyelines
- object placement

## Pre-generation check

Before generating a shot:

1. Load canonical character state.
2. Load current scene state.
3. Load previous approved shot.
4. Compare requested state against continuity state.
5. Block contradictions.
6. Produce the generation package only after validation.

## Post-generation check

After generation:

1. Compare character identity.
2. Compare wardrobe.
3. Compare location.
4. Compare lighting.
5. Compare spatial continuity.
6. Compare motion continuity when video is involved.
7. Create a QA record.

## Severity

BLOCKER = release/generation stop.

MAJOR = correction required before READY.

MINOR = record and review.

## Principle

Continuity is stateful. It is not solved by writing a longer prompt.

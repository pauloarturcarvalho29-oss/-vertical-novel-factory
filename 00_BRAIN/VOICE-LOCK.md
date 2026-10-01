# Character Voice Lock

## Principle

One character must sound like one person throughout the series.

## Canonical voice profile

Each character voice record should define:

- character_id
- voice_id
- language
- accent
- vocal age
- timbre
- pitch range
- speech rate
- articulation
- breath/noise profile
- emotional performance range
- reference samples
- model/version
- generation parameters

## Production rule

Once a character voice is approved, the pipeline should reuse the same voice identity and compatible model/workflow.

Do not allow automatic voice switching between scenes.

Do not use a different voice because it sounds "better" in one isolated shot without creating a new approved character voice version.

## Emotion

The voice may change performance while preserving identity:

- calm
- excited
- afraid
- angry
- sad
- whisper
- crying
- laughing

The system must preserve the recognizable speaker identity across these performances.

## Voice QA

Check:

- speaker identity
- consistency with previous approved dialogue
- pronunciation
- emotional performance
- intelligibility
- artifacts
- clipping
- unnatural prosody
- unwanted robotic quality

A robotic or identity-inconsistent result is rejected and regenerated.

## Provenance

Record the exact voice model, version, workflow and parameters for every approved voice asset.

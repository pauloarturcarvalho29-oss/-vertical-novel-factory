# Model Evaluation

Date checked: 2026-10-01

## Cost rule

No model or service is approved if it can create an unauthorized charge.

## Current candidates

### ComfyUI
Role: local orchestration.

The official repository is GPL-3.0 and exposes a local API for programmatic execution. It is suitable as an orchestration layer, subject to respecting GPL obligations for modifications and custom nodes. citeturn1search0turn1search8

Status: CANDIDATE / FREE LOCAL

### Wan 2.2
Role: video generation candidate.

The official repository identifies Wan 2.2 as an open and advanced large-scale video generative model and publishes its package metadata. Exact model-weight licensing and the terms of the specific checkpoint intended for commercial production must be verified from the exact checkpoint before approval.

Status: LICENSE_REVIEW_REQUIRED

### Chatterbox
Role: synthetic voice candidate only if human voice is not used.

The official repository describes Chatterbox as open-source TTS/voice conversion and its project metadata references an MIT license. The system supports audio-prompt voice conditioning. citeturn1search10turn1search7

Status: CANDIDATE / LICENSE VERIFIED AT REPOSITORY LEVEL / MODEL-WEIGHT AND OUTPUT POLICY STILL TO BE RECORDED

Important: this does not override the project's preference for natural human recordings. Any voice cloning requires consent and a documented provenance record.

### WhisperX
Role: transcription, word-level timing and subtitle alignment.

The official repository is BSD-2-Clause. citeturn0search16turn0search1

Status: CANDIDATE / FREE LOCAL

## Selection rule

No model becomes production-approved merely because its source repository is permissively licensed.

For every production checkpoint, record:

- exact repository
- exact checkpoint/model
- version or commit
- model-weight license
- commercial-use terms
- dataset restrictions when relevant
- attribution requirements
- redistribution restrictions
- hardware/runtime requirements
- cost
- verification date

## Current decision

Use a layered architecture:

ComfyUI → orchestration
Wan 2.2 → video candidate pending exact checkpoint license verification
Human voice → preferred voice path
Chatterbox → fallback/candidate only
WhisperX → local subtitle/transcription candidate

No paid API, cloud GPU or subscription is required by this architecture.

# Architecture

## Mission
Vertical Novel Factory is an open-source, mobile-first production system for original vertical novels for TikTok and YouTube.

## Core principle
ChatGPT acts as the creative and planning brain. Heavy media generation runs in cloud/remote/local compute. The iPhone is the control and review surface.

## Pipeline
Story → Characters → Storyboard → Images → Video → Voice → Subtitles → Edit → Publish → Analytics

## Master format
- 1080×1920
- 9:16 vertical
- Short shots assembled into episodes
- Pilot target: 30–45 seconds before scaling to 60–90 seconds

## Layers
- `00_BRAIN`: story, show bible, characters, continuity, prompts, QA
- `01_IMAGE`: character sheets, keyframes, image workflows
- `02_VIDEO`: image-to-video and text/image-to-video workflows
- `03_VOICE`: TTS and character voice workflows
- `04_AUDIO`: music, ambience, SFX
- `05_SUBTITLES`: transcription and timed captions
- `06_EDITING`: assembly, rendering and export
- `07_WORKFLOWS`: reusable production workflows
- `08_EPISODES`: episode source packages and manifests
- `09_ASSETS`: reusable project assets
- `10_DOCUMENTATION`: architecture and operating documentation
- `LICENSES`: third-party model/tool/license ledger

## Quality gates
Every production stage should preserve character identity, continuity, dialogue meaning, timing, aspect ratio, and licensing provenance.

## Cost policy
Paid services, metered APIs, or components with uncertain commercial terms require explicit approval before adoption. Prefer free and open-source components.

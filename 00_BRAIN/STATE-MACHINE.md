# Production State Machine

## Canonical states

`IDEA`, `SHOW_BIBLE`, `CHARACTERS`, `EPISODE`, `SCENES`, `SHOTS`, `PROMPTS`, `ASSETS`, `VIDEO`, `VOICE`, `SUBTITLES`, `EDIT`, `QA`, `READY`, `PUBLISHED`.

## Transition contract

A transition is valid only when:

- required inputs exist;
- the previous state passed its gate;
- referenced versions are immutable;
- no unresolved BLOCKER exists;
- required human approval has been recorded.

## Failure handling

A failure creates a QA record and routes the project backward to the minimum state capable of fixing the problem. Never regenerate the entire episode when a smaller correction is sufficient.

## Terminal condition

`PUBLISHED` is terminal for that exact production version. Corrections create a new version rather than mutating the published artifact.

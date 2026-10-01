# Production Bible

## Objective

The Vertical Novel Factory must behave like a professional screen-production pipeline adapted to vertical episodic storytelling.

The target is not "AI-looking content". The target is a coherent audiovisual production in which the audience can follow the same characters, world, voices, camera language, lighting logic and visual identity from shot to shot.

## Non-negotiable rules

### Character Identity Lock

A canonical character has a locked identity.

The following attributes MUST remain stable unless the script explicitly establishes a change:

- face geometry
- facial proportions
- eyes, nose, mouth and jaw
- skin tone and texture
- age appearance
- body proportions
- height/build
- hair color, haircut and hairline
- permanent marks, scars, tattoos and distinguishing features
- accessories defined as permanent
- baseline wardrobe when continuity requires it

A scene change, camera angle, lighting change, location change or generation pass MUST NOT silently modify the character.

Any identity drift is a continuity failure.

### Expression Lock

Facial expression may change because the performance changes. Facial identity may not.

Allowed:
- smile
- fear
- anger
- crying
- surprise
- subtle emotional variation

Forbidden:
- a different face caused by generation drift
- changing age
- changing facial structure
- changing eye shape
- changing ethnicity/skin characteristics
- unexplained hairstyle or permanent-feature changes

### Voice Lock

Every speaking character has one canonical voice identity.

The voice must remain consistent in:

- speaker identity
- vocal age
- perceived sex/gender when canonically defined
- accent
- language
- timbre
- pitch range
- speaking style
- pronunciation
- emotional performance

Emotion may change. The underlying voice identity may not.

The system must prefer one reproducible voice pipeline per character. Do not randomly regenerate or switch voice models between scenes.

If a voice model cannot maintain identity reliably, the shot fails QA rather than silently accepting a different voice.

## Cinematography

Every shot receives an explicit Shot Spec.

Required cinematography fields include:

- shot size
- camera position
- camera height
- lens/FOV target
- focal relationship
- camera movement
- subject blocking
- screen direction
- composition
- depth of field
- focus target
- lighting direction
- lighting quality
- color temperature
- exposure intent
- foreground/midground/background
- transition relationship with previous and next shot

### Shot vocabulary

Use conventional cinematic terminology:

- EWS / extreme wide
- WS / wide
- MS / medium
- MCU / medium close-up
- CU / close-up
- ECU / extreme close-up
- OTS / over-the-shoulder
- POV
- two-shot
- insert
- cutaway

### Composition

Composition must be intentional, not merely aesthetically pleasing.

The director system must consider:

- rule of thirds when appropriate
- headroom
- lead room
- look room
- eyeline
- negative space
- visual hierarchy
- foreground obstruction
- depth
- subject separation
- vertical safe areas for platform UI

## Continuity

Continuity is tracked across:

- character identity
- wardrobe
- hair
- makeup
- accessories
- props
- injuries
- emotional state
- body position
- screen direction
- eyelines
- time of day
- weather
- lighting
- location geography
- object placement
- dialogue facts
- chronology

### 180-degree rule

The production system should preserve screen direction and the 180-degree axis unless an intentional crossing is specified by the director.

### Match cuts and movement

When a shot cuts to another:

- movement should match when intended
- eyelines should make spatial sense
- hand/object positions should not jump without narrative cause
- screen direction should remain coherent
- lighting should remain compatible

## Lighting

Lighting is part of the visual identity.

Each location receives a lighting profile containing:

- key source
- fill level
- back/rim source
- practical lights
- color temperature
- contrast ratio target
- time-of-day profile
- mood
- motivated-lighting rationale

Lighting changes must have a narrative or environmental reason.

## Color

The production maintains a consistent color language.

The color system must define:

- palette
- contrast strategy
- skin-tone treatment
- saturation target
- highlight behavior
- shadow behavior
- scene-specific deviations
- final grade/look reference

Color grading must not be used to hide identity or generation defects.

## Image quality

Production assets should be generated at the highest practical quality supported by the selected model and hardware.

The pipeline should preserve quality through:

- high-resolution source generation
- high-quality references
- controlled upscaling where necessary
- minimal unnecessary recompression
- high-quality intermediate formats
- final mastering at the target delivery resolution

The production must distinguish between generation resolution and delivery resolution.

## Vertical cinematography

Master delivery:

- 1080x1920
- 9:16
- platform-safe composition

Important visual information must remain inside safe areas so that TikTok/YouTube interface elements do not cover faces, subtitles or narrative objects.

Vertical framing must be designed during cinematography, not obtained by blindly cropping a horizontal composition.

## Editing language

The editor follows the script and Shot Specs.

The system should define:

- cut points
- shot duration
- transition type
- pacing
- reaction timing
- dialogue overlap
- J-cuts
- L-cuts
- montage logic
- music entry/exit
- SFX synchronization

Transitions must have a reason. Avoid decorative transitions that compete with the story.

## Sound

Sound is treated as a production layer, not an afterthought.

Each scene may contain:

- dialogue
- room tone
- ambience
- Foley
- sound effects
- music
- transitions
- silence

Dialogue must remain intelligible above music and ambience.

Voice processing must preserve the canonical character voice instead of making it sound artificially processed.

## Performance direction

Characters must have consistent acting logic.

The system should specify:

- objective
- emotional state
- subtext
- intensity
- gesture intent
- gaze
- body language
- timing

Expression changes are performance changes, not identity changes.

## Professional review gates

Before an episode is considered READY, review:

1. Story continuity
2. Character identity
3. Voice identity
4. Acting/performance
5. Cinematography
6. Composition
7. Lighting
8. Color
9. Motion quality
10. Edit rhythm
11. Dialogue intelligibility
12. Sound design
13. Subtitle accuracy
14. Technical encoding
15. Rights/provenance

Any BLOCKER prevents release.

# EP001 Video Generation Plan

## Production path

Approved canonical character references
→ keyframe generation
→ ComfyUI image-to-video
→ Wan2.2 short-shot generation
→ temporal/identity QA
→ approved shots
→ edit

## Model candidate

Wan2.2 TI2V-5B / I2V workflow is the first local candidate because the project requires free/local generation. The exact checkpoint license must be verified and recorded before commercial publication.

## Important constraint

GitHub stores the canonical production specifications and provenance. It is not itself the GPU video renderer. The actual rendering runtime is ComfyUI running locally or on a separately approved compute environment.

## EP001

Generate one short shot at a time from an approved keyframe. Do not generate the whole episode as one continuous clip.

### Identity references

- Miguel: approved canonical reference from current production session.
- Daniel: approved canonical reference from current production session.

### Scene constraint

At the 2020 freshman reception:
- Miguel and Daniel do not speak.
- They do not introduce themselves.
- They do not exchange contact information.
- They do not follow each other on Instagram.
- They only notice each other and exchange looks.
- Their friend groups remain separate.

## Target master

1080x1920, 9:16, 24 fps.

## QA blockers

- face drift
- body drift
- hair drift
- wardrobe drift
- age drift
- crowd morphing
- unnatural hands
- temporal flicker
- unintended dialogue
- incorrect chronology

## Cost

No paid API, subscription, cloud GPU, or metered service may be activated without explicit approval.

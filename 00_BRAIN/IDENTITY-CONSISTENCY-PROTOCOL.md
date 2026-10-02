# Identity Consistency Protocol

## ABSOLUTE RULE

A character reference sheet is invalid if any panel changes the canonical character's identity.

This includes:

- face geometry
- facial proportions
- skin tone
- skin undertone
- eye shape/color
- nose
- lips
- jaw
- hair color
- hair texture
- hairline
- apparent age
- body proportions
- permanent marks
- tattoos/scars
- canonical accessories

## Wardrobe continuity

A reference sheet must not mix wardrobe states unless each state is explicitly labeled as a separate approved continuity state.

For a baseline reference sheet, the same canonical outfit must be used across identity angles.

Different outfits belong in a separate wardrobe sheet and must still preserve the exact same person.

## Expression continuity

Expressions may change.

Identity may not.

Natural expression changes include:

- smile
- sadness
- anger
- fear
- surprise
- fatigue
- concentration
- crying

The expression must deform the same facial structure rather than generate a new face.

## Color continuity

Skin, hair and eye color must remain consistent.

Lighting can change perceived luminance and shadow, but must not produce unexplained changes in underlying skin tone.

## Reference generation rule

Do not generate all reference panels independently from text.

Preferred sequence:

MASTER PORTRAIT
→ identity anchor
→ controlled view transformation
→ identity comparison
→ approval
→ next reference

If the generation system cannot preserve identity, the workflow is rejected or changed.

## Sheet QA

A sheet is BLOCKED when any panel shows:

- a different face
- different skin tone
- different hair identity
- different age
- different body
- unexplained clothing change
- inconsistent permanent feature

A beautiful sheet with inconsistent identity is still a failed sheet.

## Canonical asset rule

Only individually approved assets become canonical.

A composite sheet is a presentation artifact, not proof that all panels are consistent.

Each canonical reference must have its own asset ID and QA status.


## Single-character generation rule

Canonical character production must generate ONE character at a time.

Do not use multi-character composite sheets as canonical identity sources.

A composite board may be used only as a non-canonical mood/reference artifact. Every character must receive an isolated master identity asset and isolated QA.

If a generation produces an unexpected character name, multiple characters, or a different approved identity, the output is automatically NON-CANONICAL.

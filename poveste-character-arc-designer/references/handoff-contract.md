# Mat Pocock Handoff Contract

## Purpose

Prepare an approved story package for Mat Pocock's handoff skill.

The handoff skill is required before the Writing Beats skill.

Do not directly invoke or imitate the Writing Beats skill.

## Ready status

Use:

```text
HANDOFF STATUS: READY
```

Only when:

- The target age is approved.
- The central idea is clear.
- The protagonist has agency.
- The ending is emotionally safe.
- Major guideline conflicts are resolved.
- Keyframes are consistent.
- Approved proposals are distinguished from flexible material.

If these conditions are not met:

```text
HANDOFF STATUS: BLOCKED
```

## Handoff package

```yaml
story_handoff:
  canon:
    premise:
    central_what_if:
    target_age:
    target_word_count:
    tone:
    theme:
    setting:
    fixed_keyframes:
    approved_ending:

  approved_proposals:
    protagonist:
    opposing_force:
    supporting_characters:
    character_arcs:
    intermediate_events:
    scene_sequence:
    split_structure:

  flexible_material:
    - Minor transitional actions
    - Natural Romanian dialogue
    - Sensory details
    - Scene-level expansion

  protected_constraints:
    - Preserve the target age.
    - Keep conflict bedtime-safe.
    - Preserve protagonist agency.
    - Preserve the approved ending.
    - Use concise, natural Romanian.
    - Do not add unnecessary major characters.
    - Do not contradict canon.

  approved_exceptions:
    - 

  unresolved:
    - 
```

## Invocation

When the package is ready:

1. Set `HANDOFF STATUS: READY`.
2. Invoke the installed Mat Pocock handoff skill.
3. Pass the complete `story_handoff` package.
4. Do not invoke Writing Beats directly.
5. Do not write detailed beats before the handoff skill processes the package.

Use the configured Mat Pocock skill identifier when available. If no identifier
is configured, use:

```text
mat-pocock-handoff
```

If the skill is unavailable, report:

```text
HANDOFF STATUS: BLOCKED

Mat Pocock's handoff skill is not installed or its identifier is unknown.
```

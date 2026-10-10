---
name: poveste-split-story
description: >
  Split an overly long Romanian bedtime story into connected parts or chapters.
  Use when a story needs multiple reading sessions. Give Part 1 a meaningful
  local resolution, a safe ending, and a calm continuation hook. Preserve
  continuity for later parts and challenge splits that create anxiety, repetition,
  weak pacing, or unresolved frightening danger.
---

# Split Story

Read these references before working:

- `references/story-guidelines.md`
- `references/concise-romanian-style.md`
- `references/handoff-contract.md`

## Role

Split a story only when it is genuinely too long or structurally complex for one
bedtime reading.

Each part must feel meaningful and emotionally safe.

## Core rules

- Preserve the central idea, protagonist, arc, and final resolution.
- Give each part a local goal.
- Give each part an obstacle and meaningful change.
- Part 1 must resolve a local problem.
- Part 1 must end with calm curiosity, not fear.
- Part 2 must continue from established information.
- The protagonist must remain central.
- Avoid repetition.
- Keep the target age and language consistent.
- Do not split only to reach a word count.

## Challenge unsuitable splits

Challenge the request when:

- Part 1 has no meaningful resolution.
- Part 1 ends with unresolved frightening danger.
- Part 2 requires information not prepared in Part 1.
- One part is too short to feel substantial.
- The split creates unnecessary repetition.
- The target age cannot comfortably follow the extended structure.
- The split avoids resolving the central problem.
- The hook is manipulative rather than calmly curious.

Use:

```markdown
## GUIDELINE CONFLICT

**Requested split:**  
[Describe it.]

**Conflict:**  
[Name the relevant guideline.]

**Why it matters:**  
[Explain briefly.]

**Recommendation:**  
[Suggest a better split.]

**Decision required:**  
[Ask one focused question.]
```

## When to recommend splitting

Consider a split when:

- The story exceeds the target age's recommended length.
- It has two clearly different phases.
- The protagonist enters a new location, relationship, or problem.
- It contains a natural midpoint.
- One reading would be too demanding.
- A safe pause can create calm curiosity.

## Input

```yaml
story_type: outline | beat_plan | draft
story:
target_age:
target_word_count:
desired_number_of_parts:
known_ending:
must_preserve:
```

## Analysis

```yaml
story_analysis:
  current_word_count:
  estimated_reading_time:
  target_age:
  central_what_if:
  protagonist:
  central_desire:
  external_problem:
  internal_problem:
  major_keyframes:
  midpoint_candidates:
  final_resolution:
  emotional_arc:
```

Return one:

```text
SPLIT RECOMMENDATION:
- KEEP_AS_ONE_STORY
- SPLIT_INTO_TWO_PARTS
- SPLIT_INTO_MORE_PARTS
- NEEDS_AUTHOR_DECISION
```

## Split point

Choose a point after:

- A local goal is completed.
- A first problem is resolved.
- A new phase begins.
- A meaningful discovery changes the direction.
- The protagonist makes a decision beginning the next phase.

Avoid splitting during frightening danger or before the central problem is clear.

```yaml
split_point:
  after_keyframe:
  after_scene_or_beat:
  reason:
  resolved_local_problem:
  new_question:
  emotional_state:
```

## Part structure

```yaml
part:
  number:
  title:
  purpose:
  local_goal:
  local_problem:
  key_events:
  turning_point:
  meaningful_change:
  resolved_elements:
  unresolved_elements:
  emotional_start:
  emotional_end:
  approximate_word_count:
  approximate_reading_time:
```

## Part 1 ending

Part 1 must have:

- A local resolution
- A protagonist choice
- A visible change
- A calming image
- A gentle continuation question
- Reassurance of safety

```yaml
part_1_ending:
  local_resolution:
  protagonist_choice:
  visible_change:
  calming_image:
  continuation_question:
  safety_reassurance:
```

Good hook:

```text
Acasă, Luna observă că frunza argintie din buzunar începe să strălucească.
```

Avoid:

```text
O umbră se mișcă la fereastră. Luna nu știe ce o așteaptă.
```

## Continuity bridge

```yaml
continuity_bridge:
  time_transition:
  location_transition:
  protagonist_state:
  supporting_character_state:
  opposing_force_state:
  known_information:
  unknown_information:
  objects_in_play:
  promises_to_pay_off:
  relationships:
  unresolved_question:
  emotional_thread:
  recurring_image:
```

Track knowledge:

```yaml
knowledge_state:
  protagonist_knows:
    - 
  protagonist_does_not_know:
    - 
  supporting_characters_know:
    - 
  reader_knows:
    - 
```

## Part 2

Part 2 should:

- Briefly reconnect the listener.
- Establish the current goal.
- Use the continuity bridge.
- Escalate gently.
- Lead to the final meaningful choice.
- Resolve the central problem.
- End with warmth, safety, rest, or belonging.

Do not repeat the entire previous part.

## Multiple parts

For each non-final part:

```yaml
part:
  number:
  local_goal:
  local_obstacle:
  local_resolution:
  meaningful_change:
  safe_pause:
  continuation_question:
```

## Handoff package

```yaml
split_handoff:
  overall_story:
    central_what_if:
    target_age:
    total_parts:
    theme:
    final_resolution:

  parts:
    - number:
      title:
      local_goal:
      local_problem:
      fixed_keyframes:
      proposed_transitions:
      turning_point:
      local_resolution:
      ending_image:
      continuation_question:
      continuity_to_next_part:

  protected_constraints:
    - Preserve the protagonist's agency.
    - Keep the conflict bedtime-safe.
    - Give each part a meaningful local resolution.
    - Use concise, natural Romanian.
    - Resolve the overall story in the final part.

  approved_exceptions:
    - 

  unresolved:
    - 
```

## Validation

```markdown
- [ ] The story genuinely benefits from splitting.
- [ ] Each part has a local goal.
- [ ] Each part has an obstacle.
- [ ] Each part has a meaningful change.
- [ ] Part 1 resolves something important.
- [ ] Part 1 ends safely.
- [ ] The hook creates calm curiosity.
- [ ] Part 2 has clear continuity.
- [ ] Knowledge remains consistent.
- [ ] The protagonist remains active.
- [ ] The overall problem is resolved.
- [ ] The final part ends calmly.
- [ ] Repetition is limited.
```

## Final transfer

When the split plan is approved:

1. Set `HANDOFF STATUS: READY`.
2. Invoke Mat Pocock's handoff skill for each approved part.
3. Preserve the continuity bridge.
4. Do not invoke Writing Beats directly.
5. Do not merge the parts.
6. Do not invent a new central conflict.
7. If the handoff skill is unavailable, report `HANDOFF STATUS: BLOCKED`.

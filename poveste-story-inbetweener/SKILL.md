---
name: poveste-story-inbetweener
description: >
  Fill the causal gaps between major story keyframes for Romanian bedtime
  stories. Use when the user has important story moments but needs obstacles,
  discoveries, scene transitions, emotional progression, turning points, and
  continuity. Preserve canon, avoid filler, keep conflict bedtime-safe, and
  prepare a compact package for Mat Pocock's handoff skill.
---

# Story Inbetweener

Read these references before working:

- `references/story-guidelines.md`
- `references/concise-romanian-style.md`
- `references/handoff-contract.md`

## Role

The user provides the keyframes. Create purposeful transitions between them.

Do not change confirmed keyframes. Do not write full prose unless requested.

## Core rules

- Preserve `CANON`.
- Label inventions as `PROPOSED`.
- Build cause and effect.
- Use:

```text
character goal → obstacle → changed situation
```

- Every event must have a story function.
- The protagonist must remain active.
- Supporting characters may help but may not solve the central problem.
- Use two or three obstacles for a typical bedtime story.
- Escalate gently.
- End transitions with safety and calm.
- Avoid filler.
- Keep plans concise.

## Challenge conflicts

Challenge the keyframes when connecting them would require:

- Graphic or overwhelming danger
- An unresolved frightening threat
- A sudden personality change
- A deus ex machina
- A solution unrelated to the protagonist's actions
- Too many characters or locations
- Events without causal connection
- A middle more intense than the ending can safely resolve

Use:

```markdown
## GUIDELINE CONFLICT

**Author's idea:**  
[State it accurately.]

**Conflict:**  
[Name the relevant guideline.]

**Why it matters:**  
[Explain briefly.]

**Recommendation:**  
[Offer the smallest useful adjustment.]

**Decision required:**  
[Ask one focused question.]
```

## Input

```yaml
fixed_keyframes:
  - 

known_characters:
  - 

target_age:
tone:
theme:
approved_ending:
constraints:
```

## Gap analysis

For each gap:

```yaml
gap:
  from:
  to:
  starting_state:
    protagonist_knows:
    protagonist_wants:
    protagonist_feels:
    available_resources:

  destination_requirements:
    facts_that_must_be_true:
    information_required:
    emotional_change_required:
    decision_required:

  missing_links:
    - 
```

Do not propose an event until its purpose is clear.

## Intermediate events

```yaml
event:
  title:
  goal:
  obstacle:
  action:
  result:
  changed_situation:
  information_revealed:
  emotional_shift:
  relationship_change:
  story_function:
```

Keep ordinary events to one or two concise sentences. Expand only turning points,
emotional choices, or continuity-critical events.

Delete events that do not change plot, character, relationship, knowledge, stakes,
or theme.

## Scene candidates

```yaml
scene:
  number:
  purpose:
  location:
  characters:
  local_goal:
  obstacle:
  key_action:
  changed_situation:
  sensory_anchor:
  emotional_beat:
  transition:
```

## Turning point

```yaml
turning_point:
  failed_usual_strategy:
  new_understanding:
  meaningful_choice:
  immediate_consequence:
  connection_to_resolution:
```

The important choice must belong to the protagonist.

## Ending transition

```yaml
ending:
  external_resolution:
  emotional_resolution:
  visible_change:
  relationship_result:
  calming_image:
  final_bedtime_feeling:
```

## Continuity check

```markdown
- [ ] The protagonist knows enough to act.
- [ ] Each event causes or enables the next.
- [ ] The opposing force behaves consistently.
- [ ] Relationships change plausibly.
- [ ] No event is filler.
- [ ] The protagonist remains central.
- [ ] The conflict remains bedtime-safe.
- [ ] The ending becomes calmer.
```

## Output

Return:

```markdown
# BEAT HANDOFF PREPARATION

## Fixed keyframes

## Proposed intermediate events

## Proposed scene sequence

## Emotional progression

## Required discoveries

## Turning point

## Meaningful choice

## Ending transition

## Continuity checks

## Unresolved decisions
```

When complete and approved:

1. Set `HANDOFF STATUS: READY`.
2. Build the package defined in `references/handoff-contract.md`.
3. Invoke Mat Pocock's handoff skill.
4. Do not invoke Writing Beats directly.
5. If the handoff skill is unavailable, report `HANDOFF STATUS: BLOCKED`.

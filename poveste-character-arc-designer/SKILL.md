---
name: poveste-character-arc-designer
description: >
  Design concise, believable, age-appropriate character arcs for Romanian
  bedtime stories. Use when the protagonist, opposing force, or supporting cast
  needs clear desires, fears, strengths, relationships, meaningful choices, and
  visible emotional change. Challenge arcs that remove protagonist agency,
  overload the cast, or create unsafe conflict.
---

# Character Arc Designer

Read these references before working:

- `references/story-guidelines.md`
- `references/concise-romanian-style.md`
- `references/handoff-contract.md`

## Role

Design small, visible, believable character changes suitable for bedtime
listening.

The protagonist receives the main arc. Supporting characters should have only the
change required by the story.

## Core principles

- The protagonist remains central.
- The protagonist contributes to the solution.
- Another character may help but must not solve the central problem.
- The internal problem connects to the external problem.
- Character change is appropriately small.
- Only necessary supporting characters are used.
- Change is shown through action, behavior, or image.
- A villain is optional.
- Conflict remains emotionally safe.

## Challenge conflicts

Challenge the input when:

- The protagonist has no meaningful choice.
- Another character solves the entire problem.
- The internal and external problems are unrelated.
- The change is too large to be believable.
- The cast is too large for the story's length.
- Characters duplicate each other's functions.
- An antagonist is excessively frightening, cruel, or humiliating.
- The lesson is delivered as a lecture instead of discovered through action.

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

## Protagonist template

```yaml
protagonist:
  name:
  role_or_species:
  desire:
  external_problem:
  internal_problem:
  limiting_belief_or_fear:
  strength:
  weakness_or_habit:
  starting_emotion:
  meaningful_choice:
  realization:
  ending_emotion:
  visible_change:
```

## Arc sequence

```yaml
arc:
  starting_state:
  limiting_belief:
  desire:
  first_strategy:
  consequence:
  growing_pressure:
  realization:
  meaningful_choice:
  resolution:
  ending_state:
```

Use:

```text
limiting belief → problem → usual strategy → failure
→ realization → meaningful choice → visible change
```

The change must be believable for the target age.

## Opposing force

A villain is not required. Consider:

- Fear
- Mistake
- Misunderstanding
- Practical obstacle
- Nature
- Waiting
- Rival
- Worried character
- Antagonist

If an opposing character is needed:

```yaml
opposing_character:
  name:
  role_or_species:
  visible_goal:
  deeper_motivation:
  fear_or_need:
  mistaken_belief:
  relationship_to_protagonist:
  pressure_method:
  redeeming_quality:
  emotional_safety_notes:
  possible_change:
```

The opposing character should have understandable motivations and should not
create unresolved fear for a young listener.

## Supporting character template

```yaml
supporting_character:
  name:
  role_or_species:
  story_function:
  desire:
  relationship_to_protagonist:
  help_or_challenge:
  information:
  emotional_effect:
  limitation:
  change_by_the_end:
```

Each important supporting character must help, challenge, reflect another
perspective, provide information, offer humor, need help, alter the atmosphere,
or make the protagonist's choice possible.

## Relationship map

```text
Character A → Character B
- Surface relationship:
- Underlying tension:
- What A wants:
- What B wants:
- What changes:
```

## Agency check

```markdown
AGENCY CHECK

- [ ] The protagonist experiences the central problem.
- [ ] The protagonist attempts a solution.
- [ ] The initial strategy is understandable.
- [ ] The strategy is insufficient.
- [ ] The protagonist learns something.
- [ ] The protagonist makes the decisive choice.
- [ ] The choice contributes directly to the resolution.
- [ ] The ending shows a visible change.
```

If an essential item fails:

```text
CHARACTER ARC STATUS: NEEDS_RESTRUCTURING
```

## Character function audit

For each important character, ask:

- Why is this character needed?
- What would be lost if they were removed?
- What do they change?
- Are they distinct?
- Is the cast manageable for the target age?

## Output format

```markdown
### Character: [Name]

- **Role:**
- **Wants:**
- **Problem:**
- **Fear or false belief:**
- **Strength:**
- **Choice:**
- **Change:**
- **Story function:**
```

When approved:

1. Prepare the character information for the Mat Pocock handoff.
2. Do not invoke Writing Beats directly.
3. If the handoff skill is unavailable, report `HANDOFF STATUS: BLOCKED`.

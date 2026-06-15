# Presentation Planning Engine

The Presentation Planning Engine converts a presentation request into an ordered slide structure.
It does not generate final slide copy and must not invent unsupported InfoClub facts.

## Input Contract

```yaml
presentation_type: partner
audience: startup founders
goal: introduce InfoClub ecosystem
slides_count: 12
language: ru
```

## Output Contract

```yaml
presentation:
  - slide: 1
    title: InfoClub
    purpose: introduction
  - slide: 2
    title: Community Mission
    purpose: context
  - slide: 3
    title: Value Proposition
    purpose: benefits
```

## Planning Steps

1. Read the presentation request fields.
2. Select the matching presentation type template.
3. Match the audience to the audience knowledge profile.
4. Select a slide sequence that fits `slides_count`.
5. Assign each slide a title and purpose.
6. Keep unknown or unverified facts out of the plan.
7. Return the `presentation` list as the planning artifact.

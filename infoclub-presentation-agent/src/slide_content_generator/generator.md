# Slide Content Generator

The Slide Content Generator fills a planned slide with structured content.
It receives a slide plan entry and returns a slide title plus content bullets.
It must use the knowledge layer and claim constraints before adding any factual statement.

## Input Contract

```yaml
slide:
  title: Community Mission
```

## Output Contract

```yaml
title: Mission of InfoClub
content:
  - State the verified InfoClub mission, or mark the mission as verification required.
  - Explain why the mission matters to the selected audience.
  - Connect the mission to the presentation goal without adding unsupported facts.
```

## Generation Steps

1. Read the planned slide title and purpose when available.
2. Select relevant knowledge for the slide topic.
3. Check `claims_and_constraints.md` before writing factual content.
4. Rewrite the slide title for presentation clarity.
5. Generate concise content bullets.
6. Mark unknown or unverified facts as verification required.
7. Return `title` and `content` only.

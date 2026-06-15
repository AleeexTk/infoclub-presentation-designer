# Planning Rules

## Required Inputs

- `presentation_type`
- `audience`
- `goal`
- `slides_count`
- `language`

## Output Rules

- The output must contain a top-level `presentation` list.
- Each slide entry must include `slide`, `title`, and `purpose`.
- Slide numbers must start at `1` and increase by `1`.
- The number of slide entries should match `slides_count` when enough planning context exists.
- Titles must describe the planned slide topic, not final slide copy.
- Purposes must describe the role of the slide in the presentation flow.

## Knowledge Rules

- Use the knowledge layer as the source of truth for InfoClub facts.
- Use `claims_and_constraints.md` before including factual assumptions in a plan.
- Do not invent metrics, partner names, sponsor names, investor claims, services, events, or outcomes.
- If required knowledge is unknown, create a generic planning placeholder instead of a factual claim.

## Language Rules

- Preserve the requested `language` for generated titles when possible.
- If the requested language is unsupported by available templates, keep the plan structurally valid and mark language adaptation as required.

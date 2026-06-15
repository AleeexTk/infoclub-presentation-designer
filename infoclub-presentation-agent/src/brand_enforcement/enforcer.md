# Brand Enforcement Layer

The Brand Enforcement Layer applies InfoClub brand rules to generated presentation content.
It receives presentation content, reads the `brand/` sources, and returns a branded presentation draft.

## Formula

```text
Presentation Content
+
Brand Rules
=
Branded Presentation Draft
```

## Inputs

- Presentation content from the slide content generator.
- Brand guide from `brand/brand_guide.md`.
- Color rules from `brand/colors.md`.
- Typography rules from `brand/typography.md`.
- Presentation rules from `brand/presentation_rules.md`.

## Output

```yaml
branded_presentation_draft:
  slides:
    - title: Mission of InfoClub
      content:
        - State the verified InfoClub mission, or mark the mission as verification required.
      brand_applied:
        guide: true
        colors: true
        typography: true
        presentation_rules: true
```

## Enforcement Steps

1. Read the generated presentation content.
2. Load the active brand files from `brand/`.
3. Apply presentation structure rules.
4. Apply typography and color guidance when available.
5. Preserve claim constraints and verification markers.
6. Return the branded presentation draft.

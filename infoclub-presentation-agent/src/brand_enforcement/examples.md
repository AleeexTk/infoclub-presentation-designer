# Brand Enforcement Examples

## Input

```yaml
presentation_content:
  slides:
    - title: Mission of InfoClub
      content:
        - State the verified InfoClub mission, or mark the mission as verification required.
```

## Brand Sources

```yaml
brand:
  guide: brand/brand_guide.md
  colors: brand/colors.md
  typography: brand/typography.md
  presentation_rules: brand/presentation_rules.md
```

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

## Notes

- Brand enforcement changes presentation form, not factual substance.
- Verification markers remain in the branded draft until approved knowledge sources resolve them.

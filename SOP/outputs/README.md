# Output Naming Policy

Generated workbook exports live in this directory.

Use this pattern:

`{estimate-name}-{version}.xlsx`

Examples:
- `lockly-smart-lock-estimate-v1.xlsx`
- `parcel-fulfillment-baseline-v2.xlsx`

Rules:
- Keep the structured JSON estimate that produced the workbook in the repo.
- Treat the workbook as an export, not the source of truth.
- Regenerate the workbook when the estimate changes materially.
- Use workbook exports for finance review, comparison, and downstream modeling.

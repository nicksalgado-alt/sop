# Cost Model

This workspace estimates true unit cost by operational step.

## Core Question

For a given product, condition path, and fulfillment context:
- how long does each step take,
- what labor and materials are required,
- what fallout or yield risk exists,
- and what is the resulting unit cost?

## Step Library

The initial step library covers:
- receive a unit,
- inspect as new,
- refurbish as sellable used,
- inspect as damaged,
- refurbish as defective,
- fulfillment,
- pick and pack for bulk,
- pick and pack for parcel,
- storage.

Not every estimate needs every step. Claude should choose the relevant path, explain why, and show any missing branches.

## Required Reasoning

Each estimate should identify:
- the product or category,
- the expected condition mix,
- the selected process path,
- the volume assumption,
- the labor rate assumption,
- any material or parts assumptions,
- any fallout, scrap, or rework risk,
- and any uncertainty that could materially change the result.

## Cost Logic

Per-step cost should be reasoned from:

`step_cost = labor_cost + parts_cost + handling_cost + storage_cost + fallout_adjustment`

Where:
- `labor_cost = labor_minutes / 60 * labor_rate_per_hour`
- `parts_cost` includes direct refurb or consumable inputs
- `handling_cost` includes equipment, packaging, or step-specific overhead proxies
- `storage_cost` is applied when inventory dwell time matters
- `fallout_adjustment` captures expected loss, rework, or defective conversion impact

## Output Expectations

A good estimate includes:
- per-step time assumptions,
- per-step unit cost,
- total unit cost,
- sensitivity notes,
- open questions,
- and confidence levels.

## Decomposition Rule (MANDATORY)

**Never nest cost components inside a single formula or cell.** Every cost
component must be in its own column, visible and auditable on the face of the
sheet. The required columns for every step row in a workbook are:

| Column | Content | Type |
|--------|---------|------|
| Labor Min | Minutes of labor for this step | Input (blue) |
| Labor $/hr | Hourly rate (ref to Assumptions) | Reference (green) |
| Labor $ | = Labor Min / 60 × Labor $/hr | Formula (black) |
| Parts $ | Direct parts or consumable cost | Input (blue) |
| Handling $ | Equipment, packaging, overhead | Input (blue) |
| Fallout $ | Expected loss, rework, defective conversion | Input (blue) |
| Total $/Unit | = Labor + Parts + Handling + Fallout | Formula (black) |

This means:
- No `=(3/60)*35+0.35+0.20` style formulas. Ever.
- Each number lives in one cell. The total is always a SUM of visible cells.
- Anyone reading the sheet can challenge any single assumption without
  reverse-engineering a formula.
- Blue = direct input (editable). Black = formula. Green = cross-sheet ref.

This rule applies to all workbook outputs — rate cards, SOPs, estimates,
financial models. No exceptions.

## Confidence Model

Claude should classify confidence per step as:
- `high`: directly supported by SOPs, accepted benchmarks, or recent cases
- `medium`: partly benchmarked, partly assumed
- `low`: mostly inferred from limited context

## Downstream Use

The structured estimate should be easy to:
- export to Excel,
- compare against prior cases,
- revise after review,
- and reuse in future financial models.

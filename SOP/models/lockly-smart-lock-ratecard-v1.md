# Lockly Smart Lock Rate Card & SOP v1

Full rate card workbook modeled after the NextSense format, with Lockly-specific assumptions.

## Key Numbers

- **Blended avg cost per unit: $10.19**
- NTF path (25% of returns): $5.41/unit
- Grade A/B/C refurb path (45%): $15.76/unit
- Hard Fail/BER path (20% + 10% damaged routed here): $8.71/unit
- Labor rate: $35/hr (user-provided)
- Monthly volume: 1,500 units (18,000/year)

## Assumptions Basis

- Volume estimated from first principles: ~1.5% of $3.3B smart lock market at ~$300 weighted ASP = ~180K units/year sold, 10% return rate = 18K returns
- Condition mix: 25% NTF (higher than avg due to installation returns), 45% refurb, 20% hard fail/BER, 10% damaged inspection
- Step costs use Nok smart-lock category overrides at $35/hr
- Defective parts cost: $12/unit (user-validated from prior estimate revision)

## Confidence

Medium. Benchmark-backed with smart-lock category overrides. Refurb and defective paths have highest uncertainty. Recommend 50-unit pilot to validate.

## Source Files

- Workbook: `Lockly_Rate_Card_SOP_v1.xlsx` (saved to user's Documents/Claude)
- Reference format: NextSense_Financial_Model_v2.xlsx (Rate Card & SOP tab)
- Prior estimate: `examples/lockly-smart-lock-estimate.json`

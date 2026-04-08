# Lockly Smart Lock Rate Card & SOP v2 (Final)

## Pricing Tiers

| Path | Nok Price | Est. Cost | Margin | Margin % |
|------|-----------|-----------|--------|----------|
| Receive & Intake (all units) | $3.00 | $2.59 | $0.41 | 14% |
| NTF / Damaged (repack only) | $2.00 | $1.73 | $0.27 | 14% |
| Refurbishment (A/B/C) | $10.00 | $14.74 | -$4.74 | -47% |
| Defective / Hard Fail | $8.00 | $6.33 | $1.67 | 21% |

## Blended Unit Economics

- Blended Price: $10.56/unit
- Blended Cost: $12.23/unit
- Blended Margin: -$1.67/unit (-15.8%)
- **Platform fee ($7,500/mo) makes overall P&L positive**

## Monthly P&L (at 1,500 units/mo)

- Processing Revenue: $15,840
- Platform Fee: $7,500
- Total Revenue: $23,340
- Total Cost: $18,344
- Gross Profit: $4,996
- Gross Margin: 21.4%

## Key Insight

Refurb path is underwater at $10/unit — estimated cost is $14.74. This means the
platform fee and receive/defective margins subsidize refurb. This is viable if:
- Refurb cost estimate is conservatively high (likely — it's MEDIUM confidence benchmarks)
- Volume grows and fixed costs get amortized
- Nok also earns revenue share on resale proceeds (20% take rate)

The resale revenue share is not modeled in this rate card but would significantly
improve the economics — even at conservative resale prices, 20% of $115-$173/unit
recovered = $23-$35/unit in additional Nok revenue per refurbed unit.

## How We Got Here

Built through iterative back-and-forth:
1. Started with bottoms-up step-level costing from brain benchmarks
2. Built v1 rate card with nested formulas ($10.19 blended)
3. Analyzed Lockly Visage repack SOP video → validated NTF timing
4. Video revealed repack maps to refurb (not NTF), sealed units don't need repack
5. Decomposed all formulas into separate visible columns (mandatory brain rule now)
6. Flipped from bottoms-up to customer-facing pricing tiers ($3/$2/$10/$8)
7. Backed into margins with step-level detail as internal cost backup

## Confidence

- Receive: MEDIUM (benchmark)
- NTF/Damaged: HIGH (video-validated)
- Refurbishment: MEDIUM (benchmark — capture video next)
- Defective: LOW (inferred)

## Source Files

- Workbook: `Lockly_Rate_Card_SOP_v2.xlsx`
- Video SOP: `docs/process-notes/lockly-visage-repack-sop.md`
- v1 Reference: `models/lockly-smart-lock-ratecard-v1.md`

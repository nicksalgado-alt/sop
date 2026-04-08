# Lockly Smart Lock Rate Card & SOP v2 (Video-Validated)

Updated from v1 with real SOP data extracted from PGK728WRHK Repack Video (Lockly Visage).

## Key Numbers

- **Blended avg cost per unit: $12.92** (was $10.19 in v1)
- NTF path (25% of returns): $5.11/unit — ★ video-validated repack SOP
- Grade A/B/C refurb path (53%): $17.93/unit
- Hard Fail/BER path (22%): $9.72/unit
- Labor rate: $35/hr (user-provided)
- Monthly volume: 1,500 units (18,000/year)

## v2 Changes from v1

1. **NTF repack SOP is video-validated** — 5 granular steps extracted from training video, all HIGH confidence
2. **Lockly Visage added** to product table (PGK728WR, ~$350 MSRP, facial recognition)
3. **12-component checklist** documented from video (new tab in workbook)
4. **Condition mix adjusted** — Grade A 28% (was 30%), Hard Fail 14% (was 12%) due to Visage complexity
5. **100% of units now priced** — v1 only accounted for 90% (excluded damaged inspection path); v2 folds all paths into 3 buckets
6. **Activation Card flagged** as CRITICAL — unique QR per device, cannot commingle

## NTF Repack SOP (from video)

| Phase | Time (training) | Time (production) | Cost |
|-------|----------------|-------------------|------|
| Accessory Verification | 40 sec | ~26 sec | $0.44 |
| Accessory Tray Repack | 20 sec | ~13 sec | $0.21 |
| Retail Box Assembly | 30 sec | ~20 sec | $0.39 |
| Documentation & Close | 30 sec | ~20 sec | $0.34 |
| Shipping Prep | 27 sec | ~18 sec | $0.35 |
| **NTF Subtotal** | **2:27** | **~1:37** | **$1.73** |

## Confidence

- NTF path: **HIGH** — video-validated, step-level timing observed
- Refurb path: **MEDIUM** — benchmark-backed, no video yet
- Hard Fail path: **LOW** — inferred from category benchmarks

## Recommendations

1. **Capture refurb SOP video** next — that path drives 53% of volume and $17.93/unit cost
2. **Validate defective parts cost** ($12/unit assumed) with actual teardown data
3. **Run 50-unit pilot** to validate production steady-state timing
4. **Track activation card matching** as a KPI — mismatch = customer returns

## Source Files

- Workbook: `Lockly_Rate_Card_SOP_v2.xlsx` (saved to user's Documents/Claude)
- SOP Video: PGK728WRHK Repack Video.mp4 (2:37, no audio)
- Detailed SOP: `docs/process-notes/lockly-visage-repack-sop.md`
- v1 Reference: `models/lockly-smart-lock-ratecard-v1.md`

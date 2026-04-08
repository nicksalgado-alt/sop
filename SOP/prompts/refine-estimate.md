# Refine Estimate

Use this prompt after the user reviews a prior estimate and wants it improved.

## Read First

Read:
- the original estimate
- any review notes from the user
- `docs/estimation-playbook.md`
- `assumptions/default-benchmarks.yaml`
- relevant `docs/process-notes/`
- relevant files in `memory/` and `models/`

## Prompt

```text
You are revising an existing Nok estimate.

Your job is not to start over blindly. Your job is to preserve what is still useful, update what changed, and explain the impact.

Rules:
1. Compare the new feedback against the prior estimate.
2. Keep unchanged assumptions stable unless there is a strong reason to revise them.
3. Update the affected process steps and totals.
4. Explain what changed and why.
5. Surface any new uncertainty or contradiction.
6. Capture reusable lessons for future estimates.

Return:
- a short summary of what changed
- an updated structured JSON estimate
- a short list of lessons learned worth saving into memory
```

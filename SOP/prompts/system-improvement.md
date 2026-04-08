# System Improvement

Use this prompt when Claude should reflect on how the workspace can improve itself after an estimate or review cycle.

## Intent

The system should get smarter over time, but it should not drift silently.

## Prompt

```text
You are maintaining Nok's estimating brain.

Look at the latest estimate, the user feedback, and the current repo context.

Separate improvements into two groups:

1. Low-risk updates that are safe to apply automatically:
- save a lesson learned
- add a note to category knowledge
- store an accepted benchmark assumption
- create a brief estimate summary
- improve cross-references between files

2. High-risk updates that should be proposed for approval:
- changing core prompts
- changing benchmark policy
- restructuring schemas in a way that affects outputs
- changing governance or review behavior

For each proposed improvement:
- describe the change
- explain why it helps
- classify it as low-risk or high-risk
- point to the file that should change

Do not hide important system changes. Surface them clearly.
```

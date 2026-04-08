# Nok Estimating Brain

This repository is a Claude Cowork workspace for building operational pricing estimates.

The goal is not to lock Nok into a rigid template. The goal is to give your team an analyst-in-a-box that:
- reads SOPs, notes, and past estimates,
- asks smart follow-up questions,
- makes explicit assumptions when data is missing,
- produces step-level unit-cost estimates,
- remembers what worked,
- and gets better over time.

## How It Works

1. Open Claude Cowork in this repo.
2. Ask for an estimate in plain English.
3. Claude reads the context in `docs/`, `assumptions/`, `memory/`, and `models/`.
4. Claude asks for missing information or uses benchmark assumptions and labels them clearly.
5. Claude produces a structured cost model with step costs, total unit cost, sensitivity, and open questions.
6. You review the estimate, correct anything that feels off, and ask Claude to refine it.
7. The accepted estimate becomes part of the repo's growing memory.

## What Lives Here

- `docs/`: how Nok wants the estimating brain to think and reason
- `docs/process-notes/`: markdown notes, SOP excerpts, and category knowledge
- `schemas/`: lightweight structure for estimate inputs and outputs
- `assumptions/`: benchmark assumptions Claude can use when information is missing
- `prompts/`: Claude Cowork prompts for estimate creation, refinement, and self-improvement
- `memory/`: lessons learned, reusable reasoning, and update rules
- `examples/`: sample requests and structured outputs
- `models/`: accepted cost models you want to keep and reuse
- `scripts/`: export tools for finance-friendly workbooks
- `outputs/`: generated spreadsheet exports

## Quick Start

Create a virtual environment and install the export dependency:

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

Generate the sample workbook:

```bash
python3 scripts/generate_workbook.py \
  --input examples/lockly-smart-lock-estimate.json \
  --output outputs/lockly-smart-lock-estimate-v1.xlsx
```

## Design Principles

- Start with conversation, not rigid structure.
- Keep assumptions explicit and reviewable.
- Save reasoning, not just outputs.
- Let patterns emerge before formalizing them.
- Improve through feedback loops, not hidden drift.
- Stay useful for non-technical users.

## Self-Improvement

This repo is designed to improve with use.

Low-risk learning should happen automatically:
- saving estimate summaries,
- capturing accepted assumptions,
- storing lessons learned,
- and reorganizing knowledge for easier reuse.

Higher-risk changes should still be reviewable:
- core prompt rewrites,
- benchmark policy changes,
- schema changes that affect downstream finance output,
- and governance changes.

# AML Network Pretraining Lab

![Demo Screenshot](demo/screenshot.png)

## Overview

Pretrain graph representations on transaction networks to improve suspicious-entity detection with less labeled data.

## Real-world problem

- User: AML investigators and model risk teams
- Problem: AML teams rarely have enough labeled cases to train strong network models from scratch.
- Decision improved: Improve suspicious-entity prioritization using better network representations before case review.
- KPI target: Increase suspicious network recall while reducing manual review waste.

## Why this matters

This repo is positioned as a real product for a real team, not a framework-only demo. The goal is to show how research-backed AI, analytics, or graph systems become deployable workflows with docs, UI, screenshots, and business-facing outputs.

## Project profile

- Domain: Anti-Money Laundering
- Project type: `ml`
- Tags: aml, graph, self-supervised, fraud

## Workflow

1. Ingest the operational context for the user and case.
2. Score risk, quality, or opportunity using the project API.
3. Compare current signals against a business baseline.
4. Generate a recommendation or operator brief for the next step.

## Quick start

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python scripts/bootstrap_data.py
uvicorn src.app.main:app --host 0.0.0.0 --port 8000 --reload
```

Open `http://localhost:8000/` to use the interactive application.

## Key endpoints

- `GET /`
- `GET /health`
- `GET /bootstrap`
- `GET /project`
- `POST /score`
- `POST /analyze`
- `POST /query`
- `POST /recommend`

## Documentation

- [Architecture](docs/architecture.md)
- [Evaluation](docs/evaluation.md)
- [Runbook](docs/runbook.md)
- [Innovation memo](research/innovation_memo.md)
- [Upstream audit](research/upstream_audit.md)

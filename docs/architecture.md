# Architecture

## Problem framing

- User: AML investigators and model risk teams
- Problem: AML teams rarely have enough labeled cases to train strong network models from scratch.
- Decision: Improve suspicious-entity prioritization using better network representations before case review.

## System flow

1. A user submits case context, business signals, or a search question.
2. The API exposes scoring, analysis, and recommendation endpoints.
3. The web application turns those outputs into an operator-facing workflow.
4. Observability, docs, and runbooks make the project easier to evaluate and extend.

## Production posture

- Separate app, docs, demo, and data folders
- Container-ready packaging
- API endpoints for health and workflow actions
- Screenshot-ready demo surface
- Research and upstream audit artifacts included in-repo

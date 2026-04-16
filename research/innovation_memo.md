# Innovation memo

## Real-world reframing

The original repo shape was technically strong but too framework-first. This refactor repositions the project around a concrete user and decision:

- User: AML investigators and model risk teams
- Problem: AML teams rarely have enough labeled cases to train strong network models from scratch.
- Decision: Improve suspicious-entity prioritization using better network representations before case review.
- KPI target: Increase suspicious network recall while reducing manual review waste.

## What changed

- Reframed the title, summary, and domain around a real team and workflow
- Rewrote the UI copy and demo flow to support a real operational action
- Rewrote docs and social collateral to emphasize business value over tooling

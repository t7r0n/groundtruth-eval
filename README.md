# Groundtruth Eval

An open benchmark + harness that scores any context layer grounded analytics agent on natural language -> governed metric correctness, designed to make Kaelio the reference standard.

## Why This Exists

A semantic layer for agents product has one bet the company question: when the agent answers, was the answer correct against the governed definition? Kaelio's marketing copy says "metrics defined in five places, governed in none" (kaelio.com) - but the only artifact a buyer sees today is a homepage and a list of integrations.

## What It Builds

- Replays synthetic `semantic` and `layer` cases against the project's evidence rules.
- Scores `semantic_coverage`, `layer_risk`, and `agents_precision` so regressions are visible in CSV and JSON.
- Plants `semantic drift` and `layer gap` failures as negative controls.
- Writes citation-locked decision claims; unsupported claims fail verification.
- Exports a review dashboard and demo pack for `groundtruth-eval` without hosted services.

## Local Run

```bash
uv sync
uv run groundtruth-eval all
uv run pytest -q
uv run ruff check .
```

## Outputs

- `outputs/analysis.json`
- `outputs/scenario_report.csv`
- `outputs/decision_report.md`
- `outputs/evidence_packet.md`
- `outputs/dashboard.html`
- `outputs/demo_pack.zip`

## Sources

- https://www.kaelio.com/blog/best-ai-analytics-tools-for-healthcare-organizations
- https://www.kaelio.com/blog/best-semantic-layer-solutions-for-data-teams-2026-guide
- https://www.kaelio.com/blog/best-ai-analytics-tools-that-work-with-dbt-and-lookml
- https://www.ycombinator.com/companies/kaelio
- https://x.com/ycombinator/status/1924465068487667748
- https://www.linkedin.com/in/luca-martial/
- https://github.com/luca-martial
- https://github.com/JohnSnowLabs/spark-nlp
- https://github.com/Giskard-AI/giskard

## Boundary

This repository uses synthetic fixtures only. It has no credentials, no customer data, no outreach data, and no dependency on a hosted API.

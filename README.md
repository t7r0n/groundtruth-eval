# Groundtruth Eval

An open benchmark + harness that scores any context layer grounded analytics agent on natural language -> governed metric correctness, designed to make Kaelio the reference standard.

![Groundtruth Eval working dashboard](outputs/project_working.svg)

## Why it exists

A semantic layer for agents product has one bet the company question: when the agent answers, was the answer correct against the governed definition?

Most internal demos stop at a pretty chart. This repository is built around the harder part: a repeatable path from fixture, to failure, to evidence, to the operator action a serious team would actually trust.

## What is inside

- A deterministic replay harness tuned around semantic, layer, and agents.
- Company-specific strategy code in `src/groundtruth_eval/strategy.py`, not just README-level customization.
- Citation-locked reports where every decision claim has to point back to a generated evidence ID.
- Two visual artifacts generated from the latest run: `outputs/project_working.svg` and `outputs/evidence_map.svg`.
- A portable demo pack with JSON, CSV, Markdown, HTML, SVG, and benchmark artifacts.

![Groundtruth Eval evidence map](outputs/evidence_map.svg)

## Signals it measures

- `semantic coverage`
- `layer risk`
- `agents precision`
- `product latency`

## Failure modes it plants

- semantic drift
- layer gap
- agents misroute
- product blindspot

## Run it locally

```bash
uv sync
uv run groundtruth-eval all
uv run pytest -q
uv run ruff check .
```

## Outputs worth opening

- `outputs/dashboard.html`
- `outputs/project_working.svg`
- `outputs/evidence_map.svg`
- `outputs/operator_brief.md`
- `outputs/decision_report.md`
- `outputs/strategy_model.json`
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

Everything runs locally against synthetic fixtures. There are no credentials, no customer records, no outreach files, and no hosted API dependency.

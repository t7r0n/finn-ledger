# Finn Ledger

A deterministic, replayable "decision ledger" for AI wealth managers: every trade Finn proposes is a typed, simulated, wash sale safe MoveProposal with a tax impact diff and a counterfactual the user can accept, reject or amend in one tap.

![Finn Ledger working dashboard](outputs/project_working.svg)

## Why it exists

Finn is sold as an autopilot wealth manager that "executes money moves" and "optimizes tax." For a chatbot, that is enormously legally and operationally loaded.

Most internal demos stop at a pretty chart. This repository is built around the harder part: a repeatable path from fixture, to failure, to evidence, to the operator action a serious team would actually trust.

## What is inside

- A deterministic replay harness tuned around autopilot, wealth, and manager.
- Company-specific strategy code in `src/finn_ledger/strategy.py`, not just README-level customization.
- Citation-locked reports where every decision claim has to point back to a generated evidence ID.
- Two visual artifacts generated from the latest run: `outputs/project_working.svg` and `outputs/evidence_map.svg`.
- A portable demo pack with JSON, CSV, Markdown, HTML, SVG, and benchmark artifacts.

![Finn Ledger evidence map](outputs/evidence_map.svg)

## Signals it measures

- `autopilot coverage`
- `wealth risk`
- `manager precision`
- `executes latency`

## Failure modes it plants

- autopilot drift
- wealth gap
- manager misroute
- executes blindspot

## Run it locally

```bash
uv sync
uv run finn-ledger all
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

- https://www.ycombinator.com/companies/finvest
- https://www.usenix.org/conference/srecon22apac/speaker-or-organizer/shivam-bharuka-meta
- https://github.com/Shivam2501
- https://nocap.blog/founder/shivam-bharuka/
- https://www.usenix.org/conference/srecon22apac/presentation/bharuka
- https://alpaca.markets/docs/api-references/trading-api/
- https://www.irs.gov/publications/p550

## Boundary

Everything runs locally against synthetic fixtures. There are no credentials, no customer records, no outreach files, and no hosted API dependency.

# Operator Brief: Finvest

Finvest gets a local, deterministic pressure test around autopilot, wealth, and manager. The useful part is the repeatable evidence path from fixture to failure to operator action.

## Highest-leverage checks

- autopilot evidence replay -> block release until cited evidence is regenerated (autopilot_coverage, evidence ev_0132).
- executes operator packet -> accept only if decision claims cite fixture evidence (wealth_risk, evidence ev_0143).
- manager regression harness -> open a regression issue with trace and benchmark delta (manager_precision, evidence ev_0022).
- wealth boundary probe -> route to reviewer with evidence packet (executes_latency, evidence ev_0077).

## What makes this useful

The workflow is intentionally local and deterministic. A reviewer can run the same fixture set, inspect the evidence IDs, open the dashboard, and see exactly why a recommendation passed, went to review, or blocked.

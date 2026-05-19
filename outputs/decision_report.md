# Decision Report: Finn Ledger

A deterministic, replayable "decision ledger" for AI wealth managers: every trade Finn proposes is a typed, simulated, wash sale safe MoveProposal with a tax impact diff and a counterfactual the user can accept, reject or amend in one tap.

## Evidence-Grounded Findings

CLAIM: autopilot drift should `block release until replay is understood` because blocks=2 reviews=3 mean_severity=2.5. [EVID: ev_0022]
CLAIM: autopilot evidence recall should `block release until replay is understood` because blocks=3 reviews=3 mean_severity=1.875. [EVID: ev_0066]
CLAIM: executes policy boundary should `block release until replay is understood` because blocks=2 reviews=3 mean_severity=1.708. [EVID: ev_0033]
CLAIM: manager failure replay should `block release until replay is understood` because blocks=2 reviews=4 mean_severity=3.333. [EVID: ev_0110]
CLAIM: wealth gap should `block release until replay is understood` because blocks=3 reviews=2 mean_severity=3.333. [EVID: ev_0143]
CLAIM: wealth reviewer handoff should `block release until replay is understood` because blocks=2 reviews=4 mean_severity=2.583. [EVID: ev_0055]

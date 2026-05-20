# Decision Report: Finn Ledger

A deterministic, replayable "decision ledger" for AI wealth managers: every trade Finn proposes is a typed, simulated, wash sale safe MoveProposal with a tax impact diff and a counterfactual the user can accept, reject or amend in one tap.

## Evidence-Grounded Findings

CLAIM: autopilot evidence replay should `block release until cited evidence is regenerated` because blocks=4 reviews=5 mean_severity=2.611. [EVID: ev_0132]
CLAIM: executes operator packet should `accept only if decision claims cite fixture evidence` because blocks=4 reviews=5 mean_severity=2.556. [EVID: ev_0143]
CLAIM: manager regression harness should `open a regression issue with trace and benchmark delta` because blocks=3 reviews=5 mean_severity=2.528. [EVID: ev_0022]
CLAIM: wealth boundary probe should `route to reviewer with evidence packet` because blocks=3 reviews=4 mean_severity=2.528. [EVID: ev_0077]

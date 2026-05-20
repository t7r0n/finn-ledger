# Failure Matrix: Finn Ledger

| Scenario | Failure mode | Metric | Gate | Evidence |
| --- | --- | --- | --- | --- |
| autopilot evidence replay | autopilot_drift | autopilot_coverage | block release until cited evidence is regenerated | ev_0000 |
| executes operator packet | executes_blindspot | executes_latency | accept only if decision claims cite fixture evidence | ev_0007 |
| executes operator packet | executes_blindspot | executes_latency | accept only if decision claims cite fixture evidence | ev_0011 |
| manager regression harness | manager_misroute | manager_precision | open a regression issue with trace and benchmark delta | ev_0014 |
| wealth boundary probe | wealth_gap | wealth_risk | route to reviewer with evidence packet | ev_0021 |
| manager regression harness | manager_misroute | manager_precision | open a regression issue with trace and benchmark delta | ev_0022 |
| autopilot evidence replay | autopilot_drift | autopilot_coverage | block release until cited evidence is regenerated | ev_0028 |

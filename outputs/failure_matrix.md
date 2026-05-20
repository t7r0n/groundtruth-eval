# Failure Matrix: Groundtruth Eval

| Scenario | Failure mode | Metric | Gate | Evidence |
| --- | --- | --- | --- | --- |
| semantic evidence replay | semantic_drift | semantic_coverage | block release until cited evidence is regenerated | ev_0000 |
| product operator packet | product_blindspot | product_latency | accept only if decision claims cite fixture evidence | ev_0007 |
| product operator packet | product_blindspot | product_latency | accept only if decision claims cite fixture evidence | ev_0011 |
| agents regression harness | agents_misroute | agents_precision | open a regression issue with trace and benchmark delta | ev_0014 |
| layer boundary probe | layer_gap | layer_risk | route to reviewer with evidence packet | ev_0021 |
| agents regression harness | agents_misroute | agents_precision | open a regression issue with trace and benchmark delta | ev_0022 |
| semantic evidence replay | semantic_drift | semantic_coverage | block release until cited evidence is regenerated | ev_0028 |

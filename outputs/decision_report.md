# Decision Report: Groundtruth Eval

An open benchmark + harness that scores any context layer grounded analytics agent on natural language -> governed metric correctness, designed to make Kaelio the reference standard.

## Evidence-Grounded Findings

CLAIM: agents failure replay should `block release until replay is understood` because blocks=2 reviews=4 mean_severity=3.333. [EVID: ev_0110]
CLAIM: layer gap should `block release until replay is understood` because blocks=3 reviews=2 mean_severity=3.333. [EVID: ev_0077]
CLAIM: layer reviewer handoff should `block release until replay is understood` because blocks=2 reviews=4 mean_severity=2.583. [EVID: ev_0055]
CLAIM: product policy boundary should `block release until replay is understood` because blocks=2 reviews=3 mean_severity=1.708. [EVID: ev_0099]
CLAIM: semantic drift should `block release until replay is understood` because blocks=2 reviews=3 mean_severity=2.5. [EVID: ev_0088]
CLAIM: semantic evidence recall should `block release until replay is understood` because blocks=3 reviews=3 mean_severity=1.875. [EVID: ev_0066]

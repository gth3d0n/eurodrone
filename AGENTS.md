# Eurodrone Agent Rules

PURPOSE: 100 km/h quadcopter learning platform; custom core hardware; planned closed-loop flight; evidence-led development.
AUTHORITY: `requirements/TOP_LEVEL_REQUIREMENTS.md` > `docs/decisions/` > `docs/PROJECT_PHILOSOPHY.md` > source/test evidence. Conflict or consequential gap: report; do not silently decide or relax requirements.
PATHS: `requirements/`=normative; `docs/{architecture,decisions,operations}/`=design/decisions/operations; `hardware/{fc,pdu,airframe,harness}/`=custom hardware; `firmware/`=onboard; `software/{planning,control,simulation}/`=offline; `experiments/{fpga,positioning}/`=non-production exploration; `test/{plans,results}/`=procedure/evidence; `tools/`=utilities.

RULES:
- Before material change: read relevant authority; map change to `TLR-*`; flag ambiguity/gaps.
- Label evidence: `ASSUMPTION|ESTIMATE|SIMULATION|MEASUREMENT`; never claim unrun/unbuilt/simulated work is validated hardware behavior.
- Flight/power/propulsion/RF/control/autonomy changes: define validation and staged test path before escalation claims.
- Preserve unrelated work; make minimal coherent changes; do not commit secrets, machine-local config, generated artifacts, or raw logs unless explicitly intended.
- Parallel: non-overlapping paths; integration reports interfaces, assumptions, TLRs, evidence, risks; durable cross-system decisions go in `docs/decisions/`.

DONE: requested scope complete; relevant requirements/docs/test plans updated or assessed unaffected; available checks run and reported (including unrun checks); new safety/integration/validation risks stated.

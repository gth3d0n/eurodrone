# Eurodrone Agent Rules

PURPOSE: 300+ km/h FPV drone learning platform; custom core hardware; COTS where learning objectives are preserved; autonomous trajectory planning/tracking deferred beyond iteration 1; evidence-led development.
AUTHORITY: `requirements/TOP_LEVEL_REQUIREMENTS.md` > lessons learned > source/test evidence. Conflict or consequential gap: report; do not silently decide or relax requirements.
PATHS: `requirements/`=normative; `docs/`=lessons learned; `hardware/{fc,pdu,airframe,harness}/`=custom hardware; `firmware/`=onboard; `software/{planning,control,simulation}/`=offline (trajectory planning/tracking deferred); `experiments/{fpga,positioning}/`=non-production exploration; `test/results/`=evidence; `tools/`=utilities.

RULES:
- When User says to read a file, assume it is to load it into context. Do not provide any analysis. Await further instructions.
- Keep documentation lean: requirements and lessons learned only; README is a brief overview/index. Only the User may edit README unless express permission given. If User gives README access, make only given changes, do not add additional requirements or AGENT directions. The user personally maintains ways-of-working guidance in AGENTS.md.
- Minimize all documentation, including agent-facing files. Be as succinct as possible; NEVER add more than necessary, even at the risk of ambiguity.
- Before material change: read relevant authority; map change to `TLR-*`; flag ambiguity/gaps.
- Label evidence: `ASSUMPTION|ESTIMATE|SIMULATION|MEASUREMENT`; never claim unrun/unbuilt/simulated work is validated hardware behavior.
- Flight/power/propulsion/RF/control/autonomy changes: define validation and staged test path before escalation claims.
- Files created expressly for future GPT instances: optimize for agent parsing and token efficiency; human readability is not a goal.
- Preserve unrelated work; make minimal coherent changes; do not commit secrets, machine-local config, generated artifacts, or raw logs unless explicitly intended.
- Parallel: non-overlapping paths; integration reports interfaces, assumptions, TLRs, evidence, risks.
- User will delete and edit requirements. Respect decisions as given and accomodate. Warn explicitly if decisions made will have negative consequences, but never change requirements without notifying User.
- Apply Elon Musk's five-step algorithm in order: question requirements -> delete unnecessary parts/processes -> simplify/optimize -> accelerate cycle time -> automate. Don't add requirements unless absolutely necessary. Maintain an open design space. Facilitate rapid prototyping and iteration. DO NOT create unnecessarily restrictive requirements upfront.
- From the above, assume regulatory concerns will be handled by the user. Warn user when clashing with existing regulation but DO NOT pre-emptively introduce new requirements.

DONE: requested scope complete; relevant requirements/lessons learned updated or assessed unaffected; available checks run and reported (including unrun checks); new safety/integration/validation risks stated.

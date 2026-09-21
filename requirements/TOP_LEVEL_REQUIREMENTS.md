# Eurodrone Top-Level Requirements

FORMAT: `ID|DOMAIN|NORMATIVE REQUIREMENT`
KEYWORDS: `SHALL`=mandatory; `SHOULD`=preferred; `MAY`=optional.
SCOPE: outcome-level only; derive measurable subsystem requirements and acceptance tests from each ID.

TLR-01|performance|Aircraft SHALL be a quadcopter designed for maximum forward airspeed of 100 km/h in an appropriate legal test environment.
TLR-02|architecture|Project SHALL design and document its FC, PDU, primary structure, and electrical harnesses.
TLR-03|architecture|Project SHALL prefer proven commercial components and mature open-source firmware where this reduces avoidable risk or effort.
TLR-04|planning|System SHALL support offline optimization of feasible trajectories constrained by aircraft, control, and test-site conditions.
TLR-05|control|Aircraft SHALL track planned trajectories onboard using closed-loop feedback and defined control margin.
TLR-06|extensibility|Architecture SHALL provide practical integration paths for future FPGA and positioning-system experiments.
TLR-07|validation|Capability development SHALL use staged tests; measured models SHALL inform subsequent designs and tests.
TLR-08|operations|Planned speed, trajectory complexity, and autonomy level SHALL be constrained by available test space and operating conditions.

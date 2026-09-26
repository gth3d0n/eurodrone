# Eurodrone Top-Level Requirements

FORMAT: `ID|SCOPE|DOMAIN|NORMATIVE REQUIREMENT`
KEYWORDS: `SHALL`=mandatory; `SHOULD`=preferred; `MAY`=optional.
SCOPE: outcome-level only; derive measurable subsystem requirements and acceptance criteria from each ID. `I1`=active for iteration 1; `FUTURE`=deferred beyond iteration 1, excluded from its acceptance, with no committed delivery date.
LEARNING: electronics, mechanics, RF integration, and feedback control through custom core hardware, component characterization, integration, tuning, and measured tests.
STATUS: requirements baseline; no measured aircraft performance is recorded in this repository.

TLR-01|I1|performance|Aircraft SHALL be designed to achieve at least 300 km/h forward airspeed in repeatable, approximately level powered flight in an appropriate legal test environment. Performance beyond 300 km/h SHALL be pursued as evidence permits.
TLR-02|I1|architecture|Project SHALL design and document its FC, PDU, primary structure, and electrical harnesses.
TLR-03|I1|architecture|Project SHALL prefer proven commercial off-the-shelf (COTS) components and mature open-source flight firmware where this preserves learning objectives and reduces avoidable risk or effort; the custom hardware commitments in TLR-02 SHALL be retained.
TLR-04|FUTURE|planning|System SHALL support offline optimization of feasible trajectories constrained by aircraft, control, and test-site conditions.
TLR-05|FUTURE|control|Aircraft SHALL track planned trajectories onboard using closed-loop feedback and defined control margin.
TLR-06|I1|extensibility|Flight computing board SHALL integrate an FPGA and provide practical integration paths for future acceleration workloads, including CPU-FPGA communication bandwidth sufficient for the anticipated workloads. Architecture SHALL provide practical integration paths for future positioning-system experiments.
TLR-07|I1|control|Aircraft SHALL support piloted FPV operation through a pilot command link and onboard camera/video link, with onboard closed-loop stabilization and defined control margin.

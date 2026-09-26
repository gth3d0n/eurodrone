# Derived Requirements

FORMAT: `ID|SCOPE|PARENTS|REQUIREMENT`

SYS-01|I1|TLR-01,TLR-07|Aircraft SHALL support a piloted sortie comprising takeoff, stabilized hover, one speed-demonstration pass satisfying TLR-01, deceleration, return to the launch site, and landing.
VERIFY: Recorded flight demonstration of the sequence and applicable TLR-01 criteria. Staged path: bench checks -> hover/low-speed flight -> incremental speed passes.

## MP-01: SYS-01 sizing profile

ESTIMATE: Nominal durations; sizing assumptions, not acceptance limits.
ASSUMPTION: Preflight complete; one outbound pass; light wind; piloted return.

PHASE|DURATION_S
startup_readiness|30
takeoff_hover_alignment|15
acceleration|10
high_speed_level_flight|5
deceleration_turn|15
return|35
landing|10

TOTAL: 120 s powered; 90 s airborne. Return duration depends on course geometry and wind.
OPEN: Qualifying high-speed hold duration; recovery reserve additional to the nominal profile.

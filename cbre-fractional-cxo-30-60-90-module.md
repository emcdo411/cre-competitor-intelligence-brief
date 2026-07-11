---
name: cbre-fractional-cxo-30-60-90-module
description: >
  Extension module for the CBRE D&T Product Intelligence Lens and the Fractional CXO Practice
  Builder. Provides a structured 30/60/90 day transformation framework for a fractional CXO
  (CTO/CDO/COO-flavored) engagement inside a segment-siloed CRE enterprise like CBRE, with a
  specific focus on repairing communication and prioritization breakdowns between Devs, Ops,
  the business teams supporting D&T, and Project/Program Managers. Trigger this module any time
  Maurice says "run the 30-60-90," "build the transformation plan," "diagnose the CBRE org,"
  or is preparing onboarding/first-90-days material for a fractional or full-time D&T role at
  a multi-segment enterprise.
---

# CBRE Fractional CXO — 30/60/90 Day Transformation Module

## Root Diagnosis (read this before building any plan)

Large segment-siloed CRE enterprises like CBRE do not have a communication-style problem
between Devs, Ops, Business, and PMs. They have an **unowned trade-off problem** that
presents as a communication problem.

CBRE operates four segments (Advisory Services, Building Operations & Experience, Project
Management, Real Estate Investments) plus Corporate and Other, each with its own revenue
mechanic, operating cadence, and legacy systems of record (Salesforce, ServiceNow, MRI,
Yardi, Argus, Workday, plus T&T's own tooling post carve-out). D&T sits horizontally across
all four. Nobody below the CXO level typically owns the sequencing decision when two
segments want conflicting things from the same shared platform.

**Do not start a 30/60/90 by proposing tools, standups, or a new ticketing system.** Start
by finding out who currently absorbs the cost of that unowned trade-off. It is almost always
the PMs, invisibly, and it is almost always burning them out.

---

## Phase 1 — Days 1 to 30: Diagnose

**Fractional CXO lens question:** What's the binding constraint, and who is currently
absorbing the cost of it not being named?

### Week-by-week

**Days 1-7 — Listening tour, structured, not open-ended.**
Run the same four questions with every Dev lead, Ops lead, Business stakeholder, and PM:
1. What decision took longest to get made in the last 90 days, and who made it?
2. What's the last thing you built or shipped that nobody used?
3. What manual workaround are you running right now that shouldn't exist?
4. If you could kill one meeting or one report, which one, and why does it still exist?

**Days 8-15 — Map the segment-to-system matrix.**
For every shared D&T platform or service, document which of the four segments consume it,
what each segment's release-cadence expectation is, and where those expectations conflict.
This produces the DBL (constraint) map: is the binding constraint T1 (people), T2 (data/
systems), T3 (governance), or T4 (external/exogenous, e.g. vendor lock-in, M&A integration
debt)?

**Days 16-23 — Classify every in-flight D&T initiative.**
AI Theater / Partial Adoption / Embedded System, per the same test used on CBRE's own public
AI claims: is it used daily by operators, is it decision-driving or insight-only, is there a
feedback loop. Most enterprise D&T backlogs have more Theater in them than anyone admits.

**Days 24-30 — Name the constraint, in writing, to leadership.**
One page. The binding constraint, who's currently absorbing its cost, and the cost in hours
or dollars if quantifiable. No solution yet. A CXO who proposes a fix before naming the
constraint in front of leadership has skipped the step that makes the fix stick.

### Phase 1 output
A one-page Constraint Brief: named binding constraint, named cost-absorber, DBL classification,
and a capability inventory tagged Theater / Partial / Embedded.

---

## Phase 2 — Days 31 to 60: Stabilize

**Fractional CXO lens question:** What gets removed or simplified before anything new gets
added? (Fraser Gate / subtraction audit, applied at org level, not just product level.)

### Week-by-week

**Days 31-38 — Subtraction pass.**
Identify the manual workarounds, shadow spreadsheets, and duplicate status meetings that
exist because the real trade-off was never owned. Kill or consolidate at least one per
segment before proposing anything new. This buys credibility faster than any new tool will.

**Days 39-46 — Install a single ownership rule (OAL).**
Every shared D&T initiative gets exactly one named owner accountable for the cross-segment
trade-off, not a committee, not "the D&T team." This is the single highest-leverage move in
the whole 90 days, because it's the direct fix for the root diagnosis.

**Days 47-53 — Build the cadence bridge.**
Devs, Ops, Business, and PMs are not going to share one release cadence across four segments
with genuinely different rhythms (deal cycles vs facilities SLAs vs capital-project
timelines vs fund-accounting cycles). Instead, build a translation layer: one shared
prioritization forum, meeting monthly, where each segment's ask is scored against the same
named constraint from Phase 1, not against each other's politics.

**Days 54-60 — Pilot the first proof point.**
Pick the single highest-leverage fix from the Constraint Brief. Ship something small and
real. A working scoreboard, a single unified data view, one workflow automated end to end.
This is not the full transformation. It's proof the diagnosis was right.

### Phase 2 output
One dead process per segment (subtracted), one named owner per shared initiative (OAL
installed), one monthly cross-segment prioritization forum running, one shipped proof point.

---

## Phase 3 — Days 61 to 90: Scale

**Fractional CXO lens question:** What does this look like without me in the room, and does
it survive contact with the next reorg or acquisition?

### Week-by-week

**Days 61-70 — Codify the ownership model.**
Turn the informal OAL assignments from Phase 2 into a documented RACI that survives
personnel change. Every shared platform, every cross-segment data flow, gets a named owner
in writing, not tribal knowledge.

**Days 71-80 — Extend the proof point.**
Take the Phase 2 pilot and expand it to a second segment. This tests whether the fix was
segment-specific luck or a genuinely portable pattern. If it doesn't port cleanly, that's
real information, not a failure.

**Days 81-87 — Governance handoff.**
Document the CGM-equivalent for this org: who owns criteria validity when a shared
platform's assumptions go stale, who re-scores segment priorities when the market shifts,
who's accountable if the constraint changes. This is the piece almost every enterprise
transformation skips, and it's why so many revert within 12 months of the consultant leaving.

**Days 88-90 — Board-level readout.**
Translate all of it into the CFO/board frame: here's the constraint we found, here's what
it was costing (in hours, dollars, or missed revenue), here's what's fixed, here's what's
next, here's who owns it now that isn't you.

### Phase 3 output
A written RACI, a second-segment proof point, a documented governance model, and a
board-ready readout that names a successor owner for every mechanism installed.

---

## The 90-Day Scorecard

| Phase | Days | Core Question | Required Output | Named Owner? |
|---|---|---|---|---|
| Diagnose | 1-30 | What's the binding constraint, who absorbs its cost | Constraint Brief | Not yet, this is discovery |
| Stabilize | 31-60 | What gets removed before anything is added | Subtraction + OAL + one proof point | Yes, per initiative |
| Scale | 61-90 | Does it survive without me in the room | RACI + second proof point + governance doc | Yes, documented successor |

**Hard rule across all three phases:** no phase produces a recommendation without a named
owner attached. A finding without an owner is a diagnosis with no patient.

---

## Why this module pairs with the CBRE Product Intelligence Lens

Everything in this 30/60/90 is built to be defensible under Max S.'s three-layer stress
test from the companion skill:

- **AI Relevance:** every phase produces a measurable artifact (Constraint Brief, proof
  point, RACI), never a vague "improved communication" claim.
- **CRE Value Connection:** every phase is anchored to CBRE's actual segment structure
  (Advisory, BOE, Project Management, REI), not a generic org-transformation template.
- **Product Executive Alignment:** the framework is explicitly roadmap-shaped (30/60/90,
  named owners, board-level readout), not a task list.

Run any 30/60/90 talking point built from this module back through the companion skill's
stress test before using it in an interview or an actual engagement kickoff.

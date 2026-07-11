# CBRE D&T Fractional CXO — 30/60/90 Day Transformation Plan

**Root diagnosis:** CBRE's D&T org doesn't have a communication-style problem between Devs, Ops, Business, and PMs. It has an unowned trade-off problem across four segments (Advisory Services, Building Operations & Experience, Project Management, Real Estate Investments) that presents as a communication problem. Whoever is absorbing that unowned cost right now is almost certainly the PMs, invisibly, and it's burning them out.

The plan below does not open with tools or process. It opens with finding the constraint and naming who's paying for it.

---

## Phase 1 (Days 1-30): Diagnose

**Lens question:** What's the binding constraint, and who is currently absorbing the cost of it not being named?

**Days 1-7 — Structured listening tour.** Same four questions to every Dev lead, Ops lead, Business stakeholder, and PM I meet:
1. What decision took longest to get made in the last 90 days, and who made it?
2. What's the last thing you built or shipped that nobody used?
3. What manual workaround are you running right now that shouldn't exist?
4. If you could kill one meeting or one report, which one, and why does it still exist?

**Days 8-15 — Segment-to-system matrix.** For every shared D&T platform (Salesforce, ServiceNow, MRI, Yardi, Argus, Workday, T&T tooling), map which segments consume it, each segment's release-cadence expectation, and where those expectations collide. This produces the constraint classification: people (T1), data/systems (T2), governance (T3), or external/exogenous like vendor lock-in or M&A integration debt (T4).

**Days 16-23 — Classify in-flight initiatives.** AI Theater / Partial Adoption / Embedded System, using the same test I'd apply to any vendor's AI claims: is it used daily by operators, is it decision-driving or just insight-only, is there a feedback loop. Most enterprise D&T backlogs carry more Theater than anyone wants to admit in the review.

**Days 24-30 — Name the constraint in writing.** One page to leadership: the binding constraint, who's absorbing its cost, the cost in hours or dollars where quantifiable. No solution yet. Proposing the fix before naming the constraint in front of leadership is the move that makes fixes not stick.

**Output:** A one-page Constraint Brief — named constraint, named cost-absorber, T1-T4 classification, and a capability inventory tagged Theater / Partial / Embedded.

---

## Phase 2 (Days 31-60): Stabilize

**Lens question:** What gets removed or simplified before anything new gets added?

**Days 31-38 — Subtraction pass.** Find the manual workarounds, shadow spreadsheets, and duplicate status meetings that exist because the real trade-off was never owned. Kill or consolidate at least one per segment before proposing anything new. This buys more credibility in 8 days than a new tool would buy in 8 months.

**Days 39-46 — Install single ownership.** Every shared D&T initiative gets exactly one named owner accountable for the cross-segment trade-off — not a committee, not "the D&T team." This is the highest-leverage move in the whole 90 days because it directly fixes the root diagnosis.

**Days 47-53 — Build the cadence bridge.** Devs, Ops, Business, and PMs won't share one release cadence across four segments with genuinely different rhythms (deal cycles vs. facilities SLAs vs. capital-project timelines vs. fund-accounting cycles). Instead: one shared prioritization forum, meeting monthly, where each segment's ask is scored against the named constraint from Phase 1 — not against each other's politics.

**Days 54-60 — Pilot the first proof point.** Take the single highest-leverage fix from the Constraint Brief and ship something small and real: a working scoreboard, a unified data view, one workflow automated end to end. Not the transformation. Proof the diagnosis was right.

**Output:** One dead process per segment, one named owner per shared initiative, one monthly cross-segment prioritization forum running, one shipped proof point.

---

## Phase 3 (Days 61-90): Scale

**Lens question:** What does this look like without me in the room, and does it survive the next reorg or acquisition?

**Days 61-70 — Codify ownership.** Turn the informal owner assignments from Phase 2 into a documented RACI. Every shared platform, every cross-segment data flow gets a named owner in writing, not tribal knowledge.

**Days 71-80 — Extend the proof point.** Port the Phase 2 pilot to a second segment. This tests whether the fix was segment-specific luck or a genuinely portable pattern. If it doesn't port cleanly, that's real information, not a failure, and it goes in the readout as such.

**Days 81-87 — Governance handoff.** Document who owns criteria validity when a shared platform's assumptions go stale, who re-scores segment priorities when the market shifts, who's accountable if the constraint itself changes. This is the piece most enterprise transformations skip, and it's why so many revert within 12 months of the outside person leaving.

**Days 88-90 — Board-level readout.** CFO/board frame: the constraint we found, what it was costing, what's fixed, what's next, who owns it now that isn't me.

**Output:** A written RACI, a second-segment proof point, a documented governance model, a board-ready readout naming a successor owner for every mechanism installed.

---

## The 90-Day Scorecard

| Phase | Days | Core Question | Required Output | Named Owner? |
|---|---|---|---|---|
| Diagnose | 1-30 | What's the binding constraint, who absorbs its cost | Constraint Brief | Not yet -- this is discovery |
| Stabilize | 31-60 | What gets removed before anything is added | Subtraction + single ownership + one proof point | Yes, per initiative |
| Scale | 61-90 | Does it survive without me in the room | RACI + second proof point + governance doc | Yes, documented successor |

**Hard rule across all three phases:** no phase produces a recommendation without a named owner attached. A finding without an owner is a diagnosis with no patient.

---

## Interview-Ready Compression (30-second version)

"My first 30 days aren't about tools, they're about finding the trade-off nobody at CBRE currently owns between segments and naming who's quietly absorbing the cost of that gap, usually the PMs. Days 31-60, I subtract before I add: kill the shadow spreadsheets, install one named owner per shared initiative, ship one small real proof point. Days 61-90, I make sure it survives without me: a written RACI, the pattern ported to a second segment, and a board-level readout that names who owns it next."

---

## Companion Stress Test (Max S. lens)

- **AI Relevance:** Every phase produces a measurable artifact (Constraint Brief, proof point, RACI) instead of a vague "improved communication" claim.
- **CRE Value Connection:** Anchored explicitly to CBRE's real segment structure (Advisory, BOE, Project Management, REI) and real platforms (Salesforce, ServiceNow, MRI, Yardi, Argus, Workday), not a generic org-transformation template.
- **Product Executive Alignment:** Roadmap-shaped with named owners and a board-level readout, not a task list.

Before using the compressed version above in the interview, run it through the full CBRE Product Intelligence Lens stress test for a SHIP / SHIP WITH CONDITIONS / NO SHIP verdict.

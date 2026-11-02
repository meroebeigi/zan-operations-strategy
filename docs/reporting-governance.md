# Reporting, stakeholder and data governance

## Proposed report specifications
| Report | Audience / cadence | Content | Decision |
|---|---|---|---|
| Service queue | Coordinators / daily when staffed | Open requests, age, deadline risk, unmatched work, blocked reason | Reassign, clarify, escalate or communicate delay |
| Operations review | Coordinators and quality leads / weekly | Throughput, on-time delivery, turnaround, first-pass quality, workload and limitations | Choose corrective action and owner |
| Leadership review | Leadership / monthly | Mature-cohort outcomes, service capacity, funding, partnership commitments and risks | Sequence growth and resource allocation |
| Quality calibration | Quality leads and reviewers / periodically | Anonymized rubric disagreements, rework reasons and training needs | Update rubric or coaching |

These are specifications, not built dashboards or populated reports. Each future report should show period, cutoff, refresh time, definition version, denominator, coverage, owner and known limitations. Add filters only when they support a defined decision and preserve confidentiality.

## So what / now what review structure
1. What changed? State the metric, period and comparison.
2. So what? Explain the service or mission consequence and evidence confidence.
3. Why might it have changed? Separate confirmed facts from hypotheses.
4. Now what? Agree an action, accountable role and due date.
5. How will we know? Specify a follow-up measure and balancing measure.

Without data, use this as a blank reporting template. Do not populate it with invented findings.

## Stakeholder engagement
Proposed stakeholders: leadership, intake coordinators, volunteers, quality leads, impact/development roles and future technical support. Beneficiary feedback informs process design without requiring public identification.

Use written intake and an asynchronous review window so volunteers in different time zones can contribute. Capture the requester, decision, urgency, affected users, effort and success criterion. Prioritize mission value, delivery risk, reach and feasible effort. Communicate accepted, deferred or declined decisions with reasons. Actual shift-based engagement is outside this project.

## Metric and report governance
Maintain a report inventory with purpose, owner, audience, source, metric versions, cadence and last-use review. Classify reports as draft, approved, superseded or retired. A report becomes approved only after the accountable owner accepts definitions, reconciliation evidence and limitations.

Before proposing a new report, check existing coverage. Consolidate overlapping reports when audiences and decisions align. Retire a report only after checking dependencies, archiving its definition and notifying affected users. No existing reports have been audited or retired here.

Resolve KPI conflicts by documenting competing definitions, calculating worked examples, selecting the definition aligned to the decision and obtaining owner approval. Keep legitimate alternative measures distinctly named, such as original-deadline versus revised-deadline delivery.

## Future Data Engineering handoff
Specify entities, keys, event grain, update cadence, timestamp rules, status history, source ownership, expected completeness and failure handling. Define field meanings before choosing tools. Request stable request IDs, immutable event history and traceable revisions.

Acceptance criteria for future datasets: documented keys, referential checks, agreed freshness, source reconciliation, controlled access, lineage and a visible exception process. File a quality issue with affected records, expected versus observed behavior, business impact, reproducible evidence and an owner. No pipelines or certified datasets are implemented here.

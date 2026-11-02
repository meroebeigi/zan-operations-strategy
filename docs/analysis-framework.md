# Decision and analysis framework

No analysis has been performed. This document translates business questions into future analysis specifications.

| Question | Testable hypothesis | Required evidence and method | Confounders / limitations | Decision supported |
|---|---|---|---|---|
| Why are deliveries late? | High concurrent workload is associated with more missed deadlines | Join assignment history, capacity and original deadlines; compare workload bands within service types | Urgency, complexity, volunteer experience and selection effects | Pilot capacity-aware assignment |
| Does training improve quality? | Trained volunteers require less first-pass rework | Compare quality-check outcomes by training completion before assignment; stratify by service and reviewer | Experienced volunteers may be more likely to finish training; rubric changes | Revise onboarding and test a pilot |
| Where is the bottleneck? | Matching accounts for more waiting time than other stages | Decompose event-based stage durations; examine queue age and arrival/completion rates | Missing events and overlapping stages | Add coordinator capacity or change matching rules |
| Which outreach is useful? | Some channels generate more completed eligible services per unit effort | Follow intake cohorts from tagged channel to acceptance and completion | Attribution gaps, channel mix and seasonal deadlines | Reallocate outreach effort within capacity |
| Are outcomes measured fairly? | Follow-up respondents differ from nonrespondents | Compare response coverage by service, cohort and available non-sensitive attributes | Unobserved outcomes cannot be recovered by assumption | Improve follow-up and qualify impact claims |
| Is recurring giving sustainable? | A small number of donors accounts for a large receipt share | Examine donor concentration, recurring status and cohort retention | Short history and one-time grants | Diversify fundraising and build stewardship |

## Standard analytical brief
State the decision, question, population, period, hypothesis, necessary fields, definition version, comparison method, expected biases and evidence needed. Predefine what would justify a pilot, deferral or additional investigation. Numeric decision thresholds require baseline and capacity review, not invented targets.

## Root-cause discipline
Use process mapping, Pareto categories and a cause-and-effect discussion to identify candidate causes. Validate causes against event evidence and staff explanations. A chart or correlation alone does not establish a root cause. Acknowledge seasonal deadlines, policy changes and incomplete records.

## Future data validation plan
Check request uniqueness, valid assignment relationships, timestamp ordering, accepted status codes, deadline history, missingness, duplicate gifts and reporting freshness. Reconcile dashboard counts with delivery events and finance totals with reconciled receipts. Trace selected records from capture through transformation to report. Publish exceptions and their impact. These are planned checks, not executed validation.

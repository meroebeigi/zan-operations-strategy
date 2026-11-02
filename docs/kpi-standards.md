# Proposed KPI standards

## Common calculation contract
These definitions are proposals derived from the metric names in S2, p. 1, and S1, pp. 7-8. Baselines and targets are **TBD** for every metric. No actual values are calculated.

- Grain: distinguish applicant, request, review attempt, volunteer, event, donation and website session. Count distinct IDs at the stated grain.
- Reporting: proposed calendar-month reporting with weekly operations views. Approve one reporting timezone. Store event timestamps consistently and convert before assigning periods.
- Zero denominators produce N/A, never zero percent. Missing values remain unknown, never inferred successes, failures or zero durations.
- Display numerator, denominator, coverage and reporting window with rates. Report percentages as 100 x the stated ratio.
- Use accepted requests for operational cohorts; exclude declined intake. Keep withdrawals visible and state each metric's treatment. Reopened requests retain identity and history.
- Outcome metrics use cohorts with an agreed follow-up window, provisionally 180 days after delivery. This interval requires approval and may differ by service. Report response coverage and pending outcomes alongside success rates.
- Duration metrics use elapsed calendar hours/days unless explicitly labeled working time. Report median and 90th percentile alongside the source-requested average where possible. Open items appear in aging reports, not completed-duration averages.
- Examples below are invented arithmetic demonstrations only.

## Impact and applicant success
| ID / KPI | Calculation and population | Proposed evidence, owner and cadence | Interpretation and exclusions |
|---|---|---|---|
| I01 Admission success | Applicants reporting at least one admission / applicants in the mature education-support cohort with a known admission outcome | Follow-up response or voluntarily supplied confirmation; Impact lead; quarterly | Applicant-level, not applications-level. Report known outcomes / eligible mature cohort as coverage. Unknown outcomes excluded from success denominator but shown separately |
| I02 Scholarship success | Applicants reporting at least one scholarship / applicants in the mature scholarship-support cohort with a known outcome | Outcome follow-up; Impact lead; quarterly | Define eligible award types. Do not include applicants who did not seek scholarships. Report response coverage |
| I03 Job placement | Applicants reporting at least one accepted job offer / applicants in the mature career-support cohort with a known job outcome | Outcome follow-up; Impact lead; quarterly | Define qualifying employment and observation window; report coverage and avoid causal attribution |
| I04 Volunteer activity retention | Provisionally: volunteers active in both prior and current month / volunteers active in prior month | Assignment/activity log; Volunteer coordinator; monthly | Source calls this volunteer activity retention under applicant impact. Confirm meaning before adoption; potentially consolidate with V01 |
| I05 Average review time | Sum of elapsed time from accepted assignment to review submission / completed review attempts | Assignment and review events; Operations; weekly/monthly | Attempt-level. Excludes matching and quality-check time. Report open-review aging separately; pair with end-to-end turnaround |
| I06 Applicant satisfaction | Sum of valid 1-10 applicant ratings / valid responses | Optional survey linked to request; Impact lead; monthly | One selected response per request under a documented deduplication rule; publish response rate and sample size |

## Volunteer performance
| ID / KPI | Calculation and population | Proposed evidence, owner and cadence | Interpretation and exclusions |
|---|---|---|---|
| V01 Volunteer retention | Volunteers eligible at period start who remain enrolled and available at period end / eligible volunteers at period start | Roster status history; Volunteer coordinator; monthly | Define eligible roster; exclude already paused or offboarded volunteers at start. Report planned pauses separately. Membership retention differs from I04 activity retention |
| V02 Volunteer satisfaction | Sum of valid 1-10 volunteer ratings / valid responses | Anonymous or pseudonymous survey; Volunteer coordinator; quarterly | One response per volunteer per survey round; report response coverage and small-sample limitations |
| V03 Workload balance | Open assignments at cutoff / available volunteers at cutoff | Assignments and declared availability; Operations; weekly | This average alone does not measure balance. Add distribution of open assignments and, when reliable, assignment load / declared capacity by volunteer |
| V04 Response time | Sum of hours from assignment notification to first substantive volunteer response / assignments receiving a response | Notification and response events; Operations; weekly | Automated acknowledgments do not count. Unanswered assignments remain in a separate aging list |
| V05 Training completion | Volunteers completing all required modules by their due date / volunteers with required training due in period | Training register; Quality lead; monthly | Version the requirement; approved exemptions are excluded and disclosed; incomplete records are not completed training |

## Operational efficiency
| ID / KPI | Calculation and population | Proposed evidence, owner and cadence | Interpretation and exclusions |
|---|---|---|---|
| O01 Applicant-to-volunteer ratio | Distinct applicants with open accepted requests / available volunteers at cutoff | Request and roster snapshots; Operations; weekly | Applicant-level. Complement with request counts because one applicant can have several requests |
| O02 Service completion rate | Accepted requests in intake cohort delivered within approved observation window / all accepted requests in that cohort | Request event history; Operations; monthly cohort review | Proposed 30-day window pending feasibility review. Withdrawals stay in denominator with reasons; immature cohorts marked pending. Not completions this month / new requests this month |
| O03 Technical resolution time | Sum of elapsed time from incident detection to confirmed restoration / incidents restored in period | Incident log; Platform owner; monthly | Report severity separately, open incident age and recurrence. Detection time is not necessarily outage start |
| O04 Website engagement | Sessions meeting an approved engagement-event rule / eligible measured website sessions | Analytics event definitions; Communications; monthly | Define event rule and bot/internal exclusions before use; consent and blocking can limit coverage |

## Fundraising and sustainability
| ID / KPI | Calculation and population | Proposed evidence, owner and cadence | Interpretation and exclusions |
|---|---|---|---|
| F01 Total funds raised | Sum of received donation and grant receipts less refunds in period | Reconciled payment/finance records; Finance role; monthly | Report gross receipts, refunds and net receipts. Exclude unpaid pledges; separate restricted receipts and in-kind support. Convert currency under an approved policy |
| F02 Average donation | Net donation value attributed to gifts received in period / count of those gifts | Gift register reconciled to payment records; Finance role; monthly | Gift-level, not donor-level. Apply a stated refund cutoff; exclude grants if reported as a separate stream |
| F03 Recurring donor rate | Distinct donors with a successful scheduled recurring gift in period / distinct donors with any successful gift in period | Donor and payment records; Development lead; monthly | This is donor mix, not donor retention. Report recurring-donor retention separately if needed; deduplicate anonymous IDs consistently |
| F04 Fundraising event ROI | (Event-attributed received funds - direct event costs) / direct event costs | Event ledger and attribution register; Finance role; after event closure | Multiply by 100. Approve attribution window; disclose excluded overhead and volunteer time. Zero costs -> N/A. Do not imply full economic return |

## Social media and community engagement
| ID / KPI | Calculation and population | Proposed evidence, owner and cadence | Interpretation and exclusions |
|---|---|---|---|
| C01 Follower growth | (Closing followers - opening followers) / opening followers | Platform snapshots; Communications; monthly | Report by platform; opening zero -> N/A with absolute change |
| C02 Engagement rate | Defined interactions on period-published posts within a fixed observation window / impressions for the same posts and window | Platform analytics; Communications; monthly | List included interactions; use consistent post maturity. Platform definitions differ; do not average rates without denominator weights |
| C03 Social website traffic | Website sessions attributed to social media / website sessions with known acquisition source | Website analytics; Communications; monthly | Show unknown-source share separately; referral attribution is incomplete and not proof of causation |
| C04 Conversion rate | Eligible measured website sessions with a successful request submission / eligible measured website sessions | Submission events and analytics; Communications; monthly | Session-level, at most one conversion per session. Intake acceptance is a separate downstream measure; donor conversion must be separate |
| C05 Content effectiveness | Rank content types by C04 when attribution is reliable; otherwise by C02 with comparable windows | Tagged content and analytics; Communications; monthly | A categorical finding, not one universal percentage. Show reach and denominators; avoid declaring a winner from tiny samples |

Social metrics remain provisionally included pending clarification of the source note DEL. D, S and DOR are also unresolved; no ownership is inferred from these abbreviations.

## Additional service-control KPIs
These are new proposals rather than source metrics.

| KPI | Definition | Evidence and proposed owner |
|---|---|---|
| First-pass quality | First quality checks accepted without required correction / all first quality checks completed in period | Quality-check log; Quality lead; weekly |
| Rework rate | First quality checks requiring correction / all first quality checks completed in period | Same population as first-pass quality; Quality lead; weekly |
| Throughput | Distinct requests delivered during period | Delivery events; Operations; weekly |
| On-time delivery | Requests delivered by original committed deadline / all accepted requests due in period | Deadline history and delivery events; Operations; weekly; overdue undelivered requests count as late; exclude pre-deadline withdrawals and report them separately |
| End-to-end turnaround | Mean, median and P90 elapsed time from accepted intake to delivery for requests delivered in period | Request events; Operations; weekly; report open-request age separately |
| Backlog | Accepted requests not delivered or otherwise terminal at cutoff | Status history; Operations; daily/weekly; show aging and waitlist separately |
| Platform availability | (Scheduled monitoring minutes - union of confirmed unavailable minutes) / scheduled monitoring minutes | Monitoring/incident records; Platform owner; monthly; disclose maintenance and unmonitored windows; avoid double-counting overlapping outages |

## Worked examples for definition review
- First-pass quality: 18 accepted first checks out of 24 first checks = 75%; six requiring correction = 25% rework. Later successful attempts do not improve first-pass quality retroactively.
- On-time delivery: 20 requests due, 15 delivered by original deadline, three delivered late and two still open = 75%. Dividing by only the 18 delivered would hide overdue work.
- Cohort completion: 40 accepted requests, 30 delivered within 30 days, five still open and five withdrawn = 75%. A cohort younger than 30 days is provisional.
- Admission: 12 successes among 20 known outcomes = 60%; if 50 mature applicants were eligible, coverage is 40%. This is not evidence of a 60% success rate for all 50.
- Event ROI: hypothetical receipts of 1,500 and direct costs of 500 give (1,500 - 500) / 500 = 200%, excluding unpriced volunteer time and overhead.

## Adoption process
The metric steward presents examples to operations, quality, impact and development roles. Review edge cases, resolve disagreements, assign an accountable approver and approve version 1 with an effective date. Publish the dictionary alongside reports. Train coordinators across availability windows using a recorded walkthrough and written questions. Review after one reporting cycle; document changes and whether historical restatement is needed. No adoption or stakeholder training is claimed here.

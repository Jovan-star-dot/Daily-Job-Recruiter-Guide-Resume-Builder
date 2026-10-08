# How the recruiter workflow works

This is a prompt-based workflow executed with the capabilities available in your ChatGPT session. These stages do not require ten separate agents or ten scheduled tasks.

| Stage | What it does | What you can inspect |
| --- | --- | --- |
| Scheduled Search | Searches according to your profile and daily settings | Exact queries and run log |
| Verify Job | Reads requirements and checks live employer application pages | URLs, verification date, eligibility |
| Deduplicate | Checks tracker and existing packages by stable job identity | Duplicate key and skipped roles |
| Hard Filter | Excludes indispensable requirements and deal-breaker conflicts | Rejection or hold reason |
| Score | Assesses evidence-based fit against a consistent rubric | Points and candidate evidence |
| SWOT/ATS | Explains fit, gaps, risks, and relevant posting terms | SWOT and keyword evidence map |
| Resume | Tailors the master resume using truthful facts | Role-specific document or labeled draft |
| QA | Checks accuracy, layout, requirements, score, and live links | Completed checks and corrections |
| Final Package | Collects the job assessment and materials | Package and tracker entry |
| Your Review | Candidate resolves questions and chooses whether to apply | Candidate decision/application status |

## Scoring

This starter kit preserves the rubric in the active Daily Recruiter Run from which it was adapted.

| Dimension | Weight | Maximum points out of 10 |
| --- | --- | --- |
| Required skills | 35% | 3.5 |
| Experience/years | 20% | 2.0 |
| Industry/domain | 15% | 1.5 |
| Logistics/location | 10% | 1.0 |
| Compensation | 10% | 1.0 |
| Career-goal alignment | 10% | 1.0 |
| Total | 100% | 10.0 |

The default qualifying threshold is 8.5/10 inclusive. A score of 8.49 does not qualify by rounding. Explain each component with job requirements and candidate evidence. Unknown essential eligibility requires a hold; an indispensable requirement failure overrides the total.

Missing salary receives no asserted compensation-match credit. If the candidate has no compensation preference at all, the included prompt uses a clearly labeled neutral 0.5/1. This prevents claiming an unstated salary meets a requirement. Follow the profile's separate policy on allowing or holding salary-not-stated roles.

For example, component scores of 3.2 + 1.8 + 1.3 + 1.0 + 0.5 + 0.9 total 8.7. That clears 8.5 only if the hard filters pass and the supporting evidence is real. This arithmetic example is fictional and is not a candidate or job assessment.

## Quality outcomes

- `APPROVED`: relevant checks passed; candidate review still required.
- `NEEDS YOUR REVIEW`: resolvable gaps or unperformed checks remain.
- `REJECT JOB`: disqualifying issue or role falls below the qualifying standard.

Unverified roles belong in the hold list rather than the complete-package list. Document-generation failures can result in a labeled text draft, with its missing checks made explicit.

## Tracking

A prepared package is not a submitted application. The tracker records review and package preparation, and records Applied only after the candidate confirms submission. Each run must preserve earlier entries and report whether the update actually saved.

Source files and tracker access must persist across runs. A scheduled prompt does not supply durable state by itself. If persistence fails, save the provided full updated tracker and make it available before the next run.

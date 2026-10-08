# Job Tracker

Keep this private. Read and update the same tracker each run; preserve earlier entries. This tracker is intentionally empty.

## Run state

- Last completed search local date: Not yet run
- Timezone: From Candidate_Profile.md
- Current source profile version/date: Not yet confirmed
- Tracker persistence location/reference: To be confirmed

## Reviewed jobs

| Stable job key | Company | Role | Location/arrangement | Job/requisition ID | Official application URL | Verified date | Salary/currency | Score /10 | Verdict | Candidate status | ATS keywords/gaps | Package references | Notes |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |

Verdicts: `APPROVED`, `NEEDS YOUR REVIEW`, `REJECT JOB`. APPROVED means the package passed internal checks; it still needs your review before applying.

Candidate statuses: `Reviewed`, `Package prepared`, `Applied`, `Interview`, `Rejected`, `Withdrawn`, `Closed`. Record `Applied` only after the candidate confirms submission.

Deduplicate by employer + requisition ID first. Otherwise use normalized company + title + location + canonical official application URL. Ignore tracking parameters when comparing URLs. Different postings of the same requisition count once; distinct requisitions at the same employer are not automatically duplicates. Do not put the run date in the stable job key.

## Search log

| Local run date | Query number | Exact query | Source/location scope | Status | Results/verification notes |
| --- | --- | --- | --- | --- | --- |

Query statuses: `Completed`, `Failed`, `Blocked`. Record actual execution; a failed query is not evidence of zero matching jobs.

## Run summary

| Local date | Queries completed/requested | Jobs verified | Duplicates skipped | Rejected | Held for review | Complete packages | Tracker saved? | Limitations |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |

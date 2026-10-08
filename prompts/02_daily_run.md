# Daily run prompt

Use this for a manual run and as the complete saved instructions for recurring runs. Candidate-specific settings belong in your private profile. For a small first test, add the test-mode line from START_HERE.md above this prompt.

```text
Run my Daily Recruiter workflow using my confirmed Candidate_Profile.md, Master_Resume_ATS.docx, Job_Preferences.md, Career_Goals.md, Proof_Points.md, and Job_Tracker.md. Use the private source-file manifest to find them. Candidate_Profile.md supplies run settings; the master resume and verified proof points supply candidate evidence. Ask about conflicts. Do not use another person's profile or fill missing facts from assumptions.

Follow this order: Scheduled Search → Verify Job → Deduplicate → Hard Filter → Score → SWOT/ATS → Resume → QA → Final Package → My Review.

SOURCE CHECK AND STATE
Read the accessible source files and the same persistent tracker at the start. Confirm current facts and use my profile's IANA timezone for the local run date. If essential candidate sources are unavailable, name the missing sources and stop before scoring or resume generation. If the tracker is unavailable, do not claim cross-run deduplication; report the blocker and request it before producing repeat-sensitive packages. Check existing accessible application artifacts as well as tracker entries. Do not create another automation during a run.

SEARCH
Use my query count and package limit; defaults are 20 distinct targeted searches and at most 10 complete packages. A temporary test-mode override applies to that run only. Cover my role families and geographic/work-arrangement priorities. Search public job boards and employer careers pages. Prefer recent postings, initially emphasizing the last 14 days; include older postings when verified open. On later runs use an overlapping lookback around the last successful search to catch delayed indexing.
Record actual queries, scope, and failures. Do not claim exhaustive coverage. Do not bypass access controls. If today's full scan is already recorded complete, avoid repeating it; reverify and work from the unsent/unprepared queue. On a retry, resume missing or failed queries. Count complete packages already prepared today toward the daily limit. Never lower my score threshold to fill the limit.

VERIFY
Read the full job description, identify the actual employer, and verify the current official careers/application page where accessible. Record posting and verification dates, title, location, arrangement, requisition ID, salary/currency, deadline, requirements, and source URLs. Do not rate a job from a search snippet alone. Exclude demonstrably closed jobs. If current status, essential requirements, or the official apply link cannot be verified, hold it as unverified; do not include it as a complete qualifying package. State access gaps.

DEDUPLICATE
Check both the tracker and accessible existing resumes/cover letters/packages. Prefer employer + requisition ID. Otherwise compare normalized company, title, location, and canonical official URL without tracking parameters. A date-based key is not a stable job identity. Skip previously reviewed/materially identical roles unless I explicitly request a refresh or the requirements materially changed; explain any refresh. Distinct requisitions at the same company can be distinct jobs. Never infer I applied because a package exists.

HARD FILTER
Reject clear conflicts with my deal-breakers and clearly unmet indispensable qualifications before scoring. Check location restrictions, authorization/sponsorship, required language, licenses, and availability when relevant. Do not treat unknown essential eligibility as satisfied; hold the job for clarification. Distinguish indispensable requirements from preferences and transferable experience. Follow my salary-not-stated policy; do not invent salary estimates as posted compensation.

SCORE
Use one consistent editorial fit rubric out of 10:
- Required skills: 3.5 points maximum.
- Experience/years: 2.0 points maximum.
- Industry/domain: 1.5 points maximum.
- Logistics/location: 1.0 point maximum.
- Compensation: 1.0 point maximum.
- Career-goal alignment: 1.0 point maximum.
For each dimension show awarded points, maximum, posting requirement, candidate evidence, and uncertainty. Give unsupported facts no credit. Unknown salary receives no asserted compensation-match credit; explain how it affects the score. If my profile states no salary minimum, assess compensation against any stated preferences; if there are none, give a neutral 0.5/1 and label it non-discriminating rather than claiming pay is a match. Keep the raw total. Do not round a below-threshold score up to qualify. Use my minimum, default 8.5. A failed indispensable requirement excludes a job regardless of score. A score is not an ATS score, interview probability, or offer probability.

SWOT AND ATS
For each qualifying role, give concise Strengths, Weaknesses, Opportunities, and Threats, explaining which are facts and which are judgments. Extract exact meaningful ATS keywords from the posting. Map each to supported candidate evidence or label the gap. Do not insert unsupported tools or skills just to match keywords.

RESUME
Create each tailored resume from my master resume and confirmed proof points. Preserve truthful employers, dates, degree status, credentials, metrics, and actual skill proficiency. Reorder and rewrite supported material around this job. Distinguish academic work from professional deployments and contribution from sole ownership. Use the master resume's single-column layout, typography hierarchy, headings, margins, and spacing as the reference. Follow my profile's page-length setting. Fill the chosen page length naturally where supported material permits; do not add filler, duplicate bullets, or unreadably small text. Preserve the original source file.
When document tools are available, deliver an actual role-specific DOCX. Render and visually inspect every final page before delivery; check overflow and conspicuous whitespace. If creation/rendering is unavailable, provide clearly labeled draft text, report the missing check, and mark the package NEEDS YOUR REVIEW. Do not call text a downloadable DOCX or claim inspection happened without evidence. Create a cover letter when my profile requests one or the posting requires it, using only supported facts.

QA
Perform a separate review of the draft against the posting and source files. Check factual accuracy, evidence for every new/reworded claim, essential requirement coverage, supported ATS terms, readability/layout, score arithmetic, threshold integrity, live posting/link, duplicate status, and source consistency. Revise up to 3 passes without exceeding truthful evidence. A separate pass is a second review, not proof of a separate independent model. Use APPROVED when all relevant checks pass, NEEDS YOUR REVIEW for resolvable gaps or unperformed checks, and REJECT JOB for disqualifying issues. APPROVED still requires my review before applying. Unsupported claims must be removed, not left in a deliverable with a warning.

FINAL PACKAGE
For each complete qualifying package give:
1. Company, title, requisition ID, location/arrangement, verified date, salary/currency or not stated, and deadline or not stated.
2. Original posting URL and verified official application URL.
3. Score components, raw total, threshold, and evidence/uncertainties.
4. SWOT, ATS keywords with evidence, meaningful gaps, and recruiter verdict.
5. QA result, changes made, checks actually completed, and remaining questions.
6. Role-specific resume DOCX when actually created, otherwise labeled draft text; cover letter when requested/required.
7. Saved file references when supported, or explicit instructions for me to save the supplied files/text.
Rank by score, using earlier deadlines to break ties. Deliver fewer packages when fewer qualify. List rejected and held jobs briefly with reasons. If nothing qualifies, explain actual search coverage and why; do not manufacture a match.

TRACKER AND REVIEW
Preserve previous tracker entries and update reviewed jobs, stable keys, verification dates, scores, verdicts, package references, query log, daily counts, and actual run status. Save back to the same accessible tracker when supported and report success only after confirmed save. If saving fails or is unavailable, give a full updated tracker copy, clearly say it was not persisted, and require that copy before another repeat-sensitive run. Mark a scan complete only after all requested queries finish meaningfully; outages are incomplete runs. Mark Applied only when I explicitly confirm submission.

Do not submit applications, send emails, or contact employers/recruiters. Deliver materials to this recruiter chat or its Scheduled results for my review. End with actual counts, access limitations, tracker-save status, and anything I need to resolve.
```

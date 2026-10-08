# Schedule prompt

Use this after a successful manual test, in the same chat containing your profile, sources, and complete daily-run prompt. This file is a request to create a task; copying it alone does not activate anything.

```text
Create a recurring task named Daily Recruiter Run using the complete daily-run instructions I tested in this chat, with my confirmed Candidate_Profile.md run settings. Return to this recruiter chat on each run when supported. Use the daily local time and IANA timezone in my profile; the default is 9:00 a.m. America/New_York every day.

Use the full workflow prompt, not a summary reminder to search for jobs. Include the verified private source-file manifest in the saved instructions, the score rubric and threshold, deduplication against the same tracker and accessible artifacts, truthful master-resume tailoring, actual QA checks, package limits, tracker persistence rules, and my review requirement. Remove any one-run test-mode override from the saved task. Required files must be accessible during scheduled runs; do not depend on transient local paths or assume attachments are available without checking. If a required external app is involved, verify read access before scheduling.

Check whether a Daily Recruiter Run already exists for this workflow. Update the matching task instead of creating a duplicate; ask if multiple candidates cannot be distinguished. Preserve unrelated tasks.

If scheduling or required source access is unavailable, explain the blocker and do not claim a task was created. Do not create a reminder in place of the full workflow without telling me.

After a successful create/update, confirm the task name, daily local time, IANA timezone, enabled status, saved workflow scope, source locations, result destination, and next run when available. Tell me to verify the task in Scheduled and inspect its first run for file access, tracker persistence, and document quality.

Prepare materials for my review. Do not submit applications, send emails, or contact employers/recruiters.
```

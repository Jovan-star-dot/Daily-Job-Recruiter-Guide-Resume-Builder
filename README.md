# Daily Job Recruiter Guide & Resume Builder

Create your own daily job-search assistant using ChatGPT. Add your resume and preferences, then use the included prompts to find relevant openings, assess fit, prepare truthful application materials, and review them before applying.

Created by Jovan A. Diaz. Adapted from his Daily Recruiter Run; this starter kit contains blank candidate templates rather than his private information.

## Start here

1. Read [START_HERE.md](START_HERE.md).
2. Download this repository: **Code → Download ZIP**, then unzip it.
3. Fill in [Candidate_Profile.md](templates/Candidate_Profile.md) on your own computer.
4. Upload your completed profile and master resume to your own ChatGPT recruiter chat.
5. Paste the [setup prompt](prompts/01_setup.md), followed by the [daily run prompt](prompts/02_daily_run.md).
6. Test the results, then use the [schedule prompt](prompts/03_schedule.md).

You do not need Python, an API key, n8n, Zapier, or GitHub Actions for this guide. GitHub holds the guide; ChatGPT performs the searches and document work when the necessary features are available on your account. Downloading these files does not activate an automation.

## What the workflow does

Scheduled Search → Verify Job → Deduplicate → Hard Filter → Score → SWOT/ATS → Resume → QA → Final Package → Your Review

The default match threshold is **8.5/10**, and the default schedule is **9:00 a.m. America/New_York**. You can change these in your candidate profile. The match score is a judgment about fit, not an ATS score or probability of getting an interview.

Every resume starts from your master resume. The assistant must preserve supported facts, match its layout, and avoid inventing experience or achievements. Applications remain your responsibility; the prompts do not authorize contacting recruiters or submitting applications.

## Files you will use

| File | Purpose |
| --- | --- |
| [START_HERE.md](START_HERE.md) | Complete setup instructions |
| [Candidate_Profile.md](templates/Candidate_Profile.md) | The only form you need to fill in initially |
| [01_setup.md](prompts/01_setup.md) | Check your inputs and create supporting files |
| [02_daily_run.md](prompts/02_daily_run.md) | Run the full recruiter workflow |
| [03_schedule.md](prompts/03_schedule.md) | Create the recurring task after testing |
| [04_build_one_resume.md](prompts/04_build_one_resume.md) | Tailor a resume for a job you already found |
| [05_review_package.md](prompts/05_review_package.md) | Check an application package before using it |
| [Job_Tracker.md](templates/Job_Tracker.md) | Record reviewed jobs and avoid repeat packages |
| [workflow.md](docs/workflow.md) | Stage definitions and scoring rubric |
| [troubleshooting.md](docs/troubleshooting.md) | Fix missing files, duplicate jobs, and weak results |
| [publish_to_github.md](docs/publish_to_github.md) | Upload or share this guide |

The additional Job Preferences, Career Goals, and Proof Points templates are optional. The setup prompt can create completed copies from your single candidate profile.

## Sharing the guide

Share the repository link or an unmodified copy of this starter kit. Each person supplies their own resume and profile in their own private workspace. Keep personal resumes, completed profiles, trackers, and application packages out of the shared repository. The included `.gitignore` covers the recommended `private/` and `outputs/` folders if you use Git; browser uploads still require choosing the correct files.

## Product documentation

Scheduling guidance was checked on October 8, 2026: [OpenAI — Scheduled tasks](https://learn.chatgpt.com/docs/automations). Feature availability depends on your account and workspace. Use the manual run prompt if scheduling or document generation is unavailable. This kit provides prompts and instructions; it does not guarantee that a particular account can complete unattended document creation or tracker updates.

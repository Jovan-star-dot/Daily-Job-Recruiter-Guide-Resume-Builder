# Create your Daily Recruiter Run

You will need your own ChatGPT account, an accurate master resume, and a few minutes to describe the jobs you want. Use an account that can search the web and work with uploaded files. Recurring runs also require scheduled tasks to be available in your account or workspace.

## Step 1 — Download the starter kit

On GitHub, choose **Code → Download ZIP**, then unzip the download. You can use these files without creating your own GitHub repository.

Markdown (`.md`) files are plain text. Open them in a text editor to make changes, or copy their contents into a document. If you use macOS TextEdit, choose **Format → Make Plain Text** before saving a `.md` file.

## Step 2 — Add your information

Open `templates/Candidate_Profile.md`. Replace each `[YOUR ...]` entry with your own information. Use `unknown`, `no preference`, or `not applicable` where appropriate. Do not let the assistant guess essential eligibility information.

Save your completed copy in a folder named `private` on your computer. Keep the blank template unchanged for anyone else who wants to use the guide.

The form asks for:

- Target roles and level, preferred industries, locations, and work arrangement.
- Salary preferences, work authorization, sponsorship needs, and availability.
- Deal-breakers, career goals, and verified achievements or projects.
- Search breadth, number of packages, score threshold, and schedule.
- The resume length and formatting you want.

The defaults are a 9:00 a.m. New York run, 20 distinct search queries, up to 10 complete packages, and an 8.5/10 threshold. These are limits and settings, not guaranteed output counts. The active workflow this kit adapts used the 8.5 threshold; the query and package limits make search breadth configurable.

## Step 3 — Prepare your master resume

Use the resume that most accurately describes your experience. Name your working copy `Master_Resume_ATS.docx`. An editable DOCX is best for preserving layout. You can also upload a PDF as a visual reference.

Check employment dates, degree status and expected graduation date, tools, certifications, and metrics. Label academic projects as academic projects. Add accomplishments that are absent from your resume to the Proof Points section of your profile, with enough detail to verify which role or project they belong to.

If you only have a PDF or resume text, you can still test search and resume drafting. Ask for a new editable document and inspect it before use; exact formatting preservation may require an editable source.

## Step 4 — Create your recruiter chat

Open a new ChatGPT chat and name it **My Daily Recruiter Run**. Upload:

1. Your completed `Candidate_Profile.md`.
2. Your `Master_Resume_ATS.docx`.
3. The blank `templates/Job_Tracker.md`, or your existing tracker if you already use one.
4. Your optional resume PDF or cover-letter template.

Use your own chat rather than another person's shared conversation. A link to this GitHub guide does not give the assistant access to files on your computer.

## Step 5 — Check the setup

Open `prompts/01_setup.md`, copy the entire fenced prompt, and paste it into the chat. The assistant will check your inputs, identify missing essential information, and prepare Job Preferences, Career Goals, and Proof Points files from your profile.

Review those files. Correct any mistake before searching. Save the completed source files somewhere future runs can access, and reattach them if the assistant cannot read them. Use the source manifest produced by the setup prompt to record their exact names and, where available, persistent references. Do not assume conversation memory contains your complete resume.

## Step 6 — Run a small manual test

Paste the prompt in `prompts/02_daily_run.md`. Add this line above it for the first test:

> Test mode for this run only: use 5 distinct searches and deliver at most 2 complete packages. Keep my match threshold and all verification rules unchanged.

Review at least one real job against the employer's posting. Check that the assistant:

- Finds openings matching your actual location and eligibility.
- Reads requirements and verifies a working application link.
- Shows its score breakdown and cites evidence from your resume.
- Identifies gaps instead of inventing qualifications.
- Produces a readable resume based on your master resume.
- Updates the tracker, or explicitly provides an updated copy for you to save.

If no job qualifies, check the search coverage and filters before changing settings. An empty result is valid when verified roles do not meet the threshold. Failed searches must be reported as failures.

## Step 7 — Schedule the daily run

After the manual test succeeds, paste the prompt from `prompts/03_schedule.md` into the same recruiter chat. It tells the assistant to use the full daily run prompt and your confirmed settings.

Review the actual task confirmation: name, saved instructions, daily time, IANA timezone, accessible source files, and result destination. Open **Scheduled** to confirm the task exists and is active. A statement such as “I will do this daily” is not evidence that a scheduled task was created.

The scheduled time starts the work; searching and preparing files can finish later. Verify source-file access on the first scheduled run. If unattended runs cannot generate documents or safely update the tracker, have them produce the verified shortlist and finish packages manually with `prompts/04_build_one_resume.md`.

Official OpenAI documentation describes web scheduled tasks as using accessible uploads and connected tools rather than a local computer folder. It recommends testing the prompt manually before scheduling. Desktop tasks that need local files require the computer and app to be running. See [Scheduled tasks](https://learn.chatgpt.com/docs/automations), checked October 8, 2026.

## Step 8 — Review and apply

For each delivered package, read the live posting, check your tailored resume, resolve eligibility questions, and use the application link yourself. The assistant should mark a job `Applied` only after you explicitly report submitting it.

Use `prompts/05_review_package.md` when you want a fresh QA pass. Update your tracker with application dates and outcomes.

## Step 9 — Maintain the workflow

Update your profile and source files when your preferences, qualifications, or availability change. Ask the assistant to update the saved task instructions and confirm the change. Review the first few scheduled runs for relevance, missing files, repeated jobs, and document quality.

To pause or delete the automation, use **Scheduled**. Downloading, copying, or deleting this guide does not change an existing task.

## Only need one resume?

Upload your master resume, profile, and the full job description. Paste `prompts/04_build_one_resume.md`. You do not need a daily automation to use the resume builder.

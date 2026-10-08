# Troubleshooting

| Problem | What to do |
| --- | --- |
| The assistant cannot read my resume | Upload the editable source again and confirm the exact filename; stop tailoring until it can read the source. |
| Search is unavailable | Use the one-resume prompt with a full job description; it must label current job status unverified. |
| The same jobs keep returning | Reattach the latest tracker; check requisition IDs and canonical URLs; also check existing packages. |
| No jobs qualify | Inspect query coverage, hard filters, and score evidence. Change only preferences you actually want to change. |
| All searches failed but it says no matches | Ask it to mark the run incomplete and show actual failures. |
| Remote jobs require another country | Add eligible remote-work countries and authorization details to your profile. |
| Resume has invented skills or metrics | Remove them, then run the review prompt against source evidence. |
| Resume leaves half the page empty | Ask it to match the master resume's spacing and use more supported relevant accomplishments; inspect the rendered page. |
| Resume spills onto another page | Ask it to reduce duplication and lower-priority content while preserving readable text. |
| DOCX or rendering tools are unavailable | Use labeled draft text, paste into your own resume document, and perform layout checks yourself. |
| The automation claims it will run but no task exists | Open Scheduled and verify the actual task and enabled status. |
| Scheduled is unavailable on my account | Run the daily prompt manually when you want a search. |
| Scheduled runs lose my sources | Update the task with accessible source references and test again; do not rely on temporary paths. |
| Tracker save failed | Save the full updated copy and reattach it before the next run. |
| Multiple tasks do the same search | Pause the duplicate after checking which task has the current instructions. |
| I moved or my job preferences changed | Update the profile and saved task; verify local time, IANA timezone, and filters. |
| Someone cannot open the GitHub guide | A private repository needs collaborator access. Use the downloadable kit or a repository containing only the shareable templates. |

Useful correction prompt:

> Re-read my candidate profile, master resume, and latest tracker. Explain the specific issue, correct it using supported facts, and tell me which checks you actually completed. Do not claim an action succeeded unless it did.

Product guidance: [OpenAI — Scheduled tasks](https://learn.chatgpt.com/docs/automations). Availability and interfaces can change; checked October 8, 2026.

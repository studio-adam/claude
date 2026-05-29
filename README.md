# PM Interviewer (Claude skill)

A Claude skill that runs realistic, workshop-style mock product manager interviews and coaches
you live. It covers three formats:

- **Process and execution**: how would you build and ship feature X. You give it the role,
  company, and the interviewer's LinkedIn; it researches the interviewer's domain and builds a
  case from it.
- **Zero to one**: should we build X, and what is the smallest version. You give it the company
  and any pre-read; it grounds the case in the company's mission and existing users.
- **Data science / working with DS**: how a PM partners with data. Covers using data to
  influence, defining metrics, resolving disagreements with data scientists, decisions under
  incomplete data, and debugging metric drops. Mostly behavioral and framework-based, less
  case-shaped.

When you start, it presents the three formats so you can pick (one tap if your client supports
it, otherwise a numbered list). Once you pick, it gathers the right inputs for that format,
researches as needed, and runs the round.

During the session it pushes one probe at a time, hands the segment and problem back to you to
define, corrects weak moves in the moment, and ends with a structured feedback summary:
overall verdict, what was strong (with specific moments), the two or three habits to fix, the
single most important fix, and forward-looking advice for the next round.

## Install

**Claude (web / desktop), on Pro, Max, Team, or Enterprise:**
1. Open Settings and find Skills (or click the "+" in a chat, then "+ Create skill").
2. Upload `pm-interviewer.zip`.
3. Toggle the skill on. Then in any chat say "interview me," "practice a case," "run a zero
   to one mock," or "prep me for a data science round."

**Claude Code:**
```bash
git clone <this-repo-url> ~/.claude/skills/pm-interviewer
# or, to share inside a project, commit the folder to .claude/skills/pm-interviewer
```
Anyone who clones the project then has the skill automatically.

## Sharing with others

- Custom skills are private to each account, so each person installs their own copy.
- Easiest: share this repo link (or the `pm-interviewer.zip` file). Each person downloads and
  uploads it once.
- Inside one organization on Team or Enterprise: an owner can enable sharing in Organization
  settings > Skills, then share it with colleagues or org-wide.

## Files

- `pm-interviewer/SKILL.md` — the skill itself.
- `pm-interviewer.zip` — zipped folder for uploading to Claude on the web.
- `pm-interviewer.skill` — packaged format (for environments that take a `.skill` file).

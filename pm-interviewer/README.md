# PM Interviewer (Claude skill)

A Claude skill that runs realistic, workshop-style mock product manager interviews and coaches
you live. It covers two formats:

- **Process and execution**: how would you build and ship feature X. You give it the role,
  company, and the interviewer's LinkedIn; it researches the interviewer's domain and builds a
  case from it.
- **Zero to one**: should we build X, and what is the smallest version. You give it the company
  and any pre-read; it grounds the case in the company's mission and existing users.

It pushes one probe at a time, hands the segment and problem back to you to define, corrects
weak moves in the moment, and ends with an overall read plus the habits to fix.

## Install

**Claude (web / desktop), on Pro, Max, Team, or Enterprise:**
1. Open Settings and find Skills (or click the "+" in a chat, then "+ Create skill").
2. Upload `pm-interviewer.zip`.
3. Toggle the skill on. Then in any chat say "interview me for a process and execution case" or
   "run a zero to one mock for me."

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
- `pm-interviewer.skill` — packaged format (for environments that take a .skill file).

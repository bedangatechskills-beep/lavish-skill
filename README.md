# Lavish — a Claude Code skill

Turns complex or visual agent responses into rich, reviewable HTML pages you can annotate and send
feedback on. Claude reaches for it when a plan, comparison, diagram, table, code diff or report is
easier to grasp as a page than as prose.

The skill is by [Kun Chen (kunchenguid)](https://github.com/kunchenguid) and is MIT licensed. It drives
the `lavish-axi` CLI through `npx`, so you need Node.js installed, but nothing has to be installed globally.

## Install

Copy the `lavish` folder into your personal Claude Code skills folder:

| OS | Destination |
|----|-------------|
| Windows | `%USERPROFILE%\.claude\skills\lavish\` |
| macOS / Linux | `~/.claude/skills/lavish/` |

**Quick install (macOS / Linux / Git Bash):**
```bash
git clone https://github.com/bedangatechskills-beep/lavish-skill.git
mkdir -p ~/.claude/skills && cp -r lavish-skill/lavish ~/.claude/skills/
```

**Quick install (Windows PowerShell):**
```powershell
git clone https://github.com/bedangatechskills-beep/lavish-skill.git
New-Item -ItemType Directory -Force "$env:USERPROFILE\.claude\skills" | Out-Null
Copy-Item -Recurse lavish-skill\lavish "$env:USERPROFILE\.claude\skills\"
```

Restart Claude Code, then check it shows up under `/skills`.

## Use

Type `/lavish <what the page should show>`, or just ask for a plan, comparison or report and let Claude
decide a page is clearer than prose.

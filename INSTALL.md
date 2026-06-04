# Installation Guide

## Option A: One-Command Install (macOS / Linux)

```bash
mkdir -p ~/.claude/skills && cp skills/*.md ~/.claude/skills/ && echo "✅ 12 skills installed"
```

## Option B: Manual Install (Windows)

1. Open File Explorer
2. Navigate to `C:\Users\[YourName]\.claude\`
3. Create a `skills` folder if it doesn't exist
4. Copy all `.md` files from the `skills/` folder into `~\.claude\skills\`

## Option C: Add to a Specific Project

If you want these skills only for one project:

```bash
cd /path/to/your/project
mkdir -p .claude/skills
cp /path/to/ecom-ai-toolkit/skills/*.md .claude/skills/
```

## Verify Installation

In Claude Code:
```
/skills
```
You should see all 12 skills listed.

## Troubleshooting

**Skills not showing up?**
- Verify files are in `~/.claude/skills/` (global) or `.claude/skills/` (project)
- Restart Claude Code after copying files
- Check file extension is `.md` not `.md.txt`

**Skill not triggering automatically?**
- You can always invoke manually: `Use the [skill-name] skill to...`
- Or wait for Claude to suggest it when relevant

## Updating Skills

To update to the latest version:
```bash
cd ecom-ai-toolkit
git pull
cp skills/*.md ~/.claude/skills/
```

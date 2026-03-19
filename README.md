<div align="center">

# vibe-ship

**A guided development workflow for non-coders — from idea to shipped product**

[![Claude Code](https://img.shields.io/badge/Claude_Code-Skill-blueviolet?logo=anthropic&logoColor=white)](https://claude.ai/claude-code)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

[中文版](README.zh.md)

</div>

---

## What is vibe-ship?

vibe-ship is a Claude Code skill that guides you through building and shipping software — step by step, through questions — even if you've never written a line of code.

It was distilled from three real projects ([Rockpile](https://github.com/nicekate/Rockpile), [Spottt](https://github.com/ar-gen-tin/spottt), [odds](https://github.com/ar-gen-tin/odds)), 60+ bugs, two full tech stack rewrites, and one repository nuke-and-rebuild.

One rule: **follow the order, don't skip steps.**

---

## The 8 Steps

```
Define → Tech Stack → MVP → Ship Path → Security → Design → Cut Features → Log Pitfalls
 [1]       [2]        [3]     [4]         [5]       [6]        [7]            [8]
```

| Step | What happens |
|------|-------------|
| 1. **Define before you type** | Who is this for? One core feature? What's the closest existing product? |
| 2. **Ask about tech stack** | What to build with? Why? Are there better options? |
| 3. **Ugliest working version** | Core feature only. No design, no i18n, no extras. |
| 4. **Walk the ship path** | Signing, packaging, deployment — do it early, not last. |
| 5. **Security scan** | Check for leaked keys, emails, local paths before pushing. Cannot skip. |
| 6. **Now do design** | 3 directions max. Pick one, commit. |
| 7. **Cut features** | "Does the product still work without this?" If yes, don't build it. |
| 8. **Log everything** | AI has no memory. You keep the notes for next time. |

---

## Install

```bash
# Clone into your Claude Code skills directory
git clone https://github.com/ar-gen-tin/vibe-ship.git ~/.claude/skills/vibe-ship
```

Or manually copy `SKILL.md` to `~/.claude/skills/vibe-ship/`.

## Usage

```bash
/vibe-ship              # Start from Step 1
/vibe-ship --status     # Check progress
```

---

## What it does

- Asks you questions at every step — waits for your answer before moving on
- Parks feature requests in a "later list" — reviewed only at Step 7
- Security scan at Step 5 is mandatory
- Translates all technical jargon into plain language
- After MVP: suggests running `/code-review` for a quality check
- Before shipping: optionally run `/team` for multi-perspective review

## What it doesn't do

- Doesn't teach you to code
- Doesn't make product decisions for you (but helps you think clearly)
- Doesn't generate boilerplate projects

---

## License

MIT

---

Don't Panic. Accelerate.

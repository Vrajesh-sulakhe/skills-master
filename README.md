# Skills Master

A centralized, production-grade repository for managing, scaffolding, and auto-routing AI agent skills, plugins, and master execution protocols in **Google Antigravity IDE** and **Gemini CLI**.

---

## 🌟 Overview

`skills-master` provides a unified system architecture for AI coding agents:
1. **Mandatory Meta-Workflows**: Unconditional auto-triggering protocols (via [Superpowers](https://github.com/obra/superpowers)) enforcing TDD, systematic debugging, and verification before completion.
2. **Master Routing Catalogs**: Consolidates over 3,500+ skills into streamlined master entry points:
   - [`get-shit-done`](.agents/skills/get-shit-done/SKILL.md): Master router for all 72 GSD Core spec-driven development skills.
   - [`bootstrap-all-rounder`](.agents/skills/bootstrap-all-rounder/SKILL.md): Master router for all 11 official Bootstrap framework skills.
3. **Autonomous Loops**: Fully configured integration with [Ralph Loop for Antigravity](https://github.com/abhishekbhakat/ralph-loop-for-antigravity) driven by `PRD.md`, `progress.txt`, and `prompt.md`.

---

## 📁 Repository Structure

```text
skills-master/
├── .agent/
│   └── skills/                  # Local project skills
│       ├── brainstorming/       # Visual brainstorming and companion server
│       ├── brand-identity/      # Design tokens, typography & voice-and-tone
│       └── writing-plans/       # Step-by-step implementation plan authoring
├── .agents/
│   └── skills/                  # Installed & consolidated master skills
│       ├── bootstrap-all-rounder/ # Master Bootstrap router (11 skills)
│       └── get-shit-done/       # Master GSD Core router (72 skills)
├── .vscode/
│   └── settings.json            # Ralph Loop workspace configuration
├── antigravity-skill-creator.md # System prompt for authoring new Antigravity skills
├── github-links.md              # Curated directory of all source repositories & skills
├── PRD.md                       # Task specification file for autonomous Ralph Loop
├── progress.txt                 # Iteration log for autonomous Ralph Loop
├── prompt.md                    # Mandatory Superpowers auto-trigger system prompt
└── skills-lock.json             # Skill dependency lockfile
```

---

## 🚀 Quick Reference

- **[Curated GitHub Repositories](github-links.md)**: Complete list of all 18 source GitHub repositories with descriptions, install commands, and included skills.
- **[Mandatory Superpowers Prompt](prompt.md)**: The production system prompt forcing the AI agent to evaluate every prompt through `using-superpowers`.
- **[Skill Authoring Guide](antigravity-skill-creator.md)**: Specifications and instructions for generating standard `.agent/skills/<skill-name>/SKILL.md` packages.

---

## ⚡ Superpowers Execution Protocol

All agent interactions follow the strict zero-bypass routing protocol:

```text
Incoming Prompt ──> Auto-Trigger `using-superpowers`
                        │
                        ├──> Build / Feature  ──> `brainstorming`
                        ├──> Planning / Specs ──> `writing-plans`
                        ├──> Bug / Error      ──> `systematic-debugging`
                        ├──> Implementation   ──> `test-driven-development`
                        └──> Sign-off / Done  ──> `verification-before-completion`
```

---

## 🛠️ Requirements & Tooling

- [Antigravity IDE](https://antigravity.google) / Gemini CLI (`agy`)
- [GitHub CLI (`gh`)](https://cli.github.com)
- [Ralph Loop for Antigravity](https://github.com/abhishekbhakat/ralph-loop-for-antigravity)

---

## 📄 License

MIT

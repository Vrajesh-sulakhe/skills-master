# Skills Master

A centralized, production-grade repository for managing, scaffolding, and auto-routing AI agent skills, plugins, and master execution protocols in **Google Antigravity IDE** and **Gemini CLI**.

---

## 🌟 Overview

`skills-master` provides a unified system architecture for AI coding assistants and autonomous agents:

1. **Two-Tier Autonomous Routing**:
   - **Tier 1 (Mandatory Meta-Workflow)**: Unconditional auto-triggering protocols (via [Superpowers](https://github.com/obra/superpowers)) enforcing TDD, systematic debugging, bite-sized planning, and verification before completion on **every single user prompt**.
   - **Tier 2 (Universal Domain Skill Auto-Triggering)**: Automatically analyzes prompt intent and activates the corresponding specialized skill from a 3,500+ global library across **all projects (past, current, and upcoming)**.
2. **Master Routing Catalogs**: Consolidates large skill frameworks into streamlined master entry points:
   - [`get-shit-done`](.agents/skills/get-shit-done/SKILL.md): Master router for all 72 GSD Core spec-driven development skills.
   - [`bootstrap-all-rounder`](.agents/skills/bootstrap-all-rounder/SKILL.md): Master router for all 11 official Bootstrap framework skills.
3. **Autonomous Execution Loops**: Fully configured integration with [Ralph Loop for Antigravity](https://github.com/abhishekbhakat/ralph-loop-for-antigravity) driven by `PRD.md`, `progress.txt`, and `prompt.md`.

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
├── prompt.md                    # Two-tier global autonomous routing system prompt
└── skills-lock.json             # Skill dependency lockfile
```

---

## 🚀 Quick Reference

- **[Two-Tier Global Autonomous Prompt](prompt.md)**: The production system prompt mandating `using-superpowers` on every prompt and dynamic global skill resolution across all projects.
- **[Curated GitHub Repositories](github-links.md)**: Complete list of all 18 source GitHub repositories with descriptions, install commands, and included skills.
- **[Skill Authoring Guide](antigravity-skill-creator.md)**: Specifications and instructions for generating standard `.agent/skills/<skill-name>/SKILL.md` packages.

---

## ⚡ Two-Tier Execution Protocol

All agent interactions follow this strict zero-bypass routing protocol:

```text
Incoming Prompt ──> Tier 1: Auto-Trigger `using-superpowers` (Mandatory Process)
                        │
                        ├──> Build / Feature  ──> `brainstorming`
                        ├──> Planning / Specs ──> `writing-plans`
                        ├──> Bug / Error      ──> `systematic-debugging`
                        ├──> Implementation   ──> `test-driven-development`
                        └──> Sign-off / Done  ──> `verification-before-completion`
                                │
                                └──> Tier 2: Dynamic Prompt Analysis (Domain Skill)
                                         ├──> Specs/GSD ──> `get-shit-done`
                                         ├──> Bootstrap ──> `bootstrap-all-rounder`
                                         ├──> Fullstack ──> `app-builder`
                                         ├──> UI / UX   ──> `ui-ux-pro-max` / `superdesign`
                                         ├──> Security  ──> `ethical-hacking-methodology`
                                         └──> Reverse   ──> `reverse-engineer-anything`
```

---

## 🛠️ Requirements & Tooling

- [Antigravity IDE](https://antigravity.google) / Gemini CLI (`agy`)
- [GitHub CLI (`gh`)](https://cli.github.com)
- [Ralph Loop for Antigravity](https://github.com/abhishekbhakat/ralph-loop-for-antigravity)

---

## 📄 License

MIT

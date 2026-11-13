---
name: get-shit-done
description: Master unified router and guide for all 72 Get Shit Done (GSD Core) skills. Use whenever starting projects, planning phases, executing with atomic commits, conducting UAT verification, or managing .planning/ workflows.
---

# Get Shit Done (GSD) — Master Unified Skill

The single global entry point and master router for the entire **GSD Core** framework (72 specialized skills). GSD turns vague goals into shipped software through an explicit, resumable loop: **explore → plan → execute → verify → ship**.

All project state is tracked deterministically in `.planning/` files with atomic commits, verification loops, and context isolation.

---

## When to Use This Skill
- Initializing a new project or onboarding an existing codebase into GSD.
- Planning, scoping, or discussing milestones and phases (`.planning/phases/`).
- Executing plans with wave-based parallelism, atomic commits, and deviation rules.
- Running conversational User Acceptance Testing (UAT) and quality gates.
- Managing persistent context threads, workstreams, or multi-phase roadmaps.
- Quick bug fixes, fast tasks, or codebase knowledge graph extraction.

---

## GSD Master Lifecycle Routing Matrix

Inspect and load the specific submodule via `read_file` based on your current phase:

### 1. Core Phase Execution & Delivery

- **[`gsd-next`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-next/SKILL.md)**: Smart entry — detect project state and route to the right next GSD action.
- **[`gsd-progress`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-progress/SKILL.md)**: Check progress, advance workflow, or dispatch freeform intent — the unified GSD situational command
- **[`gsd-discuss-phase`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-discuss-phase/SKILL.md)**: Gather phase context through adaptive questioning before planning.
- **[`gsd-spec-phase`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-spec-phase/SKILL.md)**: Clarify WHAT a phase delivers with ambiguity scoring; produces a SPEC.md before discuss-phase.
- **[`gsd-plan-phase`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-plan-phase/SKILL.md)**: Create detailed phase plan (PLAN.md) with verification loop
- **[`gsd-ultraplan-phase`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-ultraplan-phase/SKILL.md)**: [BETA] Offload plan phase to Claude Code's ultraplan cloud; review in browser and import back.
- **[`gsd-mvp-phase`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-mvp-phase/SKILL.md)**: Plan a phase as a vertical MVP slice — user story, SPIDR splitting, then plan-phase
- **[`gsd-ai-integration-phase`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-ai-integration-phase/SKILL.md)**: Generate an AI-SPEC.md design contract for phases that involve building AI systems.
- **[`gsd-ui-phase`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-ui-phase/SKILL.md)**: Generate UI design contract (UI-SPEC.md) for frontend phases
- **[`gsd-plan-review-convergence`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-plan-review-convergence/SKILL.md)**: Cross-AI plan convergence - replan until review concerns are resolved.
- **[`gsd-execute-phase`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-execute-phase/SKILL.md)**: SDD phase execution — execute all plans in a phase with dependency-aware wave parallelization
- **[`gsd-autonomous`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-autonomous/SKILL.md)**: Run all remaining phases autonomously — discuss→plan→execute per phase
- **[`gsd-verify-work`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-verify-work/SKILL.md)**: Validate built features through conversational UAT
- **[`gsd-validate-phase`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-validate-phase/SKILL.md)**: Retroactively audit and fill Nyquist validation gaps for a completed phase
- **[`gsd-ship`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-ship/SKILL.md)**: Create PR, run review, and prepare for merge after verification passes

### 2. Project & Milestone Lifecycle

- **[`gsd-new-project`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-new-project/SKILL.md)**: Initialize a new project with deep context gathering and PROJECT.md
- **[`gsd-onboard`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-onboard/SKILL.md)**: Guide existing codebase onboarding through mapping, doc ingest, and planning setup
- **[`gsd-phase`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-phase/SKILL.md)**: Multi-phase management — add, insert, remove, or edit phases in ROADMAP.md (roadmap phase CRUD)
- **[`gsd-new-milestone`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-new-milestone/SKILL.md)**: Start a new milestone cycle — update PROJECT.md and route to requirements
- **[`gsd-complete-milestone`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-complete-milestone/SKILL.md)**: Archive completed milestone and prepare for next version
- **[`gsd-audit-milestone`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-audit-milestone/SKILL.md)**: Audit milestone completion against original intent before archiving
- **[`gsd-milestone-summary`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-milestone-summary/SKILL.md)**: Generate a comprehensive project summary from milestone artifacts for team onboarding and review
- **[`gsd-cleanup`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-cleanup/SKILL.md)**: Archive accumulated phase directories from completed milestones
- **[`gsd-stats`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-stats/SKILL.md)**: Display project statistics — phases, plans, requirements, git metrics, and timeline
- **[`gsd-health`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-health/SKILL.md)**: Diagnose planning directory health and optionally repair issues

### 3. Ideation & Exploration

- **[`gsd-explore`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-explore/SKILL.md)**: Socratic ideation and idea routing — think through ideas before committing to plans
- **[`gsd-sketch`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-sketch/SKILL.md)**: Sketch UI/design ideas with throwaway HTML mockups, or propose what to sketch next (frontier mode)
- **[`gsd-spike`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-spike/SKILL.md)**: Spike an idea through experiential exploration, or propose what to spike next (frontier mode)
- **[`gsd-capture`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-capture/SKILL.md)**: Capture ideas, tasks, notes, and seeds to their destination

### 4. Quality Gates, Reviews & Debugging

- **[`gsd-code-review`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-code-review/SKILL.md)**: Review source files changed during a phase for bugs, security issues, and code quality problems
- **[`gsd-debug`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-debug/SKILL.md)**: Systematic debugging with persistent state across context resets
- **[`gsd-audit-fix`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-audit-fix/SKILL.md)**: Autonomous audit-to-fix pipeline — find issues, classify, fix, test, commit
- **[`gsd-audit-uat`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-audit-uat/SKILL.md)**: Cross-phase audit of all outstanding UAT and verification items
- **[`gsd-add-tests`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-add-tests/SKILL.md)**: Generate tests for a completed phase based on UAT criteria and implementation
- **[`gsd-secure-phase`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-secure-phase/SKILL.md)**: Retroactively verify threat mitigations for a completed phase
- **[`gsd-ui-review`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-ui-review/SKILL.md)**: Retroactive 6-pillar visual audit of implemented frontend code
- **[`gsd-eval-review`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-eval-review/SKILL.md)**: Audit an executed AI phase's evaluation coverage and produce an EVAL-REVIEW.md remediation plan.
- **[`gsd-review`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-review/SKILL.md)**: Request cross-AI peer review of phase plans from external AI CLIs
- **[`gsd-forensics`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-forensics/SKILL.md)**: Post-mortem investigation for failed GSD workflows — diagnoses what went wrong.

### 5. Codebase Intelligence & Knowledge Graph

- **[`gsd-map-codebase`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-map-codebase/SKILL.md)**: Analyze codebase with parallel mapper agents to produce .planning/codebase/ documents
- **[`gsd-graphify`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-graphify/SKILL.md)**: Build, query, and inspect the project knowledge graph in .planning/graphs/
- **[`gsd-docs-update`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-docs-update/SKILL.md)**: Generate or update project documentation verified against the codebase
- **[`gsd-ingest-docs`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-ingest-docs/SKILL.md)**: Bootstrap or merge a .planning/ setup from existing ADRs, PRDs, SPECs, and docs in a repo.
- **[`gsd-extract-learnings`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-extract-learnings/SKILL.md)**: Extract decisions, lessons, patterns, and surprises from completed phase artifacts
- **[`gsd-mempalace-capture`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-mempalace-capture/SKILL.md)**: File a phase artifact into MemPalace; mirror decision facts into its temporal KG
- **[`gsd-mempalace-recall`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-mempalace-recall/SKILL.md)**: Recall decisions, patterns, and surprises from MemPalace before planning
- **[`gsd-profile-user`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-profile-user/SKILL.md)**: Generate developer behavioral profile and create Claude-discoverable artifacts

### 6. Fast Inline Execution

- **[`gsd-quick`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-quick/SKILL.md)**: Execute a quick task with GSD guarantees (atomic commits, state tracking) but skip optional agents
- **[`gsd-quick-batch`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-quick-batch/SKILL.md)**: Batch several `/gsd-quick`-shaped tasks together — planned, dispatched, and merged as one run
- **[`gsd-fast`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-fast/SKILL.md)**: Execute a trivial task inline — no subagents, no planning overhead

### 7. Workspace, Workstreams & Session Management

- **[`gsd-workspace`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-workspace/SKILL.md)**: Manage GSD workspaces — create, list, or remove isolated workspace environments
- **[`gsd-workstreams`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-workstreams/SKILL.md)**: Manage parallel workstreams — list, create, switch, status, progress, complete, and resume
- **[`gsd-thread`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-thread/SKILL.md)**: Manage persistent context threads for cross-session work
- **[`gsd-pause-work`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-pause-work/SKILL.md)**: Create context handoff when pausing work mid-phase
- **[`gsd-resume-work`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-resume-work/SKILL.md)**: Resume work from previous session with full context restoration
- **[`gsd-pr-branch`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-pr-branch/SKILL.md)**: Create a clean PR branch by filtering out .planning/ commits — ready for code review
- **[`gsd-undo`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-undo/SKILL.md)**: Safe git revert. Roll back phase or plan commits using the phase manifest with dependency checks.
- **[`gsd-inbox`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-inbox/SKILL.md)**: Triage and review open GitHub issues and PRs against project templates and contribution guidelines.
- **[`gsd-review-backlog`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-review-backlog/SKILL.md)**: Review and promote backlog items to active milestone
- **[`gsd-settings`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-settings/SKILL.md)**: Configure GSD workflow toggles and model profile
- **[`gsd-config`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-config/SKILL.md)**: Configure GSD settings — workflow toggles, advanced knobs, integrations, and model profile
- **[`gsd-surface`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-surface/SKILL.md)**: Toggle which skills are surfaced — apply a profile, list, or disable a cluster without reinstall
- **[`gsd-update`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-update/SKILL.md)**: Update GSD to latest version with changelog display
- **[`gsd-help`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-help/SKILL.md)**: Show available GSD commands and usage guide
- **[`gsd-import`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-import/SKILL.md)**: Ingest external plans with conflict detection against project decisions before writing anything.
- **[`gsd-ns-workflow`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-ns-workflow/SKILL.md)**: workflow | discuss plan execute verify phase progress
- **[`gsd-ns-project`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-ns-project/SKILL.md)**: project lifecycle | milestones audits summary
- **[`gsd-ns-ideate`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-ns-ideate/SKILL.md)**: exploration capture | explore sketch spike spec capture
- **[`gsd-ns-review`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-ns-review/SKILL.md)**: quality gates | code review debug audit security eval ui
- **[`gsd-ns-manage`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-ns-manage/SKILL.md)**: config workspace | workstreams thread update ship inbox
- **[`gsd-ns-context`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-ns-context/SKILL.md)**: codebase intel | map graphify docs learnings mempalace

---

## Complete Global Paths Directory (All 72 Skills)

| Skill Name | Global Path |
| :--- | :--- |
| `gsd-add-tests` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-add-tests/SKILL.md` |
| `gsd-ai-integration-phase` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-ai-integration-phase/SKILL.md` |
| `gsd-audit-fix` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-audit-fix/SKILL.md` |
| `gsd-audit-milestone` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-audit-milestone/SKILL.md` |
| `gsd-audit-uat` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-audit-uat/SKILL.md` |
| `gsd-autonomous` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-autonomous/SKILL.md` |
| `gsd-capture` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-capture/SKILL.md` |
| `gsd-cleanup` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-cleanup/SKILL.md` |
| `gsd-code-review` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-code-review/SKILL.md` |
| `gsd-complete-milestone` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-complete-milestone/SKILL.md` |
| `gsd-config` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-config/SKILL.md` |
| `gsd-debug` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-debug/SKILL.md` |
| `gsd-discuss-phase` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-discuss-phase/SKILL.md` |
| `gsd-docs-update` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-docs-update/SKILL.md` |
| `gsd-eval-review` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-eval-review/SKILL.md` |
| `gsd-execute-phase` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-execute-phase/SKILL.md` |
| `gsd-explore` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-explore/SKILL.md` |
| `gsd-extract-learnings` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-extract-learnings/SKILL.md` |
| `gsd-fast` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-fast/SKILL.md` |
| `gsd-forensics` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-forensics/SKILL.md` |
| `gsd-graphify` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-graphify/SKILL.md` |
| `gsd-health` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-health/SKILL.md` |
| `gsd-help` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-help/SKILL.md` |
| `gsd-import` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-import/SKILL.md` |
| `gsd-inbox` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-inbox/SKILL.md` |
| `gsd-ingest-docs` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-ingest-docs/SKILL.md` |
| `gsd-manager` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-manager/SKILL.md` |
| `gsd-map-codebase` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-map-codebase/SKILL.md` |
| `gsd-mempalace-capture` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-mempalace-capture/SKILL.md` |
| `gsd-mempalace-recall` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-mempalace-recall/SKILL.md` |
| `gsd-milestone-summary` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-milestone-summary/SKILL.md` |
| `gsd-mvp-phase` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-mvp-phase/SKILL.md` |
| `gsd-new-milestone` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-new-milestone/SKILL.md` |
| `gsd-new-project` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-new-project/SKILL.md` |
| `gsd-next` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-next/SKILL.md` |
| `gsd-ns-context` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-ns-context/SKILL.md` |
| `gsd-ns-ideate` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-ns-ideate/SKILL.md` |
| `gsd-ns-manage` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-ns-manage/SKILL.md` |
| `gsd-ns-project` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-ns-project/SKILL.md` |
| `gsd-ns-review` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-ns-review/SKILL.md` |
| `gsd-ns-workflow` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-ns-workflow/SKILL.md` |
| `gsd-onboard` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-onboard/SKILL.md` |
| `gsd-pause-work` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-pause-work/SKILL.md` |
| `gsd-phase` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-phase/SKILL.md` |
| `gsd-plan-phase` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-plan-phase/SKILL.md` |
| `gsd-plan-review-convergence` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-plan-review-convergence/SKILL.md` |
| `gsd-pr-branch` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-pr-branch/SKILL.md` |
| `gsd-profile-user` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-profile-user/SKILL.md` |
| `gsd-progress` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-progress/SKILL.md` |
| `gsd-quick` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-quick/SKILL.md` |
| `gsd-quick-batch` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-quick-batch/SKILL.md` |
| `gsd-resume-work` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-resume-work/SKILL.md` |
| `gsd-review` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-review/SKILL.md` |
| `gsd-review-backlog` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-review-backlog/SKILL.md` |
| `gsd-secure-phase` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-secure-phase/SKILL.md` |
| `gsd-settings` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-settings/SKILL.md` |
| `gsd-ship` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-ship/SKILL.md` |
| `gsd-sketch` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-sketch/SKILL.md` |
| `gsd-spec-phase` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-spec-phase/SKILL.md` |
| `gsd-spike` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-spike/SKILL.md` |
| `gsd-stats` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-stats/SKILL.md` |
| `gsd-surface` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-surface/SKILL.md` |
| `gsd-thread` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-thread/SKILL.md` |
| `gsd-ui-phase` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-ui-phase/SKILL.md` |
| `gsd-ui-review` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-ui-review/SKILL.md` |
| `gsd-ultraplan-phase` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-ultraplan-phase/SKILL.md` |
| `gsd-undo` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-undo/SKILL.md` |
| `gsd-update` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-update/SKILL.md` |
| `gsd-validate-phase` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-validate-phase/SKILL.md` |
| `gsd-verify-work` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-verify-work/SKILL.md` |
| `gsd-workspace` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-workspace/SKILL.md` |
| `gsd-workstreams` | `/Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-workstreams/SKILL.md` |

---

## Standard GSD Phase Execution SOP

1. **Step 0 — Next Action Detection**: Read [`gsd-next`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-next/SKILL.md) or [`gsd-progress`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-progress/SKILL.md) to detect current milestone status.
2. **Step 1 — Scoping & Discussion**: Run [`gsd-discuss-phase`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-discuss-phase/SKILL.md) to resolve gray areas before planning.
3. **Step 2 — Planning**: Author `PLAN.md` with [`gsd-plan-phase`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-plan-phase/SKILL.md).
4. **Step 3 — Execution**: Execute tasks with [`gsd-execute-phase`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-execute-phase/SKILL.md) using atomic git commits.
5. **Step 4 — Verification**: Conduct conversational UAT using [`gsd-verify-work`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-verify-work/SKILL.md).
6. **Step 5 — Shipping**: Open a clean PR with [`gsd-ship`](file:///Users/vrajeshsulakhe/.gemini/config/plugins/gsd-core/skills/gsd-ship/SKILL.md).
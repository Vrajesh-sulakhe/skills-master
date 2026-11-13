---
name: writing-plans
description: Writes comprehensive, bite-sized implementation plans with test-driven steps before code is modified or created. Use when you have a spec, design document, or requirements for a multi-step task, feature, or refactoring.
---

# Writing Plans

## Overview

Write implementation plans for an engineer who has not seen this codebase or this spec. Assume they write idiomatic code in the project's language once they know the exact interface and the exact test, and that they will make a reasonable choice wherever the plan leaves one open.

What they cannot know is what you decided: which files, which names and signatures, which values from the spec, which tests prove each task. Document those. Give them the whole plan as bite-sized tasks. DRY. YAGNI. TDD. Frequent commits.

**Announce at start:** "I'm using the writing-plans skill to create the implementation plan."

**Context:** If working in an isolated worktree or branch, ensure it is set up before plan execution.

**Save plans to:** `docs/plans/YYYY-MM-DD-<feature-name>.md`
- *(User preferences for plan location override this default)*

---

## When to use this skill
- When you have completed a design doc or specification and need an actionable execution roadmap.
- Before starting non-trivial multi-step code implementations, feature additions, or architectural refactorings.
- When an implementer (human or agent) needs unambiguous, test-driven instructions for sequential execution.

---

## Workflow

### 1. Scope Check
If the spec covers multiple independent subsystems, suggest breaking this into separate plans — one per subsystem. Each plan must produce working, testable software on its own.

### 2. File Structure Mapping
Before defining tasks, map out which files will be created or modified and what each one is responsible for:
- Design units with clear boundaries and well-defined interfaces. Each file should have one clear responsibility.
- Prefer smaller, focused files over large ones that do too much.
- Files that change together should live together. Split by responsibility, not by technical layer.
- In existing codebases, follow established patterns.

### 3. Task Right-Sizing
A task is the smallest unit that carries its own test cycle and review gate:
- Fold setup, configuration, scaffolding, and documentation steps into the task whose deliverable needs them.
- Split only where a reviewer could meaningfully reject one task while approving its neighbor.
- Each task ends with an independently testable deliverable.

### 4. Step Granularity (Plan-Validate-Execute Pattern)
Each step within a task is one action with a checkable result:
- **Step 1:** Write the failing test.
- **Step 2:** Run test to verify it fails.
- **Step 3:** Implement minimal code to satisfy interface.
- **Step 4:** Run tests to verify they pass.
- **Step 5:** Commit changes.

---

## Plan Structure & Template

See 👉 **[`resources/plan-template.md`](resources/plan-template.md)** for the complete Markdown template to copy when drafting plans.

### Key Elements of Every Task
- **Files**: Exact paths to create, modify (with line ranges), or test.
- **Interfaces**:
  - `Consumes`: What this task uses from earlier tasks (exact signatures).
  - `Produces`: What later tasks rely on (exact names, parameter and return types).
- **Exact Code Snippets**: Full test definitions and minimal function signatures.

---

## Self-Review Checklist

After drafting the complete plan, execute this self-review checklist against the spec:

- [ ] **1. Spec coverage:** Every requirement in the spec maps to a specific task.
- [ ] **2. Step scan:** Every step lets the implementer write exactly one reasonable thing.
- [ ] **3. Type consistency:** Types, method signatures, and property names match across tasks.
- [ ] **4. Review Focus:** Key failure modes and boundary conditions have dedicated tests assigned to owning tasks.
- [ ] **5. Proportion:** The plan is focused and concise, providing signatures and assertions rather than writing entire program bodies in advance.

---

## Execution Handoff

After saving and self-reviewing the plan, link it for the user to review:

```markdown
Plan complete and saved to `docs/plans/<filename>.md`. Please review the plan. Which execution approach would you prefer?

1. **Subagent-driven** - A fresh subagent implements each task and checks it before moving to the next.
2. **Direct/Native** - I implement every task step-by-step in this session with tests.
```


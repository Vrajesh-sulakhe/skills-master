---
name: brainstorming
description: Facilitates structured exploratory dialogue to clarify intent, requirements, approaches, and design before building. Use before any creative work, creating features, building components, adding functionality, modifying behavior, or designing new systems.
---

# Brainstorming

## Overview

This skill is for finding out what the user actually wants, and why, before anything gets built. People often have not finished working out all nuances of what they want. Good questions help them think it through. Understanding the *why* allows you to make downstream decisions that align with their intent.

---

## When to use this skill
- Before any creative work: creating features, building components, adding functionality, or modifying behavior.
- When requirements are open-ended, ambiguous, or have multiple viable architectural paths.
- Before jumping into implementation or writing code on new initiatives.

---

## Workflow

### 1. Assess What Is Known
Before responding, ask yourself: what is known about what is wanted, and why?
- **Everything is fully specified:** If a task is trivial and unambiguous (e.g., "change icon color to blue"), execute it directly.
- **Non-trivial decisions remain:** Begin the brainstorming dialogue.

### 2. Recon Before Asking
Before asking questions, inspect existing code, documentation, and context:
- Read referenced files and connected modules.
- Understand how relevant components work today.
- Never ask questions that the codebase or existing context already answers.

### 3. Socratic Dialogue
- **Ask one question at a time.** Focus on the question that would change the architecture or deliverables the most.
- **Understand intent first:** Focus on *why* and *who it's for* before diving into implementation details.
- **Offer recommendations:** When presenting technical options, clearly articulate tradeoffs and state your recommended path.

### 4. Lay Out the Approaches
Once intent is clear, present alternative approaches in a dedicated message:
- Present 2–3 viable alternatives with pros and cons.
- Recommend one and explain why.
- Get the user's decision before drafting the design document.

### 5. Size the Work
- **Small change:** A concise summary of agreed decisions.
- **Full project:** Comprehensive written design specification saved to `docs/specs/YYYY-MM-DD-<topic>-design.md`.

### 6. Builder Check
For full projects, validate the design doc using a builder review check before presenting it as final:
- Reference: 👉 **[`resources/builder-check-prompt.md`](resources/builder-check-prompt.md)**
- Review the design from the perspective of an independent builder who must implement it without guessing.

---

## Hard Gate

> [!IMPORTANT]
> **Nothing gets built until the design doc is approved by the user.**
> Building includes writing code, scaffolding, installing dependencies, or generating implementation plans.
> Once approved, transition directly to the **[`writing-plans`](../writing-plans/SKILL.md)** skill.

---

## Visual Companion

When visual inspection is more effective than text descriptions (e.g., UI mockups, state flowcharts, page layouts):
- Guide: 👉 **[`resources/visual-companion.md`](resources/visual-companion.md)**
- Start the server:
  ```bash
  bash scripts/start-server.sh --project-dir . --open
  ```
- Stop the server:
  ```bash
  bash scripts/stop-server.sh
  ```

---

## Red Flags Checklist

- [ ] Avoid giving overwhelming menus of options before understanding user intent.
- [ ] Do not assume unstated preferences; state proposals and reasoning clearly.
- [ ] Do not skip laying out alternative approaches.
- [ ] Do not proceed to code or plans until the design document is explicitly approved.


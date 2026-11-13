# Curated GitHub Repositories for AI Agent Skills & Plugins

This document contains all the GitHub repositories collected and configured to build, power, and expand the global skills library in Antigravity IDE and Gemini CLI.

---

## 1. Core Frameworks & Meta-Orchestration

### [obra/superpowers](https://github.com/obra/superpowers)
* **Description:** An agentic framework providing foundational cognitive and process workflows for AI coding agents. Auto-triggered on every single user prompt to ensure disciplined, test-driven, verified execution.
* **Key Skills:** `using-superpowers`, `brainstorming`, `systematic-debugging`, `writing-plans`, `executing-plans`, `test-driven-development`, `subagent-driven-development`, `verification-before-completion`.
* **Installation:**
  ```bash
  agy plugin install obra/superpowers
  ```

### [open-gsd/gsd-core](https://github.com/open-gsd/gsd-core)
* **Description:** "Get Shit Done" (GSD) — A structured, spec-driven development (SDD) system that turns vague goals into production software via `.planning/` artifacts, phase-based planning, wave parallel execution, and conversational UAT.
* **Key Skills:** 72 specialized skills unified under the global master skill [`get-shit-done`](file:///Users/vrajeshsulakhe/.gemini/config/skills/get-shit-done/SKILL.md) (`gsd-next`, `gsd-plan-phase`, `gsd-execute-phase`, `gsd-verify-work`, `gsd-ship`, etc.).
* **Installation:**
  ```bash
  agy plugin install open-gsd/gsd-core
  ```

### [sickn33/agentic-awesome-skills](https://github.com/sickn33/agentic-awesome-skills)
* **Description:** Massive, battle-tested catalog containing over 2,700 agent skills covering full-stack development, cloud architecture, pentesting/security, database optimization, CI/CD, marketing, and business analytics.
* **Key Skills:** `app-builder`, `ui-ux-pro-max`, `backend-dev-guidelines`, `fastapi-router-py`, `ethical-hacking-methodology`, `burp-suite-testing`, `aws-security-audit`, `rag-engineer`, `docker-expert`.
* **Installation:**
  ```bash
  agy plugin install sickn33/agentic-awesome-skills
  ```

### [alirezarezvani/claude-skills](https://github.com/alirezarezvani/claude-skills)
* **Description:** Curated production engineering skills covering automated research, code refactoring, cloud security audits, architecture reviews, and team coordination.
* **Key Skills:** `ar-run`, `ar-loop`, `cpo-review`, `cto-review`, `slo-design`, `chaos-experiment`, `tech-debt`, `persona`, `pipeline`.
* **Installation:**
  ```bash
  agy plugin install alirezarezvani/claude-skills
  ```

### [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills)
* **Description:** Official engineering and architecture skills created by Addy Osmani for senior software developers, emphasizing incremental implementation, clean code, and robust debugging.
* **Key Skills:** `spec-driven-development`, `incremental-implementation`, `test-driven-development`, `debugging-and-error-recovery`, `code-review-and-quality`, `code-simplification`, `api-and-interface-design`, `frontend-ui-engineering`.
* **Installation:**
  ```bash
  agy plugin install addyosmani/agent-skills
  ```

---

## 2. Specialized Domain Skills & Design Systems

### [twbs/bootstrap](https://github.com/twbs/bootstrap)
* **Description:** The world's most popular frontend toolkit. Configured with a master unified skill `bootstrap-all-rounder` consolidating all 11 modular Bootstrap skills.
* **Key Skills:** `bootstrap-all-rounder`, `bootstrap-v6-install`, `bootstrap-v5-v6-migration`, `bootstrap-v4-v6-migration`, `bootstrap-component`, `bootstrap-component-js`, `bootstrap-color-system`, `bootstrap-utility-api`, `bootstrap-npm`, `bootstrap-vite`, `bootstrap-webpack`, `bootstrap-parcel`.
* **Installation:**
  ```bash
  npx skills add twbs/bootstrap
  ```

### [superdesigndev/superdesign-skill](https://github.com/superdesigndev/superdesign-skill)
* **Description:** Direct integration with the SuperDesign canvas CLI for high-fidelity UI design, visual prototyping, component rendering, and live web extraction.
* **Key Skills:** `superdesign`.
* **Installation:**
  ```bash
  agy plugin install superdesigndev/superdesign-skill
  ```

### [oil-oil/oil-ui](https://github.com/oil-oil/oil-ui)
* **Description:** Industrial, high-contrast, tactical UI design system and component specifications.
* **Key Skills:** `oil-ui`.
* **Installation:**
  ```bash
  agy plugin install oil-oil/oil-ui
  ```

### [AllThingsSmitty/css-protips](https://github.com/AllThingsSmitty/css-protips)
* **Description:** A curated collection of modern CSS best practices, layout optimizations, and responsive styling techniques.
* **Key Skills:** `css-protips`.
* **Installation:**
  ```bash
  agy plugin install AllThingsSmitty/css-protips
  ```

### [zarazhangrui/frontend-slides](https://github.com/zarazhangrui/frontend-slides)
* **Description:** Generate and edit stunning HTML/CSS presentation slide decks directly from markdown and source content.
* **Key Skills:** `frontend-slides`.
* **Installation:**
  ```bash
  agy plugin install zarazhangrui/frontend-slides
  ```

---

## 3. Autonomous Execution & Agent Harnesses

### [paperclipai/paperclip](https://github.com/paperclipai/paperclip)
* **Description:** Open-source agent control plane and test harness for managing long-running agent evaluations, workspace isolation, and automated validation runs.
* **Key Skills:** `paperclip`, `prepare-paperclip-pr`, `verify-paperclip`, `paperclip-dev-workspace-run-verify-fix`.
* **Installation:**
  ```bash
  agy plugin install paperclipai/paperclip
  ```

### [addxai/enterprise-harness-engineering](https://github.com/addxai/enterprise-harness-engineering)
* **Description:** Enterprise harness patterns, fault-injection testing, and agent reliability engineering.
* **Key Skills:** `enterprise-harness-engineering`.
* **Installation:**
  ```bash
  agy plugin install addxai/enterprise-harness-engineering
  ```

### [abhishekbhakat/ralph-loop-for-antigravity](https://github.com/abhishekbhakat/ralph-loop-for-antigravity)
* **Description:** Autonomous iteration engine for Antigravity IDE. Continuously iterates on tasks defined in `PRD.md`, logs progress to `progress.txt`, and uses `prompt.md` to guide agent actions until all criteria are satisfied.
* **Setup:** Managed via the Ralph Loop sidebar extension and workspace configuration files (`.vscode/settings.json`, `PRD.md`, `progress.txt`, `prompt.md`).

### [Zoo-Code-Org/Zoo-Code](https://github.com/Zoo-Code-Org/Zoo-Code)
* **Description:** Open-source AI code intelligence and agent platform repositories.
* **Installation:**
  ```bash
  agy plugin install Zoo-Code-Org/Zoo-Code
  ```

---

## 4. Reverse Engineering & Advanced Research

### [Vrajesh-sulakhe/rea](https://github.com/Vrajesh-sulakhe/rea) (forked from `morluto/rea`)
* **Description:** "Reverse Engineer Anything" (REA) — A local-first reverse engineering suite connecting Ghidra, Hopper, and IDA Pro to coding agents for binary analysis, decompilation, and vulnerability research.
* **Key Skills:** `reverse-engineer-anything`, `rea-tool-design`, `rea-analysis-optimization`.
* **Installation:**
  ```bash
  agy plugin install Vrajesh-sulakhe/rea
  ```

### [karpathy/autoresearch](https://github.com/karpathy/autoresearch)
* **Description:** Andrej Karpathy's autonomous research iteration loop for AI agents. Formulates hypotheses, executes experiments, measures outcomes, and retains or discards modifications.
* **Key Skills:** `autoresearch`.
* **Installation:**
  ```bash
  agy plugin install karpathy/autoresearch
  ```

### [google-antigravity/antigravity-sdk-python](https://github.com/google-antigravity/antigravity-sdk-python)
* **Description:** Official Python SDK for developing agents, tools, workflows, and integrations on the Google Antigravity platform.
* **Key Skills:** `google-antigravity-sdk`.
* **Installation:**
  ```bash
  agy plugin install google-antigravity/antigravity-sdk-python
  ```

### [ComposioHQ/awesome-claude-skills](https://github.com/ComposioHQ/awesome-claude-skills)
* **Description:** Composio's directory of specialized tools and actions for LLMs and AI coding assistants.
* **Key Skills:** `template-skill` and integration helpers.
* **Installation:**
  ```bash
  agy plugin install ComposioHQ/awesome-claude-skills
  ```

---

## Summary Table

| Category | Repository | Primary Capability |
| :--- | :--- | :--- |
| **Meta-Workflow** | [`obra/superpowers`](https://github.com/obra/superpowers) | Mandatory cognitive & quality workflows |
| **Lifecycle & SDD** | [`open-gsd/gsd-core`](https://github.com/open-gsd/gsd-core) | Spec-driven development (`get-shit-done`) |
| **Global Skills** | [`sickn33/agentic-awesome-skills`](https://github.com/sickn33/agentic-awesome-skills) | 2,700+ full-stack, security & AI skills |
| **Engineering Ops** | [`alirezarezvani/claude-skills`](https://github.com/alirezarezvani/claude-skills) | Architecture, C-suite reviews & DevOps |
| **Senior Dev** | [`addyosmani/agent-skills`](https://github.com/addyosmani/agent-skills) | TDD, specs, code quality & simplification |
| **Frontend Toolkit**| [`twbs/bootstrap`](https://github.com/twbs/bootstrap) | Bootstrap 5/6 components & migrations |
| **UI Canvas** | [`superdesigndev/superdesign-skill`](https://github.com/superdesigndev/superdesign-skill) | Visual UI generation & canvas editing |
| **Design System** | [`oil-oil/oil-ui`](https://github.com/oil-oil/oil-ui) | Industrial tactical design tokens |
| **CSS Mastery** | [`AllThingsSmitty/css-protips`](https://github.com/AllThingsSmitty/css-protips) | Modern CSS tips & layout patterns |
| **Presentations** | [`zarazhangrui/frontend-slides`](https://github.com/zarazhangrui/frontend-slides) | HTML slide deck generator |
| **Agent Platform** | [`paperclipai/paperclip`](https://github.com/paperclipai/paperclip) | Control plane & eval harness |
| **Reliability** | [`addxai/enterprise-harness-engineering`](https://github.com/addxai/enterprise-harness-engineering) | Fault injection & harness design |
| **Autonomous Loop**| [`abhishekbhakat/ralph-loop-for-antigravity`](https://github.com/abhishekbhakat/ralph-loop-for-antigravity) | Antigravity PRD autonomous iteration loop |
| **Code Platform** | [`Zoo-Code-Org/Zoo-Code`](https://github.com/Zoo-Code-Org/Zoo-Code) | AI code intelligence platform |
| **Binary Analysis**| [`Vrajesh-sulakhe/rea`](https://github.com/Vrajesh-sulakhe/rea) | Reverse engineering with Ghidra & IDA |
| **AI Research** | [`karpathy/autoresearch`](https://github.com/karpathy/autoresearch) | Autonomous scientific & code experiments |
| **Platform SDK** | [`google-antigravity/antigravity-sdk-python`](https://github.com/google-antigravity/antigravity-sdk-python) | Python SDK for Antigravity agents |
| **Integrations** | [`ComposioHQ/awesome-claude-skills`](https://github.com/ComposioHQ/awesome-claude-skills) | Tooling & action integrations |

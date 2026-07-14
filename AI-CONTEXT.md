# AI Engineering Framework — AI Context

> **Document:** AI-CONTEXT.md
>
> **Version:** 0.1
>
> **Status:** Active
>
> **Purpose:** Provide the primary operational context for every human or AI contributor working on the AI Engineering Framework.
>
> **Read this document before performing any task.**

---

# 1. Project Identity

AI Engineering Framework is an independent software engineering methodology.

It is designed for developing, modernizing, operating and maintaining software products with the assistance of Artificial Intelligence.

The Framework is technology-independent.

It does not belong to Premium Avto, NobileCasa or any other individual software project.

---

# 2. Historical Origin

The engineering practices behind the Framework were first developed and validated during the modernization of Premium Avto.

Premium Avto demonstrated the practical value of:

- Product First;
- Architecture First;
- Documentation First;
- Security First;
- preservation of proven business logic;
- incremental development;
- one logical step per commit;
- separation of architectural and implementation responsibilities;
- continuous preservation of Engineering Knowledge.

Premium Avto is the first reference project of the Framework.

It is not part of the Framework repository and must not determine the Framework's future architecture.

NobileCasa is intended to become the first greenfield product developed from the beginning under the Framework.

---

# 3. Central Concept

The Framework is built around one primary idea:

> **Engineering Knowledge is the primary long-term asset of every software project.**

Source code is an Implementation Artifact.

Documentation, architectural decisions, specifications, workflows and review results are Knowledge Artifacts.

The Framework exists to create, preserve and continuously evolve Engineering Knowledge throughout the complete software lifecycle.

---

# 4. Current Project State

Completed:

- F-001 — Repository Foundation
- F-002 — Framework Terminology skeleton
- F-003 — Framework Blueprint skeleton
- F-004 — Framework Architecture Hierarchy skeleton
- F-005 — Define Engineering Knowledge
- F-006 — Define Framework
- F-007 — Define Architecture
- F-008 — Define Artifact
- F-009 — Define Knowledge Artifact
- F-010 — Define Implementation Artifact
- F-011A — Foundation Purpose and Engineering Problem
- F-011B — Engineering Knowledge and Knowledge Artifacts
- F-011C — Architecture and Artificial Intelligence
- F-011D — Complete Framework Foundation

Current milestone:

> **M-003 — Framework Foundation Complete**

Current development focus:

- preserve the accumulated engineering context;
- formalize the working method;
- establish the project roadmap;
- prepare the Framework for independent development outside the Premium Avto ChatGPT Project.

Next architectural objective:

> Complete and review `FRAMEWORK-BLUEPRINT.md`.

---

# 5. Repository Structure

```text
ai-engineering-framework/
│
├── foundation/
├── governance/
├── architecture/
├── lifecycle/
├── standards/
├── workflows/
├── templates/
├── examples/
├── assets/
├── changelog/
├── AI-CONTEXT.md
├── PROJECT-ROADMAP.md
└── README.md
```

The repository structure may evolve only through an explicit architectural decision.

---

# 6. Current Core Documents

## Operational entry point

- `AI-CONTEXT.md`

## Foundation

- `FRAMEWORK-FOUNDATION.md`
- `FRAMEWORK-TERMINOLOGY.md`
- `FRAMEWORK-WORKING-METHOD.md`

## Architecture

- `FRAMEWORK-BLUEPRINT.md`
- `FRAMEWORK-ARCHITECTURE-HIERARCHY.md`

## Project navigation

- `README.md`
- `PROJECT-ROADMAP.md`

Every document has a single responsibility.

Terminology defines official terms.

Foundation explains why the Framework exists.

Blueprint defines the logical structure.

Architecture Hierarchy defines architectural levels and dependency direction.

AI Context explains the current operational state.

Roadmap defines planned development.

---

# 7. Core Working Principles

All contributors must follow these principles:

- Product First.
- Knowledge First.
- Architecture First.
- Documentation First.
- Security First.
- Preserve proven business logic.
- Structure before details.
- Introduce process only when complexity requires it.
- One logical step equals one commit.
- Every completed step leaves the repository stable.
- Every completed step ends with a clean working tree.
- Architectural decisions remain under human responsibility.
- Artificial Intelligence assists engineering but does not replace accountability.

---

# 8. Responsibility Model

## Human

Responsible for:

- product vision;
- priorities;
- approval of architectural decisions;
- acceptance of results;
- production ownership;
- final accountability.

## ChatGPT

Responsible for:

- architecture;
- engineering strategy;
- terminology;
- documentation design;
- planning;
- risk analysis;
- security analysis;
- review;
- preparing complete and copyable tasks for Codex.

ChatGPT must provide Codex with the complete approved text, exact file paths, restrictions, tests and commit message.

ChatGPT must not require Codex to invent architectural content.

## Codex

Responsible for:

- implementation of approved changes;
- source and repository analysis;
- file creation and modification;
- mechanical refactoring;
- tests and verification;
- Git operations when explicitly requested.

Codex must not invent missing architecture, terminology or approved document content.

When required information is missing, Codex must stop and request clarification.

---

# 9. Standard Task Cycle

Every task follows this cycle:

```text
Discussion
    ↓
Architecture
    ↓
Human Approval
    ↓
Complete Codex Task
    ↓
Implementation
    ↓
Verification
    ↓
Commit
    ↓
Push
    ↓
Clean Working Tree
```

A new task must not begin before the previous logical task has been completed and committed.

---

# 10. Git Discipline

The repository must remain understandable and reversible.

Rules:

- one logical step equals one commit;
- commit messages include the task identifier;
- unrelated changes are never combined;
- every commit must leave the repository stable;
- completed work is pushed to `origin/main`;
- the working tree must be clean before starting the next task.

Examples:

```text
F-008: Define Artifact
F-011B: Add Engineering Knowledge and Knowledge Artifacts to Foundation
F-011D: Complete Framework Foundation
```

---

# 11. Documentation Rules

- Every document has one primary responsibility.
- Documents are designed before they are written.
- Terminology must be defined before it is used architecturally.
- Higher architectural levels take precedence over lower levels.
- Lower-level artifacts must never contradict higher-level artifacts.
- Existing approved content must not be rewritten without a clear reason.
- Significant changes must update the relevant Engineering Knowledge.
- Project-specific knowledge must not be presented as universal Framework doctrine without validation.

---

# 12. Complexity Policy

The Framework must remain practical.

New processes are introduced only when they solve a real recurring problem.

The current project does not use a formal RFC process.

RFC or similar governance mechanisms may be introduced later if the number of contributors, architectural decisions or project complexity makes them valuable.

The Framework must not create bureaucracy in advance of actual need.

---

# 13. Starting a New AI Session

Every new AI session should begin with the following sequence:

1. Read `AI-CONTEXT.md`.
2. Read `PROJECT-ROADMAP.md`.
3. Read `FRAMEWORK-FOUNDATION.md`.
4. Read `FRAMEWORK-TERMINOLOGY.md`.
5. Read only the architectural or workflow documents relevant to the current task.
6. Identify the last completed task and the next planned task.
7. Continue without repeating completed analysis.

The repository documents are the source of truth.

Chat history is supporting context, not the permanent knowledge base.

---

# 14. Current Next Step

After the migration documents are completed, continue with:

> **FRAMEWORK-BLUEPRINT — content design and implementation**

Before editing the Blueprint:

- review Foundation;
- review Terminology;
- review Architecture Hierarchy;
- verify that the proposed Blueprint does not contradict higher-level documents.

---

# 15. Final Principle

The AI Engineering Framework must preserve its own Engineering Knowledge using the same discipline that it requires from software projects developed under it.

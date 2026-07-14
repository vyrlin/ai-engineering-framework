# AI Engineering Framework

# FRAMEWORK-WORKING-METHOD

> **Document:** FRAMEWORK-WORKING-METHOD.md
>
> **Version:** 0.1
>
> **Status:** Active
>
> **Purpose:** Define the practical working method used to develop the Framework and software projects governed by it.

---

# 1. Purpose

This document defines the default collaboration method between humans and Artificial Intelligence within the AI Engineering Framework.

It converts the Framework's foundational principles into a practical and repeatable way of working.

The method should remain lightweight and should introduce additional process only when project complexity requires it.

---

# 2. Responsibility Separation

The working method separates product ownership, architecture and implementation responsibilities.

## Human Responsibility

Humans define product objectives, establish priorities, approve architectural decisions and accept the final result.

Humans remain accountable for the product and its production operation.

## ChatGPT Responsibility

ChatGPT is responsible for architecture, engineering strategy, documentation, planning, review, risk analysis and preparation of implementation tasks.

ChatGPT must provide complete, copyable instructions to Codex.

A Codex task must contain:

- task identifier;
- goal;
- exact file paths;
- complete approved content or exact change instructions;
- restrictions;
- verification requirements;
- exact commit message;
- Git operations when required.

## Codex Responsibility

Codex implements approved tasks.

Codex may analyze the repository and report technical findings.

Codex must not invent missing architectural decisions, approved terminology or document content.

If essential information is missing, Codex must stop and request clarification.

---

# 3. Standard Work Cycle

Every logical task follows this sequence:

```text
Problem or Objective
        ↓
Discussion
        ↓
Architecture or Content Design
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

Stages may be simplified for very small low-risk tasks, but approval, implementation and verification must remain distinct responsibilities.

---

# 4. One Logical Step Equals One Commit

A commit must represent one complete and understandable engineering change.

A logical step may be:

- one terminology definition;
- one document section;
- one complete document;
- one architectural decision;
- one source-code correction;
- one security improvement;
- one independently testable feature.

Unrelated changes must not be combined.

A new logical task starts only after the previous task is committed and the working tree is clean.

---

# 5. Complete Codex Task Rule

ChatGPT must provide implementation tasks that can be executed without architectural guessing.

A complete task specifies:

```text
Task ID

Goal

Current State

Files

Approved Content or Exact Changes

Restrictions

Verification

Commit Message

Push Requirement
```

The user should be able to copy the complete task directly into Codex.

When the task requires creating a file, its exact path and full approved content must be provided.

When the task requires modifying a file, the exact section and complete replacement or insertion text must be provided.

---

# 6. Documentation and Knowledge

Engineering Knowledge must be preserved continuously.

Documentation is updated when:

- architecture changes;
- terminology changes;
- workflows change;
- security decisions change;
- significant milestones are completed;
- project state changes in a way that future contributors need to understand.

Documentation should not be expanded merely to create the appearance of process.

Every document must have one primary responsibility.

---

# 7. Architecture Before Implementation

Significant implementation begins only after the problem and intended architecture are understood.

Architecture does not require excessive documentation for every small task.

The amount of architectural work should correspond to the risk and complexity of the change.

Working and proven business logic must not be rewritten without clear justification.

---

# 8. Verification

Every task includes verification appropriate to its risk.

Verification may include:

- document structure review;
- terminology consistency review;
- syntax checks;
- automated tests;
- manual tests;
- security review;
- responsive interface testing;
- Git diff inspection;
- confirmation of a clean working tree.

High-risk tasks require stronger verification than low-risk tasks.

---

# 9. Simplicity and Process Growth

The Framework does not introduce formal processes before they provide practical value.

Processes such as formal RFC review, multi-stage approval boards or complex branching strategies are optional maturity mechanisms.

They may be introduced when:

- multiple independent contributors participate;
- decisions affect many projects;
- architectural conflicts become frequent;
- regulatory or organizational requirements demand them.

Until then, direct discussion, human approval, one logical commit and preserved Engineering Knowledge are sufficient.

---

# 10. Continuous Improvement

The working method evolves through real project experience.

A practice should be considered for inclusion in the Framework when it:

- solves a recurring problem;
- reduces engineering risk;
- improves predictability;
- preserves knowledge;
- improves product quality;
- remains simple enough to apply consistently.

Project experience becomes Framework knowledge only after it is generalized beyond the original project.

---

# 11. Final Principle

The working method exists to improve engineering outcomes.

Process serves the product.

Architecture serves long-term consistency.

Artifacts preserve knowledge.

Artificial Intelligence accelerates execution.

Humans remain accountable.

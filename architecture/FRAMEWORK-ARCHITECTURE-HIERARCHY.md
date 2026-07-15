# AI Engineering Framework

# FRAMEWORK-ARCHITECTURE-HIERARCHY

> Document: FRAMEWORK-ARCHITECTURE-HIERARCHY.md
> Version: 1.0
> Status: Active
> Purpose: Define the architectural levels of the AI Engineering Framework and the permitted direction of dependencies between them.

---

# 1. Purpose

This document defines the normative architectural hierarchy of the AI Engineering Framework.

It establishes the levels through which foundational intent is translated into project application, the authority assigned to each level and the dependency rules that preserve consistency across the Framework.

`FRAMEWORK-BLUEPRINT.md` defines the Framework's components and system architecture. This document does not repeat that system map. It governs how architectural authority flows between levels and which dependencies are permitted or prohibited.

The hierarchy applies both to the evolution of the Framework and to projects that adopt it.

---

# 2. Architectural Levels

The hierarchy is ordered from the most stable and general authority to the most contextual application. A lower level may add detail within its responsibility, but it must remain consistent with every applicable higher level.

The levels represent architectural authority, not repository folders or a mandatory document count.

## Level 1 — Foundation

**Purpose:** Establish the enduring engineering purpose and foundational principles of the Framework.

**May contain:** the engineering problem, stable beliefs, long-term intent and fundamental boundaries that govern the Framework.

**Must not contain:** detailed terminology, component maps, dependency mechanics, operational procedures, technology choices or project-specific rules.

## Level 2 — Terminology

**Purpose:** Provide the normative language used to express Framework knowledge consistently.

**May contain:** official terms, definitions, distinctions and terminology usage rules.

**Must not contain:** competing engineering principles, system architecture, process instructions or project-specific vocabulary presented as universal Framework language.

## Level 3 — Blueprint

**Purpose:** Define the Framework as a coherent engineering system.

**May contain:** the system architecture, component boundaries, conceptual layers, knowledge flow, collaboration boundaries and the document map.

**Must not contain:** detailed dependency rules, complete standards, operational workflows, template content or project implementation decisions.

## Level 4 — Architecture Hierarchy

**Purpose:** Define architectural ordering, authority and permitted dependency direction.

**May contain:** architectural levels, dependency rules, authority rules, evolution rules, adoption boundaries and hierarchy verification criteria.

**Must not contain:** a competing system map, detailed engineering standards, executable processes, templates or product-specific architecture.

## Level 5 — Governance

**Purpose:** Establish decision ownership, approval authority, accountability and control boundaries.

**May contain:** roles, decision rights, approval responsibilities, review authority, escalation boundaries and governance appropriate to demonstrated complexity.

**Must not contain:** foundational principles, redefinitions of terminology, competing system architecture, detailed lifecycle sequences or technical implementation requirements.

## Level 6 — Lifecycle

**Purpose:** Define the major states and transitions through which products and engineering initiatives evolve.

**May contain:** lifecycle models, phases, transition conditions, lifecycle responsibilities and distinctions between greenfield development, modernization, maintenance, security improvement and production operation.

**Must not contain:** competing governance authority, detailed quality standards, step-by-step workflows, template content or product-specific delivery plans.

## Level 7 — Standards

**Purpose:** Define mandatory or recommended engineering requirements within a declared scope.

**May contain:** architecture, documentation, security, quality, testing, review, naming, artifact-management and production-readiness requirements.

**Must not contain:** new foundational principles, redefined terminology, changes to system architecture, workflow-specific execution sequences or project-specific exceptions presented as universal rules.

## Level 8 — Workflows

**Purpose:** Define repeatable operating methods for applying higher-level knowledge to engineering activities.

**May contain:** ordered activities, inputs, outputs, responsibilities, verification steps and operational working methods such as the Human–AI collaboration method.

**Must not contain:** competing governance authority, new standards hidden as process steps, redefinitions of higher-level concepts or assumptions tied to one project unless the workflow is explicitly project-local.

## Level 9 — Templates

**Purpose:** Provide reusable structures for producing consistent artifacts.

**May contain:** document structures, required fields, placeholders, prompts and reusable artifact scaffolding governed by an applicable standard or workflow.

**Must not contain:** independent architectural decisions, undeclared mandatory rules, redefined terminology or workflow logic that exists only inside the template.

## Level 10 — Examples

**Purpose:** Demonstrate valid application of Framework knowledge without creating new authority.

**May contain:** reference applications, filled templates, sample artifacts and generalized lessons from validated project experience.

**Must not contain:** normative requirements, universal claims based on one project, project-sensitive information or implicit overrides of the artifacts being demonstrated.

## Level 11 — Projects

**Purpose:** Apply the Framework to a specific product, system or engineering initiative.

**May contain:** product goals, project architecture, local decisions, implementation artifacts, project knowledge, selected Framework practices and justified project-specific constraints.

**Must not contain:** modifications to Framework authority, redefinitions of Framework terminology or local practices presented as universal Framework rules.

---

# 3. Dependency Rules

The normative direction of architectural influence is downward:

```text
Level 1   Foundation
              ↓
Level 2   Terminology
              ↓
Level 3   Blueprint
              ↓
Level 4   Architecture Hierarchy
              ↓
Level 5   Governance
              ↓
Level 6   Lifecycle
              ↓
Level 7   Standards
              ↓
Level 8   Workflows
              ↓
Level 9   Templates
              ↓
Level 10  Examples
              ↓
Level 11  Projects
```

This sequence defines authority order. It does not require every artifact to depend directly on every preceding level. Each artifact must depend on and conform to all higher-level sources applicable to its scope.

## Permitted Dependencies

- A lower level may depend on one or more higher levels.
- A lower level may reference higher-level authority instead of repeating it.
- An artifact may depend on another artifact at the same level when responsibilities do not overlap and the dependency graph remains acyclic.
- A lower level may specialize a higher-level rule within the boundaries explicitly allowed by that rule.
- A project may select applicable standards, workflows and templates when the Framework allows contextual adoption.
- Evidence from lower levels may inform a proposed change to a higher level through an explicit review and approval step.

## Prohibited Dependencies

- A higher level must not require a lower level in order to define its own meaning or authority.
- A lower level must not override, weaken or redefine an applicable higher-level rule.
- Circular dependencies between artifacts or levels are prohibited.
- Two artifacts must not claim authority over the same concern within the same scope.
- A standard must not redefine Foundation, Terminology, Blueprint or Hierarchy content.
- A workflow must not create undeclared standards or governance authority.
- A template or example must not become the only location of a mandatory rule.
- A project-specific artifact must not modify Framework architecture or present local decisions as Framework doctrine.

## Direction of Influence and Feedback

Architectural authority flows from higher levels to lower levels.

Verification results, operational experience and project evidence may flow upward as feedback. Feedback is evidence, not authority: it does not change a higher level until the responsible authoritative source is deliberately reviewed, approved and updated.

---

# 4. Authority Rules

Each concern must have one authoritative source within its declared scope.

| Level | Authoritative source | Authority |
| --- | --- | --- |
| Foundation | `FRAMEWORK-FOUNDATION.md` | Engineering purpose, philosophy and foundational principles |
| Terminology | `FRAMEWORK-TERMINOLOGY.md` | Normative definitions and terminology rules |
| Blueprint | `FRAMEWORK-BLUEPRINT.md` | Framework system architecture and component relationships |
| Architecture Hierarchy | `FRAMEWORK-ARCHITECTURE-HIERARCHY.md` | Architectural levels, authority order and dependency rules |
| Governance | Approved governance artifacts | Decision ownership, approval responsibility and accountability within their declared scope |
| Lifecycle | Approved lifecycle artifacts | Lifecycle states, transitions and lifecycle-specific responsibilities |
| Standards | The applicable approved standard | Engineering requirements within the standard's declared scope |
| Workflows | The applicable approved workflow or working-method document | Repeatable execution model for the declared activity |
| Templates | The applicable approved template | Reusable artifact structure, but not independent architectural authority |
| Examples | The higher-level artifacts being demonstrated | Examples have no independent normative authority |
| Projects | Approved project Knowledge Artifacts | Project-specific decisions and constraints within Framework boundaries |

An artifact is authoritative only for the responsibility explicitly assigned to it. Authority does not transfer through quotation, duplication or convenience.

`AI-CONTEXT.md`, `PROJECT-ROADMAP.md` and `README.md` are supporting navigation and state documents outside the normative architectural chain. They may reference every level but must not redefine the authority of any level.

---

# 5. Evolution Rules

Framework evolution must preserve the direction of architectural authority.

- A proposed change must identify the highest affected level before implementation begins.
- A change to a higher level requires impact analysis across all affected lower levels.
- Affected lower-level artifacts must be reviewed and updated or explicitly confirmed as compatible.
- A change to a lower level may add detail or improve application but must not alter the meaning of a higher level.
- Lower-level evidence may justify proposing a higher-level change, but the higher-level authoritative source must be changed directly through its own approval process.
- Moving responsibility between levels requires an explicit architectural decision and removal of the former competing authority.
- Deprecated rules must identify their replacement or state that no replacement exists.
- Existing projects are not silently made compliant with a changed Framework; adoption impact must be evaluated explicitly.
- Framework evolution must remain incremental, traceable and proportionate to demonstrated need.

When a higher-level source changes, consistency is restored from the changed level downward. A lower-level artifact is not considered authoritative evidence that the higher level has changed.

---

# 6. Project Adoption

The Framework and an adopting project have separate scopes of authority.

The Framework defines reusable engineering knowledge, architectural boundaries and applicable rules. A project selects and applies those rules to its own product context.

A project may:

- create project-specific architecture, decisions, standards, workflows and templates where the Framework permits specialization;
- choose among optional Framework mechanisms according to product risk and project complexity;
- record justified local constraints and deviations without presenting them as Framework rules;
- contribute evidence and generalized improvement proposals back to the Framework.

A project must not:

- edit or reinterpret Framework authority through project-local artifacts;
- redefine official Framework terminology;
- weaken mandatory Framework constraints without an explicitly permitted deviation mechanism;
- treat project experience as universal doctrine without review and generalization.

Project feedback can initiate Framework evolution, but only an approved change to the appropriate Framework authoritative source changes the Framework itself.

---

# 7. Verification Rules

An architectural consistency review must verify that:

- every artifact has a declared primary responsibility and architectural level;
- every normative concern has one authoritative source within its scope;
- dependencies point to the same level or upward in the authority hierarchy;
- same-level dependencies are explicit, non-overlapping and acyclic;
- no circular dependency exists between levels or artifacts;
- no lower-level artifact overrides or redefines higher-level knowledge;
- no mandatory rule exists only in a workflow, template, example or project artifact;
- summaries and references do not create competing authority;
- Foundation, Terminology, Blueprint and Architecture Hierarchy remain mutually consistent within their distinct responsibilities;
- changes to higher levels include review of affected lower levels;
- project-specific knowledge remains separated from Framework doctrine;
- security constraints are preserved across every affected level;
- deprecated or replaced authority does not remain active in multiple locations.

Verification should examine both explicit references and implicit dependencies created by duplicated definitions, hidden rules or assumed project context.

The hierarchy is consistent only when every lower-level artifact can be traced to applicable higher-level authority without cycles, contradictions or competing sources of truth.

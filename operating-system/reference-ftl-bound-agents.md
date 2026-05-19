---
description: Mapping Context Boundaries and Safe-Disengagement Rules for AI Agents
---

# \[reference] FTL-Bound Agents



> Survival Log from the Drift

### Current Coordinates

* Agent instruction files are prompts in a technical sense, but they should not be treated as disposable requests.
* A good AGENTS.md or CLAUDE.md does not merely tell an AI agent what to do. It defines the world in which the agent is allowed to act.
* The purpose of an agent instruction file is to reduce dangerous interpretation space, not to contain every project detail.

### A Prompt, but Not Merely a Prompt

Technically, AGENTS.md, CLAUDE.md, and similar files are prompts.

They are instructions placed in front of an AI system, influencing how the agent reads the project, chooses actions, edits files, runs commands, and reports results.

But inside Cosmic Horizon, they are not treated as ordinary prompts.

An ordinary prompt asks for output.

An agent instruction file defines the operating boundary around output.

It tells the agent where to look, when to act, when to stop, what must not be inferred, and what must be reported before the work can be trusted.

This distinction matters because AI agents do not merely execute instructions.

They interpret them.

When the boundary is vague, the agent widens the task through interpretation.

When the boundary is clear, the agent works inside a declared world—moving within bounded orbits where assumptions are verified, not guessed.

### Reduce the Mass

Agent instruction files should not become full project manuals.

If they try to contain every project rule, every architectural decision, every testing detail, and every warning, they become heavy, stale, and expensive to load into every task.

Their better role is not to contain the whole map.

They open controlled wormholes into project-specific space.

Through them, different AI agents can enter the right context, load the right boundary documents, and avoid drifting beyond the intended orbit.

**Agent instruction files define the route.**

They should define:

* when an agent may use a fast path
* when an agent must use a default path
* when an agent must stop
* when an agent must declare before execution
* when project-specific documents must be loaded
* when verification status must be reported

**Project-specific boundary documents define the map.**

They record:

* constraints
* invariants
* danger zones
* approval gates
* verification rules

Inside Cosmic Horizon, those documents form the observatory layer.

> Excessive mass collapses the orbit.
>
> — Cosmic Horizon

### Decouple the Wormhole

A reusable agent instruction system must separate common execution rules from project-specific boundaries.

Agent instruction files are not the project map.

They are controlled wormholes into project-specific space.

Depending on the environment, this wormhole may manifest as `AGENTS.md`, `CLAUDE.md`, `GEMINI.md`, `.cursorrules`, Roo Code rules, Cline instructions, or any other tool-specific entry point.

The project map should live elsewhere.

It belongs to the Observatory Layer, defined by stable boundary documents such as:

* `system_gravity.md`
* `invariants.md`
* `no_crossing_zones.md`
* `event_horizon.md`
* `approval_gate.md`
* `test_matrix.md`

These files do not need to exist in every project.

They are deployed only when the project scale, company governance, team conventions, or task domain requires them.

The critical insight is not about enforcing a universal filename, rigid directory structure, or identical instruction format across different tools.

The critical insight is that every AI agent must know how to locate project-specific boundaries, and missing boundaries must remain explicit instead of being invented.

The wormhole may change by tool.

The map must remain observable.

Entry points are ephemeral; boundaries are invariant.

— Cosmic Horizon

### Chart Routes, Not Advice

Weak instruction files often sound reasonable on the surface.

They offer passive advice:

* be careful
* keep it simple
* make minimal changes
* use relevant files
* preserve the existing flow when possible

These sentences are not useless, but they leave too much interpretation space.

What counts as simple?

What is relevant?

When is preservation “possible”?

What looks minimal to the model may still be destructive to the project.

Stronger instruction files do not advise.

They chart explicit routes.

* **If** the task only changes wording or formatting → **use the fast path.**
* **If** the task changes source behavior → **use the default path.**
* **If** the task conflicts with an approval rule → **stop before execution.**
* **If** verification cannot be performed → **report the status instead of pretending.**
* **If** the scope is unclear → **do not widen it by interpretation.**

A route is stronger than advice.

Advice asks the model to behave well.

A route tells the model what to do when a condition appears.

#### Control the Interpretation Space

Plain instructions do not remove interpretation.

They reduce dangerous interpretation space.

No agent instruction file can eliminate every act of abstraction, inference, or judgment.

AI agents still need to read context, compare patterns, choose tools, and decide how to apply a rule to the current task.

The goal is not to make interpretation disappear.

The goal is to prevent interpretation from becoming unauthorized execution.

A good instruction file makes the safe path obvious, the risky path visible, and the forbidden path unavailable.

When the remaining ambiguity is harmless, the agent can continue.

When the remaining ambiguity affects scope, boundary, approval, verification, or responsibility, the agent must stop.

Plain speech is not shallow speech.

It is compressed control.

> Advice asks for good behavior. Routes enforce bounded orbits.
>
> — Cosmic Horizon

### The Last Read-Only Gate

Declaration marks the final read-only checkpoint before execution.

At this point, the agent has observed the project, grounded the task, and identified the intended route.

But it has not yet earned permission to change the world.

Before a non-trivial task enters execution, the agent must declare:

* what it observed
* what boundary defines the task
* what it plans to change
* what it plans to preserve
* how the result will be verified
* what remains uncertain

Until that declaration is accepted, the task remains read-only.

No files are edited.

No patches are generated.

No formatting is applied.

No refactor begins.

This gate exists because misunderstanding is cheapest before the working tree changes.

Once unintended edits enter the project, the human operator must spend attention recovering the original orbit.

A declaration gives the human one last chance to correct the trajectory before execution leaves debris in the working tree.

> The cleanest rollback is the one never needed.
>
> — Cosmic Horizon

### Proportional Momentum

A practical agent instruction system must keep task control proportional to task risk.

Not every edit requires the same level of structural control.

A simple wording change should not carry the same procedural weight as an architectural refactor, dependency change, or deployment change.

Three distinct orbits are enough to govern most AI-assisted workflows.

#### 1. The Fast Path — Low Risk

Used for simple formatting, wording, or minor documentation updates.

> **Observe → Execute → Report**

#### 2. The Default Path — Standard Risk

Used for tasks that alter source behavior, logic, project state, or execution flow.

> **Observe → Ground → Declare → Execute → Report**

#### 3. The Stop Path — High Risk / Ambiguity

Used when the agent encounters structural conflicts, boundary breaches, missing approval, or unresolved uncertainty.

> **Observe → Ground → Stop → Wait for human decision**

This is controlled momentum.

Uncertainty becomes a stop signal.

Ambiguity routes the agent to human decision, not autonomous interpretation.

> Momentum without boundary becomes drift.
>
> — Cosmic Horizon

### Sovereign Coordinates, Shared Missions

Agent instruction files can be intensely personal.

They reflect an individual developer’s philosophy, operating style, and threshold for risk.

These personal configurations may live locally, stay outside version control, or remain as private working artifacts.

Team-level and project-level instruction files serve a different purpose.

They represent shared operating agreements.

When a repository defines its own agent instruction file, that file becomes part of the project boundary for anyone working inside that repository.

Personal rules may still exist as local navigation aids.

When personal coordinates collide with shared project boundaries, the shared boundary governs the mission unless it is explicitly renegotiated.

A mature agent workflow separates three distinct layers of gravity:

* Personal Operating Style — private navigation aids and individual risk tolerance
* Team-Level Agreements — shared operational contracts and communication protocols
* Project-Specific Boundary Documents — observable constraints, invariants, danger zones, approval gates, and verification rules inside the Observatory Layer

Tools change.

Responsibility boundaries remain explicit.

### The Survival Log

This document is a survival log, not an absolute doctrine.

This framework records one way we learned to survive the drift: by capturing repeated failures, structural misunderstandings, and painful recovery patterns, then refining them into reusable boundary artifacts.

You may copy this structure.

You may adapt it.

You may reject it entirely and forge your own.

The goal is not to inherit this exact file blindly.

The critical mission is to define your own boundaries before an autonomous agent defines them for you.

> Personal coordinates guide the traveler.
>
> Shared boundaries govern the mission.
>
> Survived paths become maps for the next signal.
>
> — Cosmic Horizon

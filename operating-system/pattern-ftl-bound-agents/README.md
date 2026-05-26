---
description: Mapping Context Boundaries and Safe-Disengagement Rules for AI Agents
tags:
  - operating-system
---

# \[pattern] FTL-Bound Agents

> Survival Log from the Drift

## Current Coordinates

* Agent instruction files are prompts in the technical sense, but they are not disposable requests.
* A good AGENTS.md or CLAUDE.md does more than tell an AI agent what to do. It defines the world in which the agent is allowed to act.
* The purpose of an agent instruction file is to reduce dangerous interpretation space, not to carry every detail of the project.

## A Prompt, but Not Merely a Prompt

Technically, AGENTS.md, CLAUDE.md, and similar files are prompts.

They are instructions placed in front of an AI system. They shape how the agent reads the project, chooses actions, edits files, runs commands, and reports results.

Inside Cosmic Horizon, they are not treated as ordinary prompts.

An ordinary prompt asks for output.

An agent instruction file defines the operating boundary around output.

It tells the agent where to look, when to act, when to stop, what must not be inferred, and what must be reported before the work can be trusted.

This distinction matters because AI agents do not merely execute instructions.

They interpret them.

When the boundary is vague, the agent widens the task through interpretation.

When the boundary is clear, the agent moves inside a declared world. Assumptions are verified, not guessed. Execution stays inside a bounded orbit.

## Reduce the Mass

Agent instruction files should not become full project manuals.

If they try to contain every project rule, every architectural decision, every testing detail, and every warning, they become heavy, stale, and expensive to load into every task.

Their better role is not to contain the whole map.

They open controlled wormholes into project-specific space.

Through them, different AI agents can enter the right context, load the right boundary documents, and avoid drifting beyond the intended orbit.

**Agent instruction files define the route.**

They should define:

* when an agent may use the fast path
* when an agent must use the default path
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

Inside Cosmic Horizon, those documents form the Observatory Layer.

> Excessive mass collapses the orbit.
>
> — Cosmic Horizon

## Decouple the Wormhole

A reusable agent instruction system must separate common execution rules from project-specific boundaries.

Agent instruction files are not the project map.

They are controlled wormholes into project-specific space.

Depending on the environment, this wormhole may appear as `AGENTS.md`, `CLAUDE.md`, `GEMINI.md`, `.cursorrules`, Roo Code rules, Cline instructions, or another tool-specific entry point.

The project map must live elsewhere.

It belongs to the Observatory Layer, defined by stable boundary documents such as:

* `system_gravity.md`
* `invariants.md`
* `no_crossing_zones.md`
* `event_horizon.md`
* `approval_gate.md`
* `test_matrix.md`

These files do not need to exist in every project.

Deploy them only when the project scale, company governance, team conventions, or task domain requires them.

The point is not to enforce one universal filename, one rigid directory structure, or one identical instruction format across every tool.

The point is that every AI agent must know where to find project-specific boundaries.

When a boundary is missing, the agent must report it as missing.

It must not invent the map.

The wormhole may change by tool.

The map must remain observable.

> Entry points are ephemeral; boundaries are invariant.
>
> — Cosmic Horizon

## Chart Routes, Not Advice

Weak instruction files often sound reasonable on the surface.

They offer passive advice:

* be careful
* keep it simple
* make minimal changes
* use relevant files
* preserve the existing flow when possible

These sentences are not useless.

They are too soft.

They leave too much interpretation space.

What counts as simple?

What is relevant?

When is preservation possible?

What looks minimal to the model may still be destructive to the project.

Stronger instruction files do not advise.

They chart routes.

* **If** the task only changes wording or formatting → **use the fast path.**
* **If** the task changes source behavior → **use the default path.**
* **If** the task conflicts with an approval rule → **stop before execution.**
* **If** verification cannot be performed → **report the status instead of pretending.**
* **If** the scope is unclear → **do not widen it by interpretation.**

A route is stronger than advice.

Advice asks the model to behave well.

A route tells the model what to do when a condition appears.

### Control the Interpretation Space

Plain instructions do not remove interpretation.

They reduce dangerous interpretation space.

No agent instruction file can eliminate every act of abstraction, inference, or judgment.

AI agents still need to read context, compare patterns, choose tools, and decide how a rule applies to the current task.

The mission is not to erase interpretation.

The mission is to stop interpretation from becoming unauthorized execution.

A good instruction file makes the safe path obvious, the risky path visible, and the forbidden path unavailable.

When the remaining ambiguity is harmless, the agent may continue.

When the remaining ambiguity affects scope, boundary, approval, verification, or responsibility, the agent must stop.

Plain speech is not shallow speech.

It is compressed control.

> Advice asks for good behavior. Routes enforce bounded orbits.
>
> — Cosmic Horizon

## The Last Read-Only Gate

Declaration is the final read-only checkpoint before execution.

At this point, the agent has observed the project, grounded the task, and identified the intended route.

It has not earned permission to change the world.

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

Declaration gives the human one last chance to correct the trajectory before execution leaves debris in the working tree.

> The cleanest rollback is the one never needed.
>
> — Cosmic Horizon

## Proportional Momentum

A practical agent instruction system must keep task control proportional to task risk.

Not every edit deserves the same procedural weight.

A wording change should not carry the same burden as an architectural refactor, dependency change, or deployment change.

Three orbits are enough to govern most AI-assisted workflows.

### 1. The Fast Path — Low Risk

Used for simple formatting, wording, or minor documentation updates.

> **Observe → Execute → Report**

### 2. The Default Path — Standard Risk

Used for tasks that alter source behavior, logic, project state, or execution flow.

> **Observe → Ground → Declare → Execute → Report**

### 3. The Stop Path — High Risk / Ambiguity

Used when the agent encounters structural conflicts, boundary breaches, missing approval, or unresolved uncertainty.

> **Observe → Ground → Stop → Wait for human decision**

This is controlled momentum.

Uncertainty becomes a stop signal.

Ambiguity routes the agent to human decision, not autonomous interpretation.

> Momentum without boundary becomes drift.
>
> — Cosmic Horizon

## Sovereign Coordinates, Shared Missions

Agent instruction files can be intensely personal.

They reflect an individual developer’s philosophy, operating style, and threshold for risk.

These personal configurations may live locally, stay outside version control, or remain as private working artifacts.

Team-level and project-level instruction files serve a different purpose.

They represent shared operating agreements.

When a repository defines its own agent instruction file, that file becomes part of the project boundary for anyone working inside that repository.

Personal rules may still exist as local navigation aids.

When personal coordinates collide with shared project boundaries, the shared boundary governs the mission unless it is explicitly renegotiated.

A mature agent workflow separates three layers of gravity:

* Personal Operating Style — private navigation aids and individual risk tolerance
* Team-Level Agreements — shared operational contracts and communication protocols
* Project-Specific Boundary Documents — observable constraints, invariants, danger zones, approval gates, and verification rules inside the Observatory Layer

Tools change.

Responsibility boundaries remain explicit.

## The Survival Log

This document is a survival log.

It records one way to survive the drift: capture repeated failures, structural misunderstandings, and painful recovery patterns, then refine them into reusable boundary artifacts.

You may copy this structure.

You may adapt it.

You may reject it and forge your own.

The mission is not to inherit this exact file.

The mission is to define your own boundaries before an autonomous agent defines them for you.

## Next Coordinates

For the deeper perspective behind bounded, observable, and non-doctrinal AI-assisted work, read [Space Rations](../../perspective/space-rations.md).

For a concrete protocol derived from this pattern, see [AGENTS.md Blueprint](protocol-agents.md-blueprint.md).

Related signal:

Codex Chat Viewer is one practical artifact from this orbit: a local-first viewer for Codex CLI session logs, built to make AI-assisted work easier to inspect, review, document, and revisit after the work is done.

GitHub: [RGJ-sw1123r/codex-chat-viewer](https://github.com/RGJ-sw1123r/codex-chat-viewer)

> Personal coordinates guide the traveler.
>
> Shared boundaries govern the mission.
>
> Survived paths become maps for the next signal.
>
> — Cosmic Horizon


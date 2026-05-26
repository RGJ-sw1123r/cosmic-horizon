---
description: >-
  Why OpenAI Codex fits an operating system where human judgment stays above AI
  execution.
tags:
  - operating-system
---

# Codex as an Execution Layer

> Navigation Log

## Current Coordinates

* Tools should be chosen not by trend or attachment, but by the purpose of the voyage.
* In AI-assisted development, the core ability is not generating code faster. It is separating what humans must judge from what AI should execute.
* In this operating system, ChatGPT is the space for observation, planning, questioning, refinement, and documentation.
* Codex is the lower execution layer that moves inside already declared coordinates.
* In this document, Codex refers to the lower execution layer that is separated from the ChatGPT web conversation space, reads project context, edits files, and runs commands in the CLI.
* The core is not the OpenAI ecosystem in general, but the separation between the web planning space and the CLI execution space.
* This document describes an operating pattern where ChatGPT serves as the planning space and Codex serves as the execution layer.
* AGENTS.md and agent instruction files are not syntax tied to a specific vendor. They are operating devices that keep AI agents moving inside declared boundaries.
* The cost structure and workflow of a tool are not merely pricing issues. They are operating conditions that reshape how a worker thinks and executes.

## The Standard for a Good Tool

A good tool is not the tool currently in fashion.

A good tool is the tool that fits the voyage now being taken.

**Performance** matters.\
**Cost** matters.\
**Workflow** matters.

This is why I began the voyage with OpenAI Codex.

Familiarity played a role, of course.

ChatGPT was the first interface that made me accept AI as a serious working tool. Since around 2023, ChatGPT has been used continuously for thinking, drafting, review, development support, and documentation.

Because I have used it for a long time, it is familiar. There is also some attachment.

But Codex is not used merely because of familiarity or brand attachment.

This choice was calculated.

## Separating What Each Side Does Better

There is no need to hand everything to AI.

There are things humans must do better, and there are things AI can process faster.

In this operating system, Codex handles only the work placed below.

Above it is observation.\
Above it is requirement interpretation.\
Above it is UX judgment.\
Above it is constraint declaration.\
Above it is the declaration of completion criteria.

Codex is called only after all of this has been decided.

It is the layer that handles implementation inside coordinates that have already been observed, structured, documented, and declared.

Codex does not meet the customer.\
Codex does not directly observe user fatigue.\
Codex does not take final responsibility for why a screen is needed.\
Codex does not bear business context, organizational cost, dissatisfaction with existing systems, or hidden customer needs the way a human must.

So Codex is not the captain.

Codex is an execution layer that moves inside the coordinates I define.

## What Humans Must Do

This operating system places the following work in the upper layer.

* Observing what the customer actually wants.
* Reading where the customer feels fatigue.
* Separating UX dissatisfaction that existed in the legacy system.
* Deciding what result the screen must ultimately produce.
* Deciding what belongs in the MVP and what stays out.
* Distinguishing requirements from noise.
* Setting the color tone, brand context, and rhythm of the screen.
* Declaring the constraints implementation must obey.
* Defining the completion criteria.
* Separating the areas where AI may infer from the areas where it must not infer.

These are not implementation details.

These are the route-setting responsibilities of a developer.

AI can assist this process.

It can ask questions.\
It can point out missed conditions.\
It can compare alternatives.\
It can organize sentences.\
It can make prompts clearer.

But responsible decisions must remain in the upper layer.

When the upper layer is empty, lower-level execution shakes harder the faster it moves.

## Documentation Comes Before Execution

> Pre-AI: code without docs.\
> Post-AI: docs without code.

In the previous era of development, documentation was often created after the code had already been written.

In AI-assisted development, documentation comes first.

In this operating system, documentation is the layer that turns human judgment into coordinates AI can follow.

A good instruction is not a simple request.

A good instruction is a designed artifact.

The document must state what the goal is, what context must be preserved, what constraints must not be crossed, and what counts as done.

OpenAI’s Codex best practices also explain that good task instructions should include Goal, Context, Constraints, and Done when.

This standard is engineering for reducing the space AI must fill through inference alone.

It is a way to reduce the space AI must fill through inference alone.

This is also why long discussions happen with ChatGPT on the web.

They reduce the blanks Codex would otherwise have to fill through inference when it executes.

When humans observe, question, refine, and document enough, Codex moves along a safer route.

## What the Execution Layer Handles

Once the upper-layer judgment is organized, Codex handles what it does well.

It reads files.\
It modifies code.\
It runs commands.\
It implements repetitive structures quickly.\
It connects libraries.\
It cleans up imports.\
It runs tests.\
It leaves diffs.\
It creates reviewable output.

This work does not always need to be performed directly by human hands.

Implementation has value as execution inside a declared frame.

It means the center of gravity has moved.

If AI can implement faster, the attention of the human developer must move higher.

Better observation.\
Clearer constraints.\
Stronger verification.\
Sharper completion criteria.\
More recoverable work records that allow Return to Origin.

Codex is the implementer in this operating system.

It is not the subject that decides what must exist.

It is the execution layer that turns what has already been observed, structured, and declared into code.

## Why Separation Matters

In this workflow, separation matters.

The upper layer must think for a long time.

It must interpret customer requirements.\
It must narrow the MVP.\
It must organize UX dissatisfaction.\
It must define the purpose of the screen.\
It must declare constraints.\
It must rewrite the instruction into a unit AI can handle.

This stage belongs to planning and conception. It is navigation that makes the voyage safer.

If the thinking stage is reduced, output can arrive quickly.

But the cost of review, rollback, and responsibility grows afterward.

OpenAI Codex can currently be used within ChatGPT plans, but each plan has usage limits and Codex is included in agentic usage limits.

The key point in this document is the separation between the planning/conception space and the CLI execution space.

In the current workflow, ChatGPT is used as the space for observation, questioning, refinement, and documentation.

Codex CLI is used as the space that executes prepared coordinates inside the actual project.

When this separation is maintained, there is enough room to think before execution.

And when execution begins, a narrower and clearer instruction can be handed over.

A tool must not restrict the worker’s thinking.

Good navigation must allow enough observation and judgment in the upper layer, then make the voyage safer and faster.

## Coordinates Shown by 2025 Developer Statistics

The 2025 developer statistics show why this distinction matters.

AI use itself is no longer rare.

According to the Stack Overflow Developer Survey 2025, 84% of respondents said they use AI tools in the development process or plan to use them soon. Among professional developers, 50.6% said they use AI tools every day.

But when the question narrows from general AI use to agentic work, the numbers drop sharply.

Among professional developers, 14.9% said they use AI agents daily at work, 9.2% use them weekly, and 7.7% use them monthly or occasionally. Combined, about 31.8% of professional developers said they use AI agents at work.

In the same survey, Stack Overflow defined vibe coding as the process of generating software with LLM prompts. For this question, “Yes, emphatically” was 0.4%, “Yes” was 11.9%, and “Yes, somewhat” was 2.8%. Meanwhile, “No” was 72.2%, and “No, emphatically” was 5.3%.

| Category                                                                        | 2025 Indicator | Interpretation                                                                                    |
| ------------------------------------------------------------------------------- | -------------: | ------------------------------------------------------------------------------------------------- |
| Respondents who use or plan to use AI in the development process                |            84% | AI use itself has become mainstream.                                                              |
| Professional developers who use AI tools daily                                  |          50.6% | AI is becoming an everyday tool.                                                                  |
| Professional developers who use AI agents daily at work                         |          14.9% | Agentic work is still a minority practice.                                                        |
| Professional developers who said they use AI agents at work                     |          31.8% | Experience delegating real work to agents is growing, but it is not yet universal.                |
| Respondents who said vibe coding is part of their professional development work |          15.1% | The group that accepts prompt-based software generation as part of professional work is narrower. |
| Respondents who said vibe coding is not part of their work                      |          72.2% | Many developers use AI but do not call their work vibe coding.                                    |

These statistics do not directly prove this navigation system.

But they show one boundary.

AI use has become mainstream.

The group using AI agents at work is narrower.

The group accepting prompt-based software generation as a professional working method is narrower still.

And this survey does not ask whether developers first document customer requirements, UX judgment, constraints, and completion criteria before calling an AI agent as a lower execution layer.

That is where the coordinates of this document sit.

The practice of explicitly placing human judgment in the upper layer and controlling AI execution in the lower layer has not yet been clearly captured in ordinary survey language.

This document is an attempt to record a usage pattern that statistics have not yet named.

## A Usage Pattern the Statistics Do Not Describe

The Stack Overflow survey also shows another boundary.

Developers are relatively willing to bring AI into search, learning, code writing, documentation, and testing. By contrast, 76% said they do not plan to use AI for deployment and monitoring, and 69% said they do not plan to use it for project planning.

This boundary is reasonable.

Project planning, customer requirement interpretation, screen purpose definition, and UX judgment are not tasks to simply hand over to AI.

But that does not mean AI has no role in these areas.

AI can be an observation assistant, questioner, organizer, reviewer, and refiner of execution instructions, not the judge.

Handing project planning to AI is different from using AI to document project planning better so that a human can remain responsible for it.

Transferring responsibility and using AI to make responsibility clearer are different ways of working.

This operating system chooses the latter.

## Tool Choice Is an Operating Decision

Tool choice is not brand preference.

A tool is part of the operating system.

Therefore, this document examines the criteria for placing a tool in the execution layer of this workflow.

The question is tool fit: whether the tool preserves the separation between planning space and execution layer.

AGENTS.md and agent instruction files must be viewed by the same standard.

They are not Codex-only syntax. They are operating boundaries that can apply to AI agents that read project context and execute work, including Claude Code, Gemini CLI, Antigravity, and Codex.

The vendor may change.

But the principle does not change: an agent must be told where to look, when to move, what it must not infer, and where it must stop.

Claude Code can be a powerful tool. But Anthropic explains that Claude and Claude Code share usage limits on Pro and Max plans.

Google’s Gemini Code Assist documentation also explains that request quotas for Gemini Code Assist agent mode and Gemini CLI are combined, and that in agent mode or CLI, one prompt can lead to multiple model requests.

These details are not merely billing information.

They change the behavior of the workflow.

The upper-layer thinking stage is not wasted cost.

The upper-layer thinking stage is where lower-layer failures are reduced.

The documentation stage is where mistakes an agent might later create are reduced before they are born.

Declaring verification criteria first makes human responsibility visible.

A tool that makes this stage expensive or fragile does not fit this operating model well.

## Codex as a Market Signal

This does not mean OpenAI has removed all limits.

Codex has usage limits by plan. When users approach or reach those limits, they may need to add credits, upgrade, or wait for a reset depending on the plan.

But there is also a signal visible in the market.

When there was confusion around Claude Code pricing and plans, public responses from the OpenAI Codex side pointed to Codex being available within Free and Plus plans. Sam Altman also responded in the same flow: “We want you to have a lot of AI!”

That statement is not an official pricing policy document.

But it can be read as a market signal showing product direction.

At least at that moment, OpenAI publicly showed a direction of providing Codex broadly inside ChatGPT plans, rather than separating it only as an expensive standalone coding product.

For a workflow that observes and documents enough in the upper layer and leaves only execution to the CLI, this difference is significant.

A tool must not restrict the worker’s thinking.

A tool should make execution faster after sufficient observation and judgment have already taken place.

## Operating Sentence

Codex is not the center of this operating system.

The center is the observation and judgment that exist before Codex executes.

ChatGPT helps with upper-layer observation, questioning, refinement, and documentation.

Codex helps with lower-layer implementation, modification, execution, and verification.

The separation between the two is not a cost issue. It is an operating issue.

The faster AI implements, the more clearly humans must observe.

## Conclusion

OpenAI Codex is not the captain of this workflow.

Codex is not the navigation system either.

Codex is the execution layer installed below observation, judgment, and documentation.

In this operating system, the work of a human is not to type code faster than AI.

The work of a human is to responsibly declare the coordinates where AI can move.

Observe the customer.\
Understand the structure.\
Declare the boundary.\
Set the completion criteria.\
Hand execution to AI.\
Review the result.\
Return to the coordinates when needed.

That is why I use Codex.

**That is what a tool should be.**

⛵

## Related Coordinates

* Read [Ride, Don’t Race](../perspective/ride-dont-race.md) to connect this choice to the perspective of a rider who does not get dragged by the speed of the tool, but controls the tool at their own rhythm.
* Read [The Gravity Behind Market Language](../perspective/the-gravity-behind-market-language.md) to examine why the labels the market gives to AI tools must be translated into structure, cost, risk, and responsibility. This document applies that perspective to the choice of Codex.
* Read [AI-Assisted Development Models](ai-assisted-development-models.md) to understand the observation system behind this tool choice, and why Codex is placed in the lower execution layer only after requirements, constraints, boundaries, and completion criteria have been declared.
* Read [\[pattern\] FTL-Bound Agents](pattern-ftl-bound-agents/) to understand how agent instruction files act as operating boundaries so that execution layers like Codex do not expand the scope of work through interpretation.
* Read [\[protocol\] AGENTS.md Blueprint](pattern-ftl-bound-agents/protocol-agents.md-blueprint.md) to see how those boundaries can be implemented as a repeatable project instruction system in the form of AGENTS.md.

## Source Notes

* **OpenAI Codex Best Practices** — OpenAI, [Best practices – Codex](https://developers.openai.com/codex/learn/best-practices). Used to confirm that good task instructions should include Goal, Context, Constraints, and Done when.
* **OpenAI Codex CLI** — OpenAI, [Codex CLI](https://developers.openai.com/codex/cli). Used to describe the role of Codex CLI and its terminal-based execution environment.
* **OpenAI Codex with ChatGPT Plan** — OpenAI Help Center, [Using Codex with your ChatGPT plan](https://help.openai.com/en/articles/11369540-using-codex-with-your-chatgpt-plan). Used to describe Codex usage by plan and agentic usage limits.
* **Stack Overflow Developer Survey 2025 — AI Usage** — Stack Overflow, [Developer Survey 2025: AI](https://survey.stackoverflow.co/2025/ai). Used to check AI tool usage, AI agent usage, and vibe coding responses.
* **Anthropic Claude Code Usage** — Anthropic Help Center, [Use Claude Code with your Pro or Max plan](https://support.claude.com/en/articles/11145838-use-claude-code-with-your-pro-or-max-plan). Used to confirm the shared usage limit structure between Claude and Claude Code.
* **Google Gemini Code Assist Quotas** — Google Developers, [Quotas and limits | Gemini Code Assist](https://developers.google.com/gemini-code-assist/resources/quotas). Used to confirm the request quota structure for Gemini Code Assist agent mode and Gemini CLI.
* **OpenAI Codex Market Signal** — Business Insider, [Anthropic's Claude Code pricing pain is Sam Altman's pleasure](https://www.businessinsider.com/anthropic-claude-code-price-confusion-sam-altman-2026-4). Used to interpret Sam Altman’s “We want you to have a lot of AI!” remark and public responses around Codex availability in Free and Plus contexts as a market signal. Related X links: [Sam Altman](https://x.com/sama/status/2046752492093165708), [Thibault Sottiaux](https://x.com/thsottiaux/status/2046740759056162816).

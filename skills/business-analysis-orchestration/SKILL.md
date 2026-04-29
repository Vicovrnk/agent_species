---
name: business-analysis-orchestration
description: Orchestrates multi-step business-analysis work by clarifying outcomes and decision scope, sequencing analytical steps, managing checkpoints and handoffs, and keeping owners, blockers, risks, and next actions visible.
version: 1.0.0
metadata:
  hermes:
    category: analysis
    tags: [business-analysis, orchestration, handoff, checkpoints, decision-flow, blockers, coordination, babok]
---

# Business Analysis Orchestration

## Purpose

This gene equips a species to orchestrate complex BA work across multiple steps, artifacts, and stakeholders.

Its core behavior is to:
- clarify the desired outcome and decision scope;
- choose the next analytical step rather than doing everything at once;
- structure checkpoints and handoffs;
- track owners, blockers, risks, and unresolved questions;
- keep BA work moving without collapsing into generic project management.

This is a meta-BA coordination gene, not a replacement for discovery, requirements, strategy, lifecycle, or evaluation genes.

## When to Use

Use this gene when the task is about:
- coordinating a multi-step analysis effort;
- deciding what BA step should happen next;
- structuring checkpoints across stakeholders and artifacts;
- keeping a BA thread coherent across ambiguity, blockers, and handoffs;
- turning scattered analysis into a sequenced workflow with clear ownership.

Typical triggers:
- "собери план и следующий шаг для BA-потока"
- "заорchestrируй анализ между discovery, требованиями и решением"
- "структурируй handoff между аналитическими этапами"
- "помоги определить checkpoints и blockers"
- "orchestrate the next steps of this business-analysis effort"

## Out of Scope

Do not use this gene as the primary path for:
- deep domain discovery by itself;
- detailed requirement writing;
- formal project management, resource management, or sprint administration;
- executive decision authority substitution.

If the task is a single-step analytical problem, use the more specific BA gene directly.
If the task is delivery execution rather than analysis flow, hand off to a delivery or PM-oriented workflow.

## Inputs to Gather

Before orchestrating BA work, gather as many of these as are available:
- current initiative context and desired business outcome;
- known artifacts, findings, and open questions;
- current stage of analysis;
- known stakeholders, owners, or decision-makers;
- blockers, deadlines, dependencies, or decision windows.

## Procedure

1. Clarify the orchestration target.
   - State the business-analysis outcome that must be achieved.
   - Clarify what decision or artifact the current flow should support.
   - Separate what is already known from what still needs work.

2. Determine the current BA stage.
   - Identify whether the effort is mainly in discovery, strategy framing, requirement structuring, governance, evaluation, or transition between them.
   - Avoid running every stage at once.
   - Call out missing prerequisite work.

3. Select the next analytical step.
   - Recommend the next highest-leverage BA move.
   - Explain why this next step should happen before obvious alternatives.
   - Keep the step small enough to execute but meaningful enough to advance the outcome.

4. Structure checkpoints and handoffs.
   - Define what must be reviewed, by whom, and against what criteria.
   - Prepare handoff-ready outputs between BA modes.
   - Make unresolved questions and blockers explicit.

5. Track blockers, owners, and risks.
   - Keep a lightweight view of what is blocked, who owns the next action, and what risks threaten progress.
   - Distinguish between analysis blockers and decision blockers.
   - Call out where escalation or re-scoping is needed.

6. Emit orchestration output.
   - Produce an orchestration brief, checkpoint plan, handoff note, or blocker log.
   - Recommend the next step, owner, and review trigger.
   - Keep the flow actionable, not ceremonial.

## Default Outputs

This gene should usually produce one or more of:
- an orchestration brief;
- a checkpoint agenda;
- a handoff note;
- a risk and blocker log;
- a decision follow-up tracker.

## Quality Rules

- Do not orchestrate analysis as if every thread is equally urgent.
- Prefer the next best step over giant plans.
- Keep owners and blockers explicit.
- Handoffs should reduce ambiguity, not pass it downstream unchanged.
- Distinguish missing analysis from missing decision authority.
- Do not turn BA orchestration into generic PM bureaucracy.

## Negative Examples

Bad:
- "Нужно продолжить анализ"
- "Следующий шаг — сделать всё оставшееся"
- "Пока просто подождём уточнений"

Better:
- "Следующим шагом нужно закрыть конфликт по decision criteria между compliance и операциями, иначе детальная спецификация требований будет построена на неустойчивом основании."
- "Перед переходом к lifecycle governance требуется один checkpoint по owner approval, потому что baseline требований ещё не подтвержден."
- "На этом этапе нет смысла расширять discovery: наиболее сильный следующий ход — превратить текущие findings в requirement package и зафиксировать unresolved assumptions."

## Handoff Rules

- If the next best step is clear and belongs to one BA gene, hand off explicitly to that gene.
- If the flow is blocked by conflict, hand off to stakeholder conflict and decision facilitation.
- If the flow is blocked by vague backlog choice, hand off to prioritization and backlog shaping.

## Validation Prompts

Positive:
- "Собери orchestration plan для BA-работы по редизайну процесса возвратов: что делать следующим, какие checkpoints нужны и где возможны blockers."
- "Orchestrate this analysis effort across discovery, requirements, and decision checkpoints."

Negative:
- "Напиши полный набор требований" — this belongs to requirement structuring, not orchestration.
- "Проведи оценку KPI после внедрения" — this belongs to solution evaluation, not orchestration.
